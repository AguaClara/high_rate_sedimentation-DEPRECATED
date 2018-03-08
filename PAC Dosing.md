#PAC Dosing
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

print('Mehrin is soo awesome and thinks that Mike is really dope! Please be nice to her! :)')
print('Mike, I staged changes and committed this file. Please just push this out to GitHub!')
```
