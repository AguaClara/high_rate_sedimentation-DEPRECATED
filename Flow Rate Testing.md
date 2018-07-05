```python
from aguaclara_research.tube_sizing import *
from aide_design.shared.units import unit_registry as u
import numpy

# V_stock = 3*u.L
# dilution_factor = 0.8*u.mL/u.L
# density_stock = 1*u.g/u.mL

rpm = 10.2*u.rev/u.min
vol_per_rev = Q6_roller(ID_colored_tube("yellow-blue"))
print(vol_per_rev)
flow_theoretical = (rpm * vol_per_rev).to(u.mL/u.s)
print(flow_theoretical)

#############################################
mass_flow = (0.0430*u.ounce/u.min).to(u.g/u.s)
density = 1*u.g/u.mL
flow_actual = mass_flow / density
error = (flow_actual-flow_theoretical)/flow_theoretical
print(flow_actual)
print(error*100, "%")

C_coag = 70.28*u.g/u.L
m_flow_coag = (.0202*u.mL * 1.2165*u.mL/u.L * C_coag).to(u.mg)
concentration = m_flow_coag/((1.209829868*u.mL+0.0202*u.mL).to(u.L))
print(concentration)

# New dilution factor of 1.2165 mL/L of coagulant should obtain the correct coagulant dosage given an RPM of 10.2 for a 2 mm/s experiment

m_flow_coag = (flow_theoretical*u.s * 0.8*u.mL/u.L * C_coag).to(u.mg)
concentration = m_flow_coag/((1.013*u.mL).to(u.L))
print(concentration)
```
