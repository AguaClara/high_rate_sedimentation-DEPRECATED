# High Rate Sedimentation, Spring 2018
#### Mike Zarecor, Sneha Sharma, Justin Conneely
#### March 9th, 2018

## Abstract
Past High Rate Sedimentation teams have hypothesized that floc blankets thin as experiments progress due to coagulant sticking to the walls of the flocculator, reducing the overall coagulant dosage. The 2018 spring team has conducted an experiment to test if increasing the coagulant dosage solves this problem and leads to stable floc blankets. The results show that ...

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
Swetland (2014) Found that as flocs formed, they would sediment due to their higher density compared to water. The flocs must settle faster than the upflow velocity. As the flocs concentrated and fell down to the bottom of the tank, a floc blanket formed.

These findings defined the High Rate Sedimentation teams's understanding of a floc blanket. This contributed directly to many of the past designs the team has used, and spurred interest in the effects of having a floc blanket.

Hurst (2010) stated that the presence of the floc blanket would enhance the removal of turbidity causing particles. These experiments found that upflow velocities of 1.0 to 1.3 m/s produced the best performance. Past teams have tried to  

Balwan (2016), a researcher from the International Journal of Innovative
Research in Advanced Engineering (IJIRAE), explored the effect of the length
of tube settler on effluent turbidity. As indicated in his report, increasing the
length of tube settlers increased the percentage of turbidity removed (defined as
percentage change between influent and effluent turbidity). With tube settlers in
45 degrees inclination angle and 60 cm length, turbidity removal was measured
to be 80 percent. However, his experiments only had three length variables
(40cm, 50cm, 60cm) and the effluent of longer tube settlers were unknown.

Culp et al. (1968) used tubes to figure out the optimal slope of the tube
settlers. Under laboratory conditions, a 60 degree angle with respect to the
horizontal provided continuous sludge removal while showing effective sedimentation
performance.


## Methods
### Experimental Apparatus
The overall lab bench set up of the HRS team is composed of several parts (Figure 10). They are the pumps, the stocks, the flocculator, and the turbidimeters.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Lab%20Bench%20Setup.png" height250 width=400>

Figure 10: The HRS lab bench setup is composed of the turbidimeters, stocks, pumps, and flocculator.

This allows the team to simulate non-potable water and its treatment through high rate sedimentation while keeping track of performance via NTU. The influent and effluent turbidimeters are what tell the team how well the system is performing at any given time. In order to run experiments, tap water is contaminated with clay from the Clay stock. This contaminated water is known as the influent and is kept at a constant NTU of 100 through ProCoDA by utilizing PID control. For more on Clay dosing, see Manual.

Once the influent passes through the turbidimeter, it moves toward the flocculator. Upon entering the flocculator, the untreated water is dosed with Poly-Aluminum-Chloride (PAC), which is the coagulant Aguaclara utilizes. The Coagulant pump is manually set up to control how much of the Coagulant stock enters the system. When a dose is chosen (generally between .5-3.2 mg/L PAC), the team uses a MathCAD doc to determine the stock concentration and required RPM of the pump. For more on Coagulant dosing, see Manual. The treated water then passes through the coiled tube that is the flocculator, forming flocs. The end of the flocculator then enters the bottom of the recirculator where upflow begins. The effluent that exits through the top of the tube settler then flows through the effluent turbidimeter. This is where the turbidity of the effluent is determined; the goal is to reach an NTU of 0.3 or lower. After the effluent turbidimeter, the wastewater flows out towards the wastewater drainage.

This Fall semester, all particle removal teams are utilizing the HRS standard apparatus design and a flocculator designed by the High G Flocculation Fall 2017 team. The flocculator’s purpose is to mimic the flocculation process in an actual AguaClara plant with a sufficient collision potential (G). The High G flocculation team provides information on the following table with the flocculator’s dimensions and the resulting values for an upflow velocity of 3 mm/s.

| V.Sed | Sed Tank Upflow Velocity | 3 mm/s |
| ----- | ------------------------ | ----- |
| D.Sed | Sed Tank Inner Diameter  | 1 in  |
|Q.Sed, Q.Reactor| Flow rate (from V.Sed) |1.52 mL/s|
|D.Floctube|Floctube Inner Diameter| 0.17 in |
|R.c|Radius of Curvature of Floc Coils|5 gm|
| Gtheta | G*theta | 20,000 |
|  G  |  Shear   |  175.5 Hz  |
|Theta |Residence Time | 1.899 min or 113.9 s|
| L.Flocc| Length of Flocculator Tubing|11.821 m|
|Epsilon.Flocc |Energy Dissipation Rate| 30.814 mW/kg|

Figure 11: The HRS lab bench setup consists of a flocculator developed by the High G Flocculation Fall 2017 team. The following are the parameters and resulting values of the current flocculator design.

