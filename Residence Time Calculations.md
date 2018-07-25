```python
from aide_design.shared.units import unit_registry as u
import numpy as np

L_recirc = 18*u.inch
L_tube_settler = 16.5*u.inch
area = np.pi*(0.5**2)*(u.inch**2)
volume = (L_recirc + L_tube_settler) * area

upflow_velocity = (3*u.mm/u.s).to(u.inch/u.s)
waste_flow = (3.8*u.mL/u.rev * 1*u.rev/u.min).to(u.inch**3/u.s)
flow_rate = upflow_velocity * area - waste_flow

res_time = volume / flow_rate
print(res_time.to(u.min))
```
