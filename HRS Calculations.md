```python
from aguaclara_research.tube_sizing import *
import numpy
from aide_design.shared.units import unit_registry as u

def vol_per_rev(diameter):
    R_pump = 1.62 * u.cm
    k_nonlinear = 13
    term1 = (R_pump * 2 * numpy.pi - k_nonlinear * diameter) / u.rev
    term2 = numpy.pi * (diameter ** 2) / 4
    return (term1 * term2).to(u.mL/u.rev)

Q_sys =.1*numpy.pi*(.5*2.54)**2*u.mL/u.s

C_clay = 100*u.NTU
C_pacl_min = 1.4*u.mg/u.L
tubing = "yellow-blue"
Q_water = Q_water(Q_sys, 100*u.NTU, 1.4*u.mg/u.L, tubing, tubing)

print("Our Calculations")
Q_rev_water = 82.6*u.mL/u.min/(25*u.rev/u.min)
print("Volume per rev for water pump:", Q_rev_water)
rpm_water = Q_water/(Q_rev_water)
print("Water pump speed: ", rpm_water, "\n")

print("AguaClara Research Calculations")
print("Volume per rev for water pump:", vol_per_rev(6.4*u.mm))
rpm_water = Q_water/vol_per_rev(6.4*u.mm)
print("Water pump speed: ", rpm_water, "\n")

#Current Concentration
C_super_stock = 70.28*u.g/u.L
V_stock = 5*u.L
dilution_factor = 0.8*u.mL/u.L
V_super_stock = (V_stock*dilution_factor)
print("Current volume of super stock: ", V_super_stock)

M_stock = (C_super_stock*V_super_stock).to(u.g)
C_stock = M_stock/V_stock
print("Current concentration of coag stock: ", C_stock, "\n")
#C_stock = 70.28*.8/1000) = C_super_stock * dilution_factor/1000

#Recommended Concentration
C_coag_max = C_stock_max(Q_sys, 1.4*u.mg/u.L, tubing)
print("Max concentration of coag stock: ", C_coag_max)
Q_coag_min = Q_stock_max(Q_sys, 1.4*u.mg/u.L, tubing)
print("Corresponding coagulant flow rate: ", Q_coag_min)
rpm_coag = pump_rpm(Q_coag, tubing)
print("Corresponding coagulant pump speed:", rpm_coag)

dilution_factor = C_coag_max/C_super_stock*1000
print("Corresponding dilution factor: ", dilution_factor*u.mL/u.L)
print(5*dilution_factor)
```