### Procedure
Discuss your experimental procedure. How did you run your experiment? What were you testing? What were the values of relevant parameters?

## Results and Analysis
Present an observation (results), then explain what happened (analysis).  Each paragraph should focus on one aspect of your results. In that same paragraph, you should interpret that result.  
In other words, there should not be two distinct paragraphs, but instead one paragraph containing one result and the interpretation and analysis of this result. Here are some guiding questions for results and analysis:

When describing your results, present your data, using the guidelines below:
* What happened? What did you find?
* Show your experimental data in a professional way.
```python
from aide_design.play import*
x = np.array([1,2,3,4,5])
y = np.array([1,2,3,4,5])
plt.figure('ax',(10,8))
plt.plot(x,y,'*')
plt.savefig('/Users/jillianwhiting/github/Jillian-Whiting/Images/linear')
plt.show()
```
![linear](https://github.com/jillianwhiting/Jillian-Whiting/blob/master/Images/linear.png?raw=true)
Figure 1: Captions are very important for figures. Captions go below figures.

After describing a particular result, within a paragraph, go on to connect your work to fundamental physics/chemistry/statics/fluid mechanics, or whatever field is appropriate. Analyze your results and compare with theoretical expectations; or, if you have not yet done the experiments, describe your expectations based on established knowledge. Include implications of your results. How will your results influence the design of AguaClara plants? If possible provide clear recommendations for design changes that should be adopted. Show your experimental data in a professional way using the following guidelines:
* Why did you get those results/data?
* Did these results line up with expectations?
* What went wrong?
* If the data do not support your hypothesis, is there another hypothesis that describes your new data?

## Conclusions
Explain what you have learned and how that influences your next steps. Why does what you discovered matter to AguaClara?

Make sure that you defend your conclusions with facts and results.

## Future Work
Describe your plan of action for the next several weeks of research. Detail the next steps for this team. How can AguaClara use what you discovered for future projects? Your suggestions for challenges for future teams are most welcome. Should research in this area continue?

## Bibliography
Logan, B. E., Hermanowicz, S. W., & Parker,A. S. (1987). A Fundamental Model for Trickling Filter Process Design. Journal (Water Pollution Control Federation), 59(12), 1029–1042.

# Manual
The goal of this section is to provide all of the guidance that would be necessary for a future team to pick up your work where you left off. Please try to be thorough and put yourselves in the shoes of a newcomer to the project. Below are some recommended sections, but the manual will likely take a slightly different form for each team.

## Fabrication Details
Include any information related to the fabrication of equipment, experimental apparatuses, or technologies. Include the purpose of each step and the fabrication methods used. Reference appropriate safety precautions.

## Special Components
If your subteam uses a particular part that is unique and you could foresee a future subteam needing to order it or learn more about it, please include basic information like the vendor where it was purchased, catalog/item number, and a link to any documentation.

## Experimental Methods
### Set-up
Step 1.
* Put tasks in a sequential order.
* It is okay to have sub-lists.
  - Like this.

### Experiment
Step 1.

### Cleaning Procedure
Step 1.

## Experimental Checklist
Another potential section could include a list of things that you need to check before running an experiment.

## ProCoDA Method File
Use this section to explain your method file. This could be broken up into several components as shown below:

### States
Here, you should describe the function of each state in your method file, both in terms of its overall purpose and also in terms of the details that make it distinct from other states. For example:
\begin{itemize}
\item \underline{OFF} - Resting state of ProCoDA. All sensors, relays, and pumps are turned off.
\end{itemize}

### Set Points
Here, you should list the set points used in your method file and explain their use as well as how each was calculated.

## Python Code

### Variables
$g$: gravity
$\sigma$: dispersion
$a$: amplitude
$h$: water depth
$H$: distance from wave crest to trough (2$a$)
$T$: wave period
$\lambda$: wavelength
$k$: wavenumber
$c_p$: celerity (wave phase speed)
$P$: pressure
$F$: force
$u$, $w$: x-velocity, z-velocity components

```python
# Comment
```

# Add/Delete/Change this Template as you see Fit
When using this template keep in mind that this serves three purposes. The first is to provide your team feedback on your progress, assumptions, and conclusions. The second is to keep your team focused on what you are learning and doing for AguaClara. Another is to educate future teams on what you've learned and done. This document should be comprehensive, consistent, and well-written. With that in mind, add, subtract, or move sections. Reach out to the RAs and graders for help with figuring out what should or shouldn't include. Focus on how wonderful a reference you are making through this and work hard on communicating amongst yourselves and with future teammates. (Delete this section before submitting)

```python
# To convert the document from markdown to pdf
pandoc Name_of_this_file.md -o TeamName_Research_Report.pdf
```
