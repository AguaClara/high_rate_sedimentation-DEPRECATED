# High Rate Sedimentation, Spring 2018
#### Mike Zarecor, Sneha Sharma, Justin Conneely
#### March 9th, 2018

## Abstract
Past High Rate Sedimentation teams have hypothesized that floc blankets thin as experiments progress due to coagulant sticking to the walls of the flocculator, reducing the overall coagulant dosage. The 2018 spring team has conducted an experiment to test if increasing the coagulant dosage solves this problem and leads to stable floc blankets. The results currently indicate that this will solve the floc blanket degredation problem, but more work should be done.

## Introduction
Sedimentation is a critical process for water treatment plants. It is the process by which coagulated minerals, dirt, clay, and other particles are removed from the water via gravitational settling. The particles settle into a "floc" - a fluidized bed of suspended solids colliding in a bottom zone of the tank. The particles are initially light and small, but as coagulant dosage persists and particles continue to collide,  the particles clump together into heavier floc that will settle into the basin of the recirculator. This process permits clearer water to continue up the plate settler, resulting in a lower effluent NTU (Nephelometric Turbidity Unit, a measure of clarity).

AguaClara's sedimentation tank design includes inclined parallel plates called plate settlers. The purpose of these plates is to catch small particles and return them to the floc blanket developing in the base of the tank. In the AguaClara lab, a sedimentation tank and its respective plate settlers are simulated by tubing. The tube that simulates a pathway of fluid in the tank is referred to as  the "recirculator" by the High Rate Sedimentation (HRS) team.

The slanted tube that simulates a plate settler is designated  as the "tube settler." See Figure 1 for a visual representation of this concept. The plate settlers increase the amount of horizontal area for the flocs to settle out. Due to their sticky nature, these flocs aggregate; growing in size as they slide down the plate settler and back into the basin.

