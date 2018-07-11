```python
from aguaclara_research.tube_sizing import *
from aide_design.shared.units import unit_registry as u
import numpy

#Tubing ID : volume per revolution
#Obtained from Masterflex tubing specs, summarized on Confluence:
#https://confluence.cornell.edu/display/AGUACLARA/Auto+Tutorial+for+
#Peristaltic+Pumps
tubing_water = {
  13 : .06*u.mL/u.rev,
  14 : .21*u.mL/u.rev,
  16 : 0.8*u.mL/u.rev,
  17 : 2.8*u.mL/u.rev,
  18 : 3.8*u.mL/u.rev
}

def Q_stock(Q_plant, C_plant, C_stock):
  return (Q_plant * C_plant / C_stock).to(u.mL/u.s)

def turbidity_to_concentration(turbidity):
  ''' Precondition: turbidity is in units of NTU '''
  return (turbidity/u.NTU + 2.0839) / .3729 * u.mg/u.L

####################################################################

#System parameters, in relation to the sedimentation tank
C_clay = 100*u.NTU
C_pacl = 1.4*u.mg/u.L
tubing_clay = "yellow-blue"
tubing_pacl = "yellow-blue"

upflow_velocity = 2 #in millimeters per second
print("CALCULATIONS FOR UPFLOW VELOCITY OF", upflow_velocity, "MM/S \n")

cross_sectional_area = numpy.pi * (0.5*u.inch * 2.54*u.cm/u.inch) ** 2
Q_sys = (upflow_velocity/10*u.cm/u.s * cross_sectional_area).to(u.mL/u.s)
print("System flow rate: ", Q_sys, "\n")

'''
#Current coagulant (PACl) concentration and pump speed
print("CURRENT COAGULANT DOSAGE CALCULATIONS")
C_super_stock = 70.28*u.g/u.L
V_stock = 5*u.L
dilution_factor = 0.8*u.mL/u.L
V_super_stock = V_stock * dilution_factor
print("Current volume of coagulant super stock to add: ", V_super_stock)

M_stock = (C_super_stock * V_super_stock).to(u.g)
C_stock = M_stock / V_stock #Note: C_stock= C_super_stock * dilution_factor/1000
print("Current concentration of coagulant stock: ", C_stock)

Q_stock_pacl = (Q_sys * C_pacl / C_stock).to(u.mL/u.s)
rpm_pacl = pump_rpm(Q_stock_pacl, tubing_pacl)
print("Current coagulant pump speed:", rpm_pacl, "\n")


#Recommended coagulant (PACl) concentration and pump speed
print("RECOMMENDED COAGULANT DOSAGE CALCULATIONS")
rpm_pacl = min_rpm
print("Minimum coagulant pump speed:", rpm_pacl) #defined in tube_sizing.py

C_stock = C_stock_max(Q_sys, C_pacl, tubing_pacl)
print("Maximum concentration of coagulant stock: ", C_stock)

dilution_factor = C_stock / C_super_stock * 1000 * u.mL/u.L
V_super_stock = V_stock * dilution_factor
print("Maximum volume of super stock: ", V_super_stock)


#aguaclara_research water pump speed calculation
Q_water = Q_water(Q_sys, C_clay, C_pacl, tubing_clay, tubing_pacl)
tubing_water_ID = 17
Q_rev_water = tubing_water[tubing_water_ID]
rpm_water = Q_water/Q_rev_water
print("Water pump speed:", rpm_water, "\n")
'''

#Our water pump speed calculation
C_clay_sys = turbidity_to_concentration(C_clay)
C_clay_stock = turbidity_to_concentration(3500*u.NTU)
Q_clay = Q_stock(Q_sys, C_clay_sys, C_clay_stock)
print("Clay stock concentration:", C_clay_stock)
print("Clay flow rate:", Q_clay)
print("Clay pump speed (average):", pump_rpm(Q_clay, tubing_clay), "\n")

#Q_pacl = Q_stock_pacl
Q_pacl = 0.0063786375*u.mL/u.s * 2
print("Pacl flow rate:", Q_pacl)
# print("Pacl pump speed:", pump_rpm(Q_pacl, tubing_pacl))
print("Pacl pump speed:", 9, "\n")

Q_water = Q_sys - Q_clay - Q_pacl
tubing_water_ID = 17
Q_rev_water = tubing_water[tubing_water_ID]
rpm_water = (Q_water/Q_rev_water).to(u.rev/u.min)
print("Water flow rate:", Q_water)
print("Water pump speed:", rpm_water)


```
