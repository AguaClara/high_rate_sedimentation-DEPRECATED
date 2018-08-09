```python
from aguaclara_research.tube_sizing import *
from aide_design.shared.units import unit_registry as u
import numpy

#Tubing ID : volume output per revolution
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
  '''
  Parameters
  ----------
  Q_plant : float
    flow rate of the system, in u.mL/u.s
  C_plant : float
    concentration of substance of interest in the entire system, must have same
    units as C_stock
  C_stock : float
    concentration of stock solution of substance of interest, must have same
    units as C_plant

  Returns
  -------
  float : the mass-balanced flow rate of the stock solution of interest
  '''
  return (Q_plant * C_plant / C_stock).to(u.mL/u.s)


def C_stock(Q_plant, C_plant, Q_stock):
  '''
  Parameters
  ----------
  Q_plant : float
    flow rate of the system, in u.mL/u.s
  C_plant : float
    concentration of substance of interest in the entire system, in u.mg/u.L
  Q_stock : float
    flow rate of stock solution of substance of interest, in u.mL/u.s

  Returns
  -------
  float : the mass-balanced concentration of the stock solution of interest
  '''
  return (Q_plant * C_plant / Q_stock).to(u.mg/u.L)


def dilution_factor(C_stock, C_super_stock):
    '''
    Parameters
    ----------
    C_stock : float
        concentration of the stock solution connected to the pump
    C_super_stock : float
        concentration of the super stock solution from which stock is made
    '''
    return (C_stock / C_super_stock).to(u.mL/u.L)


def turbidity_to_concentration(turbidity):
  '''
  Parameters
  ----------
  turbidity : float
    must be in units of u.NTU

  Returns
  -------
  float : the concentration of kaolin clay for the desired turbidity, in milligrams
    of clay per liter of water
  Relation was determined by previous research documented on Confluence:
    https://confluence.cornell.edu/display/AGUACLARA/Clay+Concentration+in+Stock
    +Solution+for+Desired+Influent+Turbidity
  '''
  return (turbidity/u.NTU + 2.0839) / .3729 * u.mg/u.L

#######################################################

#SYSTEM PARAMETERS
C_clay = 100*u.NTU            #system influent turbidity
C_pacl = 2.8*u.mg/u.L         #system coagulant dosage
tubing_clay = "yellow-blue"   #color coding of Masterflex tubing for clay pump
tubing_pacl = "yellow-blue"   #color coding of Masterflex tubing for coagulant pump

sed_tank_radius = 0.5*u.inch  #inner radius of sedimentation tank
upflow_velocity = 3           #sed tank upflow velocity, in mm/s

cross_sectional_area = numpy.pi * (sed_tank_radius.to(u.cm)) ** 2
Q_sys = (upflow_velocity/10*u.cm/u.s * cross_sectional_area).to(u.mL/u.s)

print("CALCULATIONS FOR UPFLOW VELOCITY OF", upflow_velocity, "MM/S \n")
print("System flow rate: ", Q_sys, "\n")


#CLAY CONCENTRATION AND PUMP SPEED CALCULATIONS
C_clay_stock = 5.4*u.g/u.L    #concentration of clay stock (mg kaolin clay per
                              #liter of water)

C_clay_sys = turbidity_to_concentration(C_clay)
Q_clay = Q_stock(Q_sys, C_clay_sys, C_clay_stock)
print("Clay stock concentration:", C_clay_stock)
print("Clay pump speed (average):", pump_rpm(Q_clay, tubing_clay), "\n")


#COAGULANT CONCENTRATION CALCULATIONS
C_super_stock = 70.28*u.g/u.L   #concentration of super stock solution from
                                #which stock is made   
pacl_flow_3_rpm = 0.0063786375*u.mL/u.s  #flow rate when coagulant pump is running
                                         #at 3 rpm (chosen for being near the
                                         #lowest speed of the pump),
                                         #EXPERIMENTALLY DETERMINED
rpm_pacl = 9*u.rev/u.min        #desired coagulant pump speed   

Q_pacl = pacl_flow_3_rpm * rpm_pacl/(3*u.rev/u.min)
C_pacl_stock = C_stock(Q_sys, C_pacl, Q_pacl)
print("Coagulant pump speed:", rpm_pacl)
print("Coagulant stock concentration:", dilution_factor(C_pacl_stock, C_super_stock), "\n")


#WATER PUMP CALCULATIONS
Q_water = Q_sys - Q_clay - Q_pacl
tubing_water_ID = 17
Q_rev_water = tubing_water[tubing_water_ID]
rpm_water = (Q_water/Q_rev_water).to(u.rev/u.min)
print("Water pump speed:", rpm_water)
```
