## PAC Dosing

**Attention: The calculation for coagulant pump speed (RPM) is outdated. Please see [Pump Speed and Stock Calculations.md](https://github.com/AguaClara/high_rate_sedimentation/blob/master/Calculations/Pump%20Speed%20and%20Stock%20Calculations.md) in the Calculations folder of our Github repository for a corrected calculation.** 

```python
from aide_design.play import*

#inputs
C_sys = 1.4*(u.mg/u.L)
C_labstock = 70.9*(u.g/u.L)
Q_sys = 1.48*(u.mL/u.s)
K_dilution = .8*(u.mL/u.L)
V_resivor = 5*(u.L)
Frac_resivor = .76
Q_per_rpm = .001828 *(u.mL/u.s)

#Calculations
M_flow_coag = (Q_sys * C_sys).to(u.mg/u.s)
C_resivor = (C_labstock * K_dilution).to(u.gram/u.L)
Q_resivor = (M_flow_coag / C_resivor).to(u.mL/u.s)
V_lab = ((V_resivor * C_resivor) / C_labstock).to(u.L)

#Outputs
RPM = Q_resivor / Q_per_rpm
RunTime = ((V_resivor * Frac_resivor) / Q_resivor).to(u.hour)

print('The RPM needed for this coagulent dosage is' ,RPM)

print('The run time is ', RunTime)
```
