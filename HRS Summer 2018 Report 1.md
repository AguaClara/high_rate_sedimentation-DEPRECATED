#High Rate Sedimentation, Summer 2018
#### Hannah Si and Anna Hong
#### June 29, 2018

##Abstract
Since Spring 2018, the AguaClara High Rate Sedimentation (HRS) team has been investigating the cause behind floc blanket decay in the sedimentation tank, which has been attributed to system failure at high upflow velocities. Along with conducting a small series of experiments, the Summer 2018 HRS team has developed a more robust experimental apparatus and clear set of instructions for setup.

##Methods
###Experimental Apparatus
Below is a picture of the revised lab bench setup of the HRS team followed by a table listing the various components.

<p align=center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/updatedlabbenchsetup.JPG" width = 500>
</p>

Figure 1. Labeled experimental setup for the High Rate Sedimentation lab bench

| Label | Component             |
|:-----:| :-------------------- |
|   1   | Water Pump            |
|   2   | Clay Pump             |
|   3   | Coagulant Pump        |
|   4   | Waste Pump            |
|   5   | Flocculator           |
|   6   | Pressure Sensor       |
|   7   | Influent Turbidimeter |
|   8   | Effluent Turbidimeter |
|   9   | Pressure Attenuator   |
|  10   | Coagulant Stock       |
|  11   | Clay Stock            |
|  12   | Sedimentation Tank    |
|  13   | Waste Tube            |

###Setup Procedures
####Original configuration

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Original%20Configuration.png" width = 500>
</p>

For detailed instructions and guidelines on preparing the High Rate Sedimentation experimental setup, refer to the HRS Setup Procedures document in our Github repository. (PUT HYPERLINK)

1. Drain the sedimentation tank.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/DrainSed.png" width = 500>
</p>

2. Clean the flocculator and sedimentation tank.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Step2.png" width = 500>
</p>

3. Clean out the pressure attenuator.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/PressureAttentuator.png" width = 500>
</p>

4. Disconnect the coagulant pump from system and check if coagulant is pumping through. Then reconnect it to the system.
   * Make sure the coagulant valve is open. There should be steady droplets of solution.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/CoagulantStock.png" width = 500>
</p>

5. Run water through the system while bypassing the pressure attenuator.
<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/CleanWaterRun.png" width = 500>
</p>

6. After the water reaches the top of the sed tank, shut off the water pump and drain the sed tank again.
   * Repeat steps 5 and 6 to achieve a more thorough cleaning of the sed tank.

7. Run water only through the system with the pressure attenuator included until effluent turbidity stabilizes near 0 NTU (ideally below 1.0 NTU).

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Step%207.png" width = 500>
</p>

8. Clean out the influent and effluent turbidimeters.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Step%208.png" width = 500>
</p>

9. Direct the flow to waste instead of the flocculator.

10. Turn the clay stirrer and ProCoDa on.

11. Stabilize influent turbidity to 100 NTU.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Stabilize%20influent.png" width = 500>
</p>

12. Redirect the flow back to the flocculator and main system. Turn on the coagulant pump to start the experiment.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/LastStep.png" width = 500>
</p>

###Experiments and Results

#####Experiment 1
Description:
Result:

###Results and Analysis


###Calculations
We have written code in Python for calculating the system flow rate, water pump speed, coagulant concentration, and coagulant pump speed given an upflow velocity and other parameters.

```python
from aguaclara_research.tube_sizing import *
from aide_design.shared.units import unit_registry as u
import numpy

#Tubing ID : volume per revolution
tubing_water = {
  13 : .06*u.mL/u.rev,
  14 : .21*u.mL/u.rev,
  16 : 0.8*u.mL/u.rev,
  17 : 2.8*u.mL/u.rev,
  18 : 3.8*u.mL/u.rev
}

#System parameters, in relation to the sedimentation tank
upflow_velocity = 1 #in millimeters per second
print("CALCULATIONS FOR UPFLOW VELOCITY OF", upflow_velocity, "MM/S \n")

cross_sectional_area = numpy.pi * (0.5*u.inch * 2.54*u.cm/u.inch) ** 2
Q_sys = (upflow_velocity/10*u.cm/u.s * cross_sectional_area).to(u.mL/u.s)
print("System flow rate: ", Q_sys, "\n")

C_clay = 100*u.NTU
C_pacl = 1.4*u.mg/u.L
tubing_clay = "yellow-blue"
tubing_pacl = "yellow-blue"

#Water pump speed
Q_water = Q_water(Q_sys, C_clay, C_pacl, tubing_clay, tubing_pacl)
Q_rev_water = tubing_water[17]
rpm_water = Q_water/Q_rev_water
print("Water pump speed:", rpm_water, "\n")

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

Q_stock = (Q_sys * C_pacl / C_stock).to(u.mL/u.s)
rpm_pacl = pump_rpm(Q_stock, tubing_pacl)
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
```
