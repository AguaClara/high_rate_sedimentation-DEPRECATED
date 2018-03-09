# AguaClara Research Report & Manual Template
#### Natalie Mottl, William Pennock, Janak Shah, and Jillian Whiting
#### February 20, 2018

# Template Description
This template will lay out all possible sections that could be used for a research report and manual. All research reports and manuals should strive to comply with this template, but every team will use different parts. In order to use this template, copy this file from the AguaClara team resources repository to your team's repository, and rename it for your team in a format similar to  "[Team Name] [Semester]". An example would be "Filter and Treatment Train Flow Control Spring 2017." For additional information on all the possibilities in markdown files, refer to the AguaClara Interactive Tutorial and the AguaClara Tutorial training pages. After you complete that step, please delete this description and everything above this.

# High Rate Sedimentation, Spring 2018
#### Mike Zarecor, Sneha Sharma, Justin Conneely
#### March 9th, 2018

## Abstract
Briefly summarize your previous work, goals and objectives, what you have accomplished, and future work. (100 words max)

## Introduction
Explain how the completion of your challenge will affect AguaClara and the mission of providing safe drinking water (or sustainable wastewater treatment!). If this is a continuing team, how will your contribution build upon previous research? What needs to be further discovered or defined? If this is a new team, what prompted the inclusion of this team?

## Literature Review and Previous Work
Discuss what is already known about your research area based on both external work and that of past AguaClara Teams. Connect your objectives with what is already known and explain what additional contribution you intend to make. Make sure to add APA formatted in-text citations. If you mention the author(s) in your sentence, you can simply give the year of publication.[(Logan et. al. 1987)](http://www.jstor.org/stable/pdf/25043431.pdf?acceptTC=true)


## Methods
### Experimental Apparatus
The overall lab bench set up of the HRS team is composed of several parts (Figure 10). These parts include the pumps, the stocks, the flocculator, and the turbidimeters.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Lab%20Bench%20Setup.png" height250 width=400>

Figure 10: The HRS lab bench setup is composed of the turbidimeters, stocks, pumps, and a flocculator.

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

Figure 11: The HRS lab bench setup consists of a flocculator developed by the High G Flocculation Fall 2017 team. The above are the parameters and resulting values of the current flocculator design.

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

Figure 12: A diagram of the active tube settler length L, the inner diameter of the apparatus S, and the angle α.

Materials: In the Fall 2017 model, the floc weir is welded onto the tube settler rather than the
recirculator and the apparatus is enclosed by compression fittings. The reason for an intermittent floc weir on the tube settler is due to the findings of the Summer 2017 team. If a floc blanket could
be established with a low bend, then further investigation is required on whether multiple bends
characteristic of the trapezoidal apparatus are necessary for performance, or just keep essential
flocs low and recirculating.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Screen%20Shot%202018-03-08%20at%2011.53.16%20PM.png" height250 width=400>

Figure 13: The HRS Fall 2017 team compiled the
materials necessary for all particle team apparatuses.
This includes compression fitting, push-to-connects,
PVC tubing, tubing, and valves for floc hopper
drainage.

<img src="https://raw.githubusercontent.com/JustinConneely/Personal/master/Images/Screen%20Shot%202018-03-08%20at%2011.53.29%20PM.png" height250 width=400>

Figure 14: The standard design includes a 50 cm recirculation zone, a 36.47 cm tube settler, an a 40 cm long floc weir. The inner diameter of the PVC tubing is 1 inch rather than 3/4 inches like previous
semesters.

Compared to previous semesters, the size of the apparatus has been reduced a considerable amount.
It is important to note that the team’s goal is not necessarily to reduce turbidity more than what
the trapezoidal was able to achieve, but rather to investigate possible alternatives to sedimentation
tank design in order to avoid the complex geometry that the trapezoidal design implicates.

Construction Process: The team obtains 5 PVC tubes with 1 in inner diameter and a 60<sup>o</sup> bend
from the horizontal. From there, the team implements the following:

1. Cut the tubes to the necessary length (50 cm recirculator and 36.47 cm tube settler)
2. Cut floc weirs from 1/2 inch tubing
3. Weld weir to tube settler
4. Layer of glue as a failsafe sealant
5. Install fittings on all the apparatus.

Since the tubing size increased from 3/4 inch to 1 inch, the flow rate of influent water had to be
altered in order to achieve the 3 mm/s upflow velocity that is unique to high rate sedimentation. The following equation is used in order to help the team determine these values:

$$ V_{floc} = \frac{Q_{floc}}{\frac{D^2_{pipe}}{4} ∗ π} ... (4) $$

Where Q<sub>floc</sub> is the volumetric flow of water through the system and D<sub>pipe</sub> is the inner diameter of the PVC pipe.

### Procedure
Using the aforementioned set-up, the HRS team tests the effect of increasing coagulant dose on floc blanket degradation and effluent turbidity. This is tested by first flushing the system to assure it was clean of coagulant and clay particles, then setting the influent turbidity to 100 NTU. Then the team tests varying doses of coagulant with a constant upflow velocity in the sedimentation tank of 3 mm/s (experimentally extrapolated from an RPM of 28.3). The first experiment is conducted at a coagulant dosage of 1.4 mg/L and a corresponding coagulant pump RMP of 20. That initial coagulant dose was then increased incrementally, then tested under the same conditions as above.

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