![SedimentationTank](https://www.overleaf.com/docs/11173977ftrfnxyhrpyv/atts/59342342)
Figure 1: The recirculator and tube settler simulate the sedimentation tank basin and plate settlers respectively. Since the behavior of a section of fluid is characteristic of the entire tank, tubing can be used to simulate a simple pathway in the reactor. This allows for a practical form of experimentation that is small scale, easy to manipulate, and representative of the respective tank design.

AguaClara designed a vertical sedimentation tank, which has the water flow from the bottom of the tank to the top. The flow velocity that maintains the floc blanket is known as overflow rate or upflow velocity. Flow rate (Q), upflow velocity (V), and tank surface area (A) are related to the continuity equation:

$$ Q = V * A $$

The AguaClara HRS team hopes to design a tank that will yield an effluent of 0.3 NTU or lower with maintaining high upflow velocity. While the World Health Organization has a standard of at most 1 NTU for drinking water, the EPA standard is 0.3 NTU. AguaClara currently achieves this with an upflow velocity of 1 mm/s, but not at upflows of 3 mm/s or greater. A larger upflow velocity would allow for a reduction in treatment plant size, which would reduce construction costs.

## Literature Review and Previous Work
Culp et al. (1968) used tubes to figure out the optimal slope of the tube settlers. Under laboratory conditions, a 60 degree angle with respect to the horizontal provided continuous sludge removal while showing effective sedimentation performance. This information was used by the Fall 2017 team when designing the tube settler currently being used by the Spring 2018 team.

Hurst (2010) stated that the presence of the floc blanket would enhance the removal of turbidity causing particles. These experiments found that upflow velocities of 1.0 to 1.3 m/s produced the best performance. Past teams have tried to  implement his findings at higher upflow velocities, but have been unable to develop stable floc blankets.

Swetland (2014) Found that as flocs formed, they would sediment due to their higher density compared to water. The flocs must settle faster than the upflow velocity. As the flocs concentrated and fell down to the bottom of the tank, a floc blanket formed. These findings defined the High Rate Sedimentation teams's understanding of a floc  formation, which is a critical step of the AguaClara sedimentation process.

Balwan (2016) explored the effect of the length of tube settler on effluent turbidity. As indicated in his report, increasing the length of tube settlers increased the percentage of turbidity removed (defined as percentage change between influent and effluent turbidity). With tube settlers in 45 degrees inclination angle and 60 cm length, turbidity removal was measured to be 80 percent. However, his experiments only had three length variables (40cm, 50cm, 60cm) and the effluent of longer tube settlers were unknown.

 The Fall 2017 High Rate Sedimentation team experimented with varied sedimentation tank geometries in an attempt to find a configuration that allowed for stable floc blankets. They were unsuccessful; however, they found that they could not reestablish floc blankets mid experiment, and that headloss increased as the experiment progressed. This led to their floc accumulation hypothesis. This hypothesis suggests that coagulent sticks to the inside of the flocculator tubing, reducing the effective dosage of coagulent. The 2018 spring team began by testing this idea.

## Methods
### Experimental Apparatus
The overall lab bench set up of the HRS team is composed of several parts (Figure 10). These parts include the pumps, the stocks, the flocculator, and the turbidimeters.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Lab%20Bench%20Setup.png" height250 width=400>

Figure 2: The HRS lab bench setup is composed of the turbidimeters, stocks, pumps, and a flocculator.

This system allows the team to simulate non-potable water and its treatment through high rate sedimentation while keeping track of performance via NTU. The influent and effluent turbidimeters are what tell the team how well the system is performing at any given time. In order to run experiments, tap water is contaminated with clay from the Clay stock. This contaminated water is known as the influent and is kept at a constant NTU of 100 through ProCoDA by utilizing PID control. For more on Clay dosing, see the Manual.

Once the influent passes through the turbidimeter, it moves through the flocculator. Upon entering the flocculator, the untreated water is dosed with Poly-Aluminum-Chloride (PAC), which is the coagulant Aguaclara utilizes. The Coagulant pump is manually set up to control how much of the Coagulant stock enters the system. When a dose is chosen, the team uses a python doc (converted from the team's old MathCAD files) to determine the stock concentration and required RPM of the pump. For more on Coagulant dosing, see the Manual. The treated water then passes through the coiled tube that is the flocculator, which allows for the formation of flocs. The end of the flocculator then enters the bottom of the recirculator where upflow begins. The effluent that exits through the top of the tube settler then flows through the effluent turbidimeter. This is where the turbidity of the effluent is determined; the goal is to reach an NTU of 0.3 or lower. After the effluent turbidimeter, the wastewater flows out towards the wastewater drainage.

All particle removal teams are currently utilizing the HRS standard apparatus design and a flocculator designed by the High G Flocculation Fall 2017 team. The flocculator’s purpose is to mimic the flocculation process in an actual AguaClara plant with a sufficient collision potential (G). The High G flocculation team provides information on the following table with the flocculator’s dimensions and the resulting values for an upflow velocity of 3 mm/s.

| Parameter | Meaning | Value |
| ----- | ------------------------ | ----- |
| V.Sed | Sed Tank Upflow Velocity | 3 mm/s |
| D.Sed | Sed Tank Inner Diameter  | 1 in  |
|Q.Sed, Q.Reactor| Flow rate (from V.Sed) |1.52 mL/s|
|D.Floctube|Floctube Inner Diameter| 0.17 in |
|R.c|Radius of Curvature of Floc Coils|5 gm|
| Gtheta | G*theta | 20,000 |
|  G  |  Shear   |  175.5 Hz  |
|Theta |Residence Time | 1.899 min or 113.9 s|
| L.Flocc| Length of Flocculator Tubing|11.821 m|
|Epsilon.Flocc |Energy Dissipation Rate| 30.814 mW/kg|

Table 1: The HRS lab bench setup consists of a flocculator developed by the High G Flocculation Fall 2017 team. The above are the parameters and resulting values of the current flocculator design.

### The Standard Design

This section contains the theories, steps, and progress the Fall 2017 team followed in order to fabricate the five reactors that all particle removal teams are to use for their experiments (flouride removal, high G flocculation, etc.). For more information on the work that these teams are involved in, see AguaClara’s Github page.

Design: The geometry of the apparatus is based on the concept of ”capture velocity.” Capture velocity is the slowest moving particle that an area can capture and is a property of the sedimentation tank. In other words, the greater a particle’s terminal settling velocity, the less distance it must travel and the more likely it is to be captured. Terminal settling velocity is reached when the frictional force (viscous shear) of the fluid, combined with the buoyant force, balances with the gravity. The larger the diameter of a particle, the greater its terminal velocity. This relationship may be shown through Stoke’s Theorem as seen in the following formula:

$$ V_t = \frac{d^2g}{18v} ∗ \frac{ρ_{floc} − ρ_{H_2O}}{ρ_{H_2O}} ... (2)$$

Where d is the diameter of the pipe, g the gravity force, v is viscosity and ρ represents the different densities of the water and the floc.

On the other hand, capture velocity depends on the dimensions of the apparatus being used, as
one can see in the following formula:

$$ V_c = \frac{SV_αsinα}{Lsinαcosα+S} ... (3)$$

Where α is the angle of the tube settler, V<sub>α</sub> is the upflow velocity, L is the length of the tube settler
(after the floc weir), and S is the diameter of the tubing. If a floc has a terminal settling velocity
that is too low, it will not be captured and instead will escape with the effluent.

A floc blanket has the potential to climb up to the weir, so the distance after the floc weir is used as the active length of the tube settler in the capture velocity calculation. In the case of the standard design, with an effective length of 27.08 cm, the resulting capture velocity is .462 mm/s. In order to be consistent with previous research teams, the tube settler is at a 60<sup>o</sup> bend in relation to the x-axis in the Fall 2017 model. Also, the inner diameter is set to 1 inch rather than 3/4 inches.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Screen%20Shot%202018-03-08%20at%2011.53.45%20PM.png" height250 width=400>

Figure 3: A diagram of the active tube settler length L, the inner diameter of the apparatus S, and the angle α.

Materials: In the Fall 2017 model, the floc weir is welded onto the tube settler rather than the
recirculator and the apparatus is enclosed by compression fittings. The reason for an intermittent floc weir on the tube settler is due to the findings of the Summer 2017 team. If a floc blanket could
be established with a low bend, then further investigation is required on whether multiple bends
characteristic of the trapezoidal apparatus are necessary for performance, or just keep essential
flocs low and recirculating.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Screen%20Shot%202018-03-08%20at%2011.53.29%20PM.png" height250 width=400>

Figure 4: The standard design includes a 50 cm recirculation zone, a 36.47 cm tube settler, an a 40 cm long floc weir. The inner diameter of the PVC tubing is 1 inch rather than 3/4 inches like previous
semesters.

Compared to previous semesters, the size of the apparatus has been reduced a considerable amount.
It is important to note that the team’s goal is not necessarily to reduce turbidity more than what the trapezoidal was able to achieve, but rather to investigate possible alternatives to sedimentation tank design in order to avoid the complex geometry that the trapezoidal design implicates. Since the tubing size increased from 3/4 inch to 1 inch, the flow rate of influent water had to be altered in order to achieve the 3 mm/s upflow velocity that is unique to high rate sedimentation. The following equation is used in order to help the team determine these values:

$$ V_{floc} = \frac{Q_{floc}}{\frac{D^2_{pipe}}{4} ∗ π} ... (4) $$

Where Q<sub>floc</sub> is the volumetric flow of water through the system and D<sub>pipe</sub> is the inner diameter of the PVC pipe.

### Procedure
Using the aforementioned set-up, the HRS team tests the effect of increasing coagulant dose on floc blanket degradation and effluent turbidity. This is tested by first flushing the system to assure it was clean of coagulant and clay particles, then setting the influent turbidity to 100 NTU. Then the team tests varying doses of coagulant with a constant upflow velocity in the sedimentation tank of 3 mm/s (experimentally extrapolated from an RPM of 28.3). The first experiment is conducted at a coagulant dosage of 1.4 mg/L and a corresponding coagulant pump RMP of 20. That initial coagulant dose was then increased incrementally, then tested under the same conditions as above.

## Results and Analysis
It is believed that the floc blanket eventually degrades as a result of the coagulant adhering to the walls of the tubing. Thus, it was hypothesized that increasing the concentration of the coagulant would compensate for the amount of coagulant  sticking to the tubing's walls. The hypothesis was tested by varying the coagulant dose with respect to time over a period of 24 hours.

Increasing the PAC dose led to a lower effluent turbidity, as is illustrated in Figure 15. These results support the hypothesis that increasing coagulant dose would increase the longevity of the floc blanket. Based on the results obtained from the first four trials of the experiment, it is expected that increasing the coagulant dose will continue to increase the life of the floc blanket until a threshold value is reached.

![Figure15](https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Experiment%201.JPG)

Figure 5: The effluent turbidity over 24 hours at varied coagulant doses. This confirms that increasing the coagulant dose decreases the rate of floc blanket decay.

## Conclusions
Based on the above data, the HRS team was able to conclude that increasing coagulant dose mitigated floc blanket degradation. This confirms our hypothesis that this aforementioned floc blanket degradation was occurring due to coagulant sticking to the walls of the flocculator, which in turn decreased the effective coagulant concentration and floc blanket duration.

## Future Work
Future work should include more trials under experiment one until a fully stable floc blanket is possible. After this experiments testing varried basin geometry could be conducted in an effort to optimize removal at high upflow velocities.

## Bibliography

Balwan, K. (2016). Study of the effect of length and inclination of tube settler on the effluent quality. Journal (International Journal of Innovative Research and Advanced Engineering).

Culp, G., Hansen, S., & Richardson, G. (1968). High-rate sedimentation in water treatment works. Journal (High-Rate Sedimentaion in Water Treatment Works).

Hurst, M. (2010). Evaluation Of Parameters Affecting Steady-State Floc Blanket Performance. Thesis (Cornell University).

Galantino, C., Oritz, A., & Zarecor, M. (2017). High Rate Sedimentation Fall 2017 Report.

Swetland, K., Weber-Shirk, M., Lion, L. (2014).  Flocculation-sedimentation performance model for laminar flow hydraulic flocculation with polyaluminum chloride and aluminum sulfate coagulants. Journal (Journal of Environmental Engineering).

# Manual

## Experimental Methods
### Set-up
1. Make sure the set up is throughly cleaned out and the stocks are replenished. Open the valves for the water supply as well as the wastewater tube. Fill the recirculator and tube settler with water by turning on the water pump, but keep the effluent turbidimeter closed. To speed up the process of filling up the apparatus with water, increase the RPM of the water pump.
2. Once the apparatus is filled, pause the water pump, close the valve to the wastewater, and use a push pin to replace the influent turbidimeter outflow tube on the connection between the flocculator and influent turbidimeter.
3. Turn on the water pump to the respective RPM for your experiment. Be sure to put the outflow tube of the influent turbidimeter in a container to collect the water that will be flowing through the influent turbidimeter.
4. Turn on ProCoDA by going to process operations and select ON, make sure the clay pump stabilizes and does not constantly stay at 100 RPM. The clay pump must be set on EXT and going clockwise. Also, make sure that the ”1 rpm pump” and ”on off switch” are both OFF. See ProCoDA section below on how to turn those off.
5. Wait until the the influent turbidimeter stabilizes to 100 NTU.
6. Start experiment (be sure to start recording data).

### Cleaning Procedure
1. Clean turbidimeters by removing the top, detaching the glass vial, emptying to the sink, then refilling with water.

2. Clean flocculator and sedimentation tank by attaching the long cleaning tube to the push to connect at the start of the flocculator and the sink. Then detach the tube at the bottom of the sedimentation tank and attach it to the top of the tank. Then turn the sink on slowly and run for 30 seconds.

3. Rinse coagulent reservoir with DI water.

## ProCoDA Method File

The following is taken directly from the Calibrating PID Control on the AguaClara Confluence website:

To establish constants for PID control in ProCoDA, follow the procedure shown at this link. The steps will be summarized below

1. After you have loaded the proper PID control function and have created the appropriate set points in your method file, set the P, I, and D set points to zero.
2. Set P to a small value and change the target value to provoke a response from the PID control
3. Observe the graph of the variable being controlled for this value of P. If the result is an oscillation that becomes damped (decreasing amplitude), increase the value of P incrementally and repeat the process. If the result is an oscillation that becomes amplified (increasing amplitude), lower the value of P and repeat the process.
4. The objective is to find a value of P for which there is a periodic oscillation of the value with a constant amplitude. Once the correct P value (Ku) has been found, write it down and also record the period of the wave (time between two consecutive crests of the oscillation - Pu - in minutes).
5. AguaClara researchers typically use PI control (the value of D is set to zero). To find the value of P required, use the equation: P = Ku/2.2. To find the value of I required, use the equation: I = Pu/1.2. This should result in a value in minutes, which is the correct unit for I.
6. Change your set points (P and I) to the new values. Ensure that there is less than 10 percent variation in your variable, and fine tune if necessary.

This calibration method may result in oscillatory behavior. To reduce variability in the output, consider reducing P to damp the oscillations. This will reduce the responsiveness of the algorithm and will increase the stability.

### States
In order to properly begin an experiment, the ProCoDA method file must be turned ON. When an experiments in not in progress, ProCoDA is turned off.
* ON - The active state of ProCoDa. The 1 rpm pump drain is turned on (for draining the floc hopper) and the the clay pump is control (with PID) is turned on.

* OFF – Resting state of ProCoDA. All sensors, relays, and pumps are turned off.


<img src="https://writelatex.s3.amazonaws.com/xwbtgtsrxrxy/uploads/3515/18132096/1.PNG?X-Amz-Expires=14400&X-Amz-Date=20180309T225843Z&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJF667VKUK4OW3LCA/20180309/us-east-1/s3/aws4_request&X-Amz-SignedHeaders=host&X-Amz-Signature=7ec40a369ef8347b616cae821821b3aff120b22142e29f88638e8be500e4323c" width=600>

Figure 6: The ON state of the HRS ProCoDA method file. The floc hopper drain and clay pump are the active items controlled by the pump.

### Set Points
Here, you should list the set points used in your method file and explain their use as well as how each was calculated.

The following is a list of all the Set Points in the method file and their values. Exact location of these points in the method file can be seen in the figure below.

<img src="https://writelatex.s3.amazonaws.com/xwbtgtsrxrxy/uploads/3545/18132331/1.PNG?X-Amz-Expires=14400&X-Amz-Date=20180309T230328Z&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJF667VKUK4OW3LCA/20180309/us-east-1/s3/aws4_request&X-Amz-SignedHeaders=host&X-Amz-Signature=9d1a8a9cc2766757b559bc7d44d31b6dd45cf967c318af45f3e689752c21dca3" width=600>

Figure 7: This is the overall order of the Set Points for the HRS method file.


* OFF - no units, value of 0, constant
* ON - no units, value of 1, constant
* Turb Target - NTU, value of 100, constant. Value determined as the influent turbidity desired by the pump control
* P - no units, value of 300m, constant. Value determined through method mentioned in "PID Control" section of report and trial and error.
* i - no units, value of 2.3, constant. Value determined through method mentioned in "PID Control" section of report and trial and error.
* D - no units, value of 0, constant

<img src="https://writelatex.s3.amazonaws.com/xwbtgtsrxrxy/uploads/3556/18132401/1.PNG?X-Amz-Expires=14400&X-Amz-Date=20180309T230958Z&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJF667VKUK4OW3LCA/20180309/us-east-1/s3/aws4_request&X-Amz-SignedHeaders=host&X-Amz-Signature=4cfffd6c222b0f17284243c2296dd53dcb2481edeeaf5be55aa0a41480c89752" width=600>

Figure 8: This is the output settings for the PID state. This process runs in the background and only needs to be set up at the beginning of a semester's work. Note that PID controls the clay pump and whether it is turned on or not at any given time.

* Influent Turbidimeter ID - no units, value of 1, constant. Value is due to the step in which the turbidimeter is installed and acknowledged in the data recording process. Effluent Turbidimeter ID is 2 since it takes in data later down the line.
* Influent Turbidity - no units, value of 0, variable. See Figure below

<img src="https://writelatex.s3.amazonaws.com/xwbtgtsrxrxy/uploads/3547/18132348/1.PNG?X-Amz-Expires=14400&X-Amz-Date=20180309T232849Z&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJF667VKUK4OW3LCA/20180309/us-east-1/s3/aws4_request&X-Amz-SignedHeaders=host&X-Amz-Signature=1873f77fbba467a6a7c77a1e4acba3fff7fffafc39e2cd6b35fe9acc6a0a5a59" width=600>

Figure 9: This displays the influent turbidity Set Point and the selected sensors to establish the relationship.

* Effluent Turbidimeter ID - no units, value of 1, constant.
* Effluent Turbidity - no units, value of 2
* PumpControl(Clay) - no units, value of 0, variable

<img src="https://writelatex.s3.amazonaws.com/xwbtgtsrxrxy/uploads/3548/18132354/1.PNG?X-Amz-Expires=14400&X-Amz-Date=20180309T232816Z&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJF667VKUK4OW3LCA/20180309/us-east-1/s3/aws4_request&X-Amz-SignedHeaders=host&X-Amz-Signature=d89273cfa2a007e1fef18612d5f9374d5421eea175a51b38212c6593a4a19afa" width=600>

Figure 10: This shows the relationship between the PumpControl(Clay) variable and other predefined set points.

## Python Code
### Variables

$C_{sys}$: Concentration of coagulent in system

$C_{labstock}$: Concentration of coagulent in lab stock

$Q_{sys}$: Flowrate of system

$K_{dilution}$: Dilution factor in reservoir

$V_{reservoir}$: Volume of reservoir

$Frac_{resivor}$: Fraction of usable reservoir

$Q_{per rpm}$: Flow rate per pump rpm

$M_{flowcoag}$: Mass flowrate of coagulent  

$C_{reservoir}$: Concentration of coagulent in reservoir

$Q_{reservoir}$: Flow rate out of reservoir

$RPM$: number of pump RPMs for desired flowrate

$RunTime$: Amount of time the experiment can run without refilling the coagulent reservoir

### Python Code

```python
from aide_design.play import*

#inputs
C_sys = 1.4*(u.mg/u.L)
C_labstock = 70.9*(u.g/u.L)
Q_sys = 1.48*(u.mL/u.s)
K_dilution = .8*(u.mL/u.L)
V_reservoir = 5*(u.L)
Frac_reservoir = .76
Q_per_rpm = .001828 *(u.mL/u.s)

#Calculations
M_flow_coag = (Q_sys * C_sys).to(u.mg/u.s)
C_reservoir = (C_labstock * K_dilution).to(u.gram/u.L)
Q_reservoir = (M_flow_coag / C_reservoir).to(u.mL/u.s)

#Outputs
RPM = Q_reservoir / Q_per_rpm
RunTime = ((V_reservoir * Frac_reservoir) / Q_reservoir).to(u.hour)

print('The RPM needed for this coagulent dosage is' ,RPM)

print('The run time is ', RunTime)
```

```python
# To convert the document from markdown to pdf
pandoc Name_of_this_file.md -o TeamName_Research_Report.pdf
```
