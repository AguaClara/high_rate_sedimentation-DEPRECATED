#  High Rate Sedimentation, Summer 2018
#### Anna Hong and Hannah Si
#### July 27, 2018

## Abstract
Sedimentation is a critical process for water treatment plants by which coagulated minerals, dirt, and other particles are removed from the water via gravitational settling. The High Rate Sedimentation (HRS) team works to design a sedimentation tank that will yield an effluent with turbidity of 0.3 NTU or lower at a high upflow velocity. While 1 NTU is the World Health Organization's standard for turbidity drinking water, the EPA standard is 0.3 NTU. AguaClara currently achieves this with an upflow velocity of 1 mm/s, but not at upflow velocities of 3 mm/s or greater. Therefore, the goal of HRS team is to preserve system success while raising upflow velocity in order to provide more clean water in a given time without increasing treatment plant size. Operating at a greater efficiency would eliminate the need for additional building materials and higher construction and maintenance costs.

Since the fall of 2017, the AguaClara High Rate Sedimentation (HRS) team has been investigating the cause behind floc blanket decay, which has been attributed to system failure, at high upflow velocities in the sedimentation tank. The Summer 2018 HRS team first conducted experiments at lower upflow velocities of 1 mm/s and 2 mm/s in a 1" diameter tube to replicate system success. However, after failing to produce a floc blanket at these lower upflow velocities yet succeeding at higher velocities, the Summer 2018 HRS team has focused on optimizing sedimentation at a higher upflow velocity of 3 mm/s. The team confirmed the optimal coagulant dosage to be approximately 4.5 mg/L of PACl and is currently redesigning the sedimentation tank's bottom geometry to enhance resuspension of flocs.

## Methods
### Experimental Apparatus
Below is a picture of the revised lab bench setup of the HRS team followed by a table listing the various components.

**Ian's Comment:** Whenever you refer to a picture or table in the text, refer to it by its number (eg "Figure 1 below shows...")

<p align=center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/updatedlabbenchsetup.JPG" width = 500>
  <br></br>
  Figure 1. Labeled experimental setup for the High Rate Sedimentation lab bench
</p>

| Label | Component             | Label | Component             |
|:-----:|:--------------------- |:-----:|:--------------------- |
|   1   | Water Pump            |   8   | Effluent Turbidimeter |
|   2   | Clay Pump             |   9   | Pressure Attenuator   |
|   3   | Coagulant Pump        |  10   | Coagulant Stock       |
|   4   | Waste Pump            |  11   | Clay Stock            |
|   5   | Flocculator           |  12   | Sedimentation Tank    |
|   6   | Pressure Sensor       |  13   | Waste Tube            |
|   7   | Influent Turbidimeter |       |                       |


### Setup Procedures
#### Original Configuration

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Org%20Config.png" width = 500>
</p>


1. Drain the sedimentation tank.
   a. Close the valves that would allow backflow into the sedimentation tank’s effluent tube. Disconnect that tube.
   b. Close the valve between the flocculator and sed tank.
   c. Open the valve that drains the sed tank from the bottom.
   d. Disconnect the tube attached to the floc weir and catch the draining fluid in a waste bucket or tub.
   e. Reconnect the tube to the floc weir. Turn on the waste pump to drain the floc weir throughout the rest of the setup.
     * The waste pump should be controlled by ProCoDA, so turning it on may require turning on ProCoDA and then manually disabling other pumps.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/DrainSedTank.png" width = 500>
</p>

2. Clean the flocculator and sedimentation tank.
   a. Close values leading to the flocculator.
   b. Take the disconnected effluent tube (see step 1) and connect it to end of the flocculator.
   c. Connect one end of a long cleaning tube to the system just before the **coagulant entry point**.
   d. Connect the other end of the cleaning tube to the sink and turn on the faucet slowly. Make sure that the water is not rising more than a couple inches from the bottom of the sed tank. Continue for 30 seconds.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/CleanFloc.png" width = 500>
</p>

3. Clean out the flocculator in the reverse direction.
   a. Just before the coagulant entry point, swap the cleaning tube for another tube long enough to reach a waste bucket or tub. This can be a new tube or, as shown in the diagram, the waste tube that drains the sedimentation tank.
   b. Connect the cleaning tube to the end of the flocculator.
   c. Turn on the sink faucet and gradually accelerate the water speed. This can reach a higher speed than in Step 2, though not high enough for the faucet to  start spraying water.
   d. Turn off the faucet and redo all connections that were modified in Steps 1-3.

<p align = center>
  <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/ReverseFloc.png" width = 500>
  </p>

4. Clean out the pressure attenuator if there seems to be clay inside.
   a. Close valves on either side of the pressure attenuator.
   b. If there is water inside the pressure attenuator bottle, turn it upside down (so water does not spill out) and remove the tubes connected to the inlets and outlets.
   c. Pour out the contents and rinse the bottle.
   d. Add enough water to cover the inlet and outlet holes, screw the cap on, turn the bottle upside down again, and insert the tubes back into the inlets and outlets.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/PressureAtt.png" width = 500>
</p>

5. Disconnect the coagulant tube from system, turn on the pump, and check that coagulant is running through. If it is, reconnect the tube to the system.
   * Make sure the coagulant valve is open. There should be steady drops of solution.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/CoagStock.png" width = 500>
</p>

6. Run water through the system while bypassing the pressure attenuator.
   * While waiting for one of the longer steps of the setup to complete (such as this step), start making the coagulant and clay stocks.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/CleanSystem.png" width = 500>
</p>

7. After the water reaches the top of the sed tank, shut off the water pump and drain the sedimentation tank again.
   * Repeat steps 5 and 6 about two to three more times to achieve a more thorough cleaning of the sed tank.
<br></br>

8. Run water only through the system _with_ the pressure attenuator included until effluent turbidity stabilizes near 0 NTU (ideally below 1.0 NTU). It is natural for influent and effluent turbidity to rise at first in this step.
   *  Troubleshooting Pressure Buildup
      * If the water level is rising steadily in the pressure attenuator (and it was already above the outlet), there is still pressure buildup in the system, most likely due to a closed valve or air in the tubing.
      * If there may be air, redirect flow to waste instead of the flocculator (after the influent turbidimeter) until the pressure stabilizes.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Effluent0NTU.png" width = 500>
</p>

9. Clean out the influent and effluent turbidimeters. Refer to the [AguaClara Tutorial Wiki Page](https://github.com/AguaClara/aguaclara_tutorial/wiki) for more details on how to do this.
<!--need to update this link!-->

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Cleanturbidimeters.png" width = 500>
</p>

10. Direct the flow to waste instead of the flocculator as shown in the diagram below.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Stabilizeinfluent.png" width = 500>
</p>

11. Turn on the clay stirrer, make sure that the ProCoDA state is ON, and then start the clay pump.
    * Note: While on internal control mode (INT), the clay pump must be controlled manually. While on external control mode (EXT), it must be controlled programmatically.
    * If ProCoDA should be, but is not controlling the clay pump, press the INT/EXT button on the pump to toggle its control mode to internal, start the pump, and then toggle back to external control mode.
<br></br>

12. Allow stabilize influent turbidity to 100 NTU. With the appropriate clay stock concentration and PID constants, this will take several minutes.
<br></br>

13. Redirect the flow back to the flocculator and main system. Turn on the coagulant pump to start the experiment.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Runexperiment.png" width = 500>
</p>

### Experiments and Results

**Ian's Comment:** Include a link somewhere in this section to where your data is stored on Github so someone can look at it if they want.  Also either label the data files with what experiment they correspond to, or include that in the description of each experiment.

The HRS team has been experimenting with two sedimentation tank designs in an effort to understand the reasons for floc blanket decay in the Spring 2018 and Fall 2017 semesters.

1. **Sedimentation Tank A** is the sedimentation tank design used by most AguaClara particle removal research teams, including the HRS team in the Fall 2017 semester. The tube settler is relatively short and the floc weir is placed on the left side of the tube settler (when the tube settler points to the left).

<p align="center">
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Sedimentation%20Tank%20A.png" width=300>
</p>

Figure 2. Sedimentation Tank A, the sedimentation tank used by most AguaClara research teams, including the Fall 2017 HRS team.

2. **Sedimentation Tank B** is the sedimentation tank design used by the Spring 2018 HRS team. The tube settler is relatively long and the floc weir is placed on the right side of the bend in the recirculator (when the tube settler points to the left).

<p align="center">
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/SedTankB.png" width=300>
</p>
Figure 3. Sedimentation Tank B, the sedimentation tank used by the Spring 2018 HRS research subteam.

#### Summary of Experiments

|Experiment |Upflow Velocity (mm/s) |Tank Type| Coagulant Dosage (mg/L)|Floc <br/> Blanket Formed| Ending Effluent Turbidity|Insights|
|:---:|:---------------:|:----:| :-------: |:-----:|:---|:---|
|[1](#experiment-1)|3|A|1.4|Yes| ≤ 2 NTU|
|[2](#experiment-2)|3|B|1.4|Yes| 4.4 NTU &rarr; 19.5 NTU
|[3](#experiment-3)|1|B|4.2 &rarr; 1.4 |No|135 NTU| Failure may be due to initial excess coagulant.
|[4](#experiment-4)|1|B|1.4|No|20 NTU|New hypothesis: 1 mm/s upflow velocity is too slow.
|[5](#experiment-5)|3|A|1.4|Yes|26 NTU
|[6](#experiment-6)|1 &rarr; 2| A |1.4|No|46 NTU| 2 mm/s upflow velocity may also be too slow.|

Note: All subsequent experiments were run using Tank A. See section [Sedimentation Tank A vs. B](#sedimentation-tank-a-vs-b).

|Experiment|Upflow Velocity (mm/s)|Coagulant Dosage (mg/L)|Floc Blanket Formed|Ending Effluent Turbidity|Insights|
|:---:|:---:|:--------:|:---|:------|:---|
|[7](#experiment-7)|2|1.4|No|37-40 NTU|
|[8](#experiment-8)|2|2.8 &rarr; 4.2|No|33-35 NTU|
|[9](#experiment-9)|2|4.2|No|35-40 NTU|
|[10](#experiment-10)|3|1.5|Yes|15 NTU|
|[11](#experiment-11)|3|3.0|Yes|16 NTU|Faster floc blanket formation|
|[12](#experiment-12)|3|4.5|Yes|2-3 NTU &rarr; 11-12 NTU|Even faster floc blanket formation|
|[13](#experiment-13)|4|4.5|Yes|27-28 NTU|Gelling observed in flocculator and sedimentation tank|
|[14](#experiment-14)|4|4.5 <br/> with higher pump speed|Yes|~30 NTU|Gelling still observed; 4 mm/s may be too high|
|[15](#experiment-15)|3|4.5|Yes|27 NTU (at 1 hr)| With inserted, flat surfaced sedimentation tank bottom to observe floc buildup|
|[16](#experiment-16)|3|4.5|Yes|22 NTU|With conical sedimentation tank bottom, flocs are still building up|

#### Experiment 1

**Description**: The purpose of the first two experiments was to record initial observations of floc blanket behavior using both sedimentation tank designs. For Experiment 1, the HRS apparatus was run at an upflow velocity of 3 mm/s for 9.5 hours using Tank A in order to confirm that this higher rate would lead to floc blanket decay and system failure.

**Results**: At about 2.5 hours into the experiment, an opaque floc blanket formed in the recirculator. By the end of this shorter experiment, the effluent turbidity did not rise above 2.0 NTU, making this a success -- contrary to the Fall 2017 and Spring 2018 teams' results. Whether this success was due to the floc weir being in an optimal position or a more robust system will need to be further investigated.
[Return to Summary of Experiments](#summary-of-experiments)

**Ian's Comment:** Do you have data from this experiment?  If so include it

#### Experiment 2

**Description**: Experiment 2 ran a test with an upflow velocity of 3 mm/s using Tank B for a longer time (22.5 hours). This test was intended to confirm whether the sedimentation tank design plays a factor in floc blanket decay and thus system failure.

**Results**: At the same time at which Experiment 1 ended (9.5 hours), the effluent turbidity reached 4.4 NTU. Movement of flocs at this time was slower than that observed in Tank A and the floc blanket was not opaque, but became less dense toward the bottom of the sedimentation tank. By the end of 22.5 hours, the effluent turbidity of 19.5 NTU. While the turbidity level signals system failure, it decayed at a significantly slower rate than for the Spring 2018 HRS team.

<p align="center">
  <a href="https://www.youtube.com/watch?v=JcQjRKY91NI&feature=youtu.be"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Exp2pic.PNG" width=200> </a>
</p>

Figure 4. Click the image or [this link](https://www.youtube.com/watch?v=dMs-pc6IACs&feature=youtu.be) for a video of the sedimentation tank during Experiment 2.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/6-14-2018.png">
</p>

Figure 5. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity using Tank B

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 3
**Description**: The next two experiments were run at a slower upflow velocity with Tank B in order to simulate successful particle removal in AguaClara treatment plants. This experiment tested a 1 mm/s upflow velocity. For the first 30 minutes, there was an input of excess coagulant because the coagulant pump speed was not reduced from 20 RPM to 6.7 RPM to accommodate this lower upflow velocity.

**Results**: The initial effluent turbidity began at 4.6 NTU and rapidly increased throughout experiment. By the end of 20 hours, the effluent turbidity spiked higher than the influent turbidity -- 135 NTU compared to 100 NTU -- making this a failure. It was hypothesized that the excess coagulant at the beginning of the experiment stuck to the walls of the tubing, creating higher shear and decreased diameter. Coagulant particles may have collided with other coagulant particles instead of clay particles, leading to smaller flocs that are more difficult to capture in the tube settler.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/6-25-2018.png">
</p>

Figure 6. Effluent turbidity vs. Time with a 1 mm/s Upflow Velocity using Tank B with Initial Excess Coagulant

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 4

**Description**: To nullify any potential effects from the initial coagulant dosage spike in Experiment 3, this experiment ran at 1 mm/s with the appropriate coagulant pump speed of 6.7 RPM for 8 hours.

**Results**: With a final effluent turbidity of 20 NTU, the system still failed, disproving that initial excess coagulant was the main problem. There was no observable formation of a floc blanket, and smaller flocs in the sedimentation tank were not being captured and settled out. One key observation was that the size and amount of flocs emerging in the sedimentation tank appeared to be less than that at the end of the flocculator. The large flocs may have been accumulating in the bottom of the sedimentation tank, which is covered by white PVC connections. Therefore, it is hypothesized that the upflow velocity of 1 mm/s is too slow for floc resuspension in the sedimentation tank that leads to healthy floc blanket formation.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/6-26-2018.png">
</p>

Figure 7. Effluent turbidity vs. Time with a 1 mm/s Upflow Velocity using Tank B with No Initial Excess Coagulant

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 5

**Description**: To ensure that no modifications to our experimental apparatus were the cause of system failure, Experiment 1 (3 mm/s upflow velocity with Tank A) was rerun but for a longer period of 18 hours.

**Results**: As before, an opaque floc blanket formed with the same density gradient of flocs in the recirculator (higher density toward the top). However, this experiment ended with a slowly rising effluent turbidity of 26 NTU at 18 hours. There were many flocs settled high in the tube settler. It seems that the floc blanket formed later than it did in Experiment 1, allowing small flocs to escape in the beginning of the experiment. This significantly higher effluent turbidity suggests that something has changed since Experiment 1, but whether the design of the system was the change has yet to be determined.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/6-27-2018.png">
</p>
Figure 8. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity using Tank A for Longer Period of Time (18 hours)

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 6

**Description**: This experiment tested whether a lower upflow velocity of 1 mm/s could also be successful with Tank A. After about 2 hours, there were still no signs of floc blanket formation. Since other AguaClara subteams experienced system success at a 2 mm/s upflow velocity, the water and coagulant pump speeds were doubled at this time to attain this higher velocity to test whether a 1 mm/s upflow velocity is indeed too slow (as hypothesized after Experiment 4).

**Results**: This experiment ended with a failing effluent turbidity of 46 NTU. No floc blanket formed during the experiment even with the increased flow rates. It seems that floc blanket formation requires an upflow velocity of approximately 3 mm/s or higher.

<p align = center>
  <img src="Images/Graphs/6-28-2018.png">
</p>

Figure 9. Effluent turbidity vs. Time with a 1 -> 2 mm/s Upflow Velocity using Tank A

[Return to Summary of Experiments](#summary-of-experiments)

#### Sedimentation Tank A vs. B
Since the design of the sedimentation tank did not seem to be the deciding factor between system success and failure, the subsequent experiments were conducted using the standard design Tank A, as it is the configuration used by other AguaClara subteams.

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 7
**Description**: The following three experiments ran at upflow velocities of 2 mm/s in order to confirm whether 2 mm/s is indeed too slow to achieve system success. Experiment 7 ran at 2 mm/s with a coagulant system concentration of 1.4 mg/L.

**Results**: Ending with an effluent turbidity of 37-40 NTU, this experiment observed system failure. No floc blanket formed throughout the duration of the experiment, which was around 7 hours. Whether this failure was a result of insufficient levels of coagulant in the system or due to too low of an upflow velocity has yet to be determined.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-9-2018.png">
</p>
Figure 10. Effluent turbidity vs. Time with a 2 mm/s Upflow Velocity at 1.4 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 8
**Description**: Experiment 8 ran at 2 mm/s using Tank A with a coagulant system concentration of 2.8 mg/L, which was increased to 4.2 mg/L after 1 hour into the experiment.  

**Results**: Since this experiment seemed to be showing the same observations as that of Experiment 7, the coagulant system concentration was increased to 4.2 mg/L, a level that would supply more than enough coagulant to the system. However, effluent turbidity did not deviate from 33-35 NTU and there was no formation of a floc blanket even with the increased coagulant input to the system.

<p align = center>
  <img src ="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/exp8new2.png" width = 150>
</p>
Figure 11. Instead of a floc blanket, Experiment 8 only formed dispersed flocs as shown above.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-10-2018%20a.png">
</p>

Figure 12. Effluent turbidity vs. Time with a 2 mm/s Upflow Velocity at 2.8 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 9
**Description**: To confirm that insufficient levels of coagulant were not the cause of system failure and that timing was not the issue, Experiment 9 ran at 2 mm/s with a coagulant system concentration of 4.2 mg/L from the beginning.

**Results**: Large flocs formed in the sedimentation tank near the beginning of this experiment, indicating that there is more than enough coagulant in the system. Therefore, an insufficient level of coagulant in the system does not seem to be the cause for system failure. From these experiments, it is now hypothesized that 2 mm/s is still to slow to make a healthy floc blanket and thus cleaner effluent waters.

<p align="center">
  <a href="https://www.youtube.com/watch?v=dMs-pc6IACs&feature=youtu.be"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Exp9Pic.PNG" width=200> </a>
</p>

Figure 13. Click the image or [this link](https://www.youtube.com/watch?v=dMs-pc6IACs&feature=youtu.be) for a video of the sedimentation tank during Experiment 9.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-10-2018%20b.png">
</p>

Figure 14. Effluent turbidity vs. Time with a 2 mm/s Upflow Velocity at 4.2 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 10
**Description**: The next series of experiments were run at a higher upflow velocity of 3 mm/s. This was done to further confirm that 2 mm/s was still too slow for floc blanket formation and thus system success. Experiment 10 had a system coagulant dosage of 1.5 mg/L.

**Results**: Effluent turbidity initially spiked to ~45 NTU but decreased to a somewhat stable value of ~15 NTU. While 15 NTU does not meet the turbidity standards for the World Health Organization or the EPA, this experiment may have well reached 0.3 NTU had not the initial spike in effluent turbidity occurred. Unlike the experiments at slower upflow velocities, a healthy floc blanket formed and showed a density gradient as time passed.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-11-2018.png">
</p>

Figure 15. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity at 1.5 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 11
**Description**: Experiment 11 ran at 3 mm/s with a coagulant system concentration of 3.0 mg/L.

**Results**: Effluent turbidity stabilized around 16 NTU by the time 20.5 hours passed. A healthy floc blanket formed about 1.5 hours faster in Experiment 11 than in Experiment 10. Therefore, the trend seems to be that a higher system coagulant dosage leads to faster floc blanket formation and thus system success.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-12-2018.png">
</p>

Figure 16. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity at 3.0 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 12
**Description**: Experiment 12 ran at 3 mm/s with a coagulant system concentration of 4.5 mg/L.

**Results**: Effluent turbidity initially spiked to ~22 NTU but rapidly decreased to 2-3 NTU after 1 hour, most likely due to the formation of a healthy floc blanket early on. As the experiment progressed the floc blanket did experience decay, causing the effluent turbidity to increase to 11-12 NTU. Another key observation is that as you increase the upflow velocity, the size of flocs in the flocculator decrease. For the 3 mm/s experiments, there was a good mixture of small and bigger flocs in the floccualtor. These results suggest that a higher upflow velocity combined with a higher coagulant dosage contribute to system success. As of now, this combination of a 3 mm/s upflow velocity and a system coagulant dosage of 4.5 mg/L seems to demonstrate optimal high rate sedimentation performance.

<p align = "center">
  <a href="https://www.youtube.com/watch?v=mQuRGDWsnd4&feature=youtu.be"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Experiment12NEW.png" width = 200> </a>
  </p>

Figure 17. Click the image or [this link](https://www.youtube.com/watch?v=mQuRGDWsnd4&feature=youtu.be) for a video of the sedimentation tank during Experiment 12.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-16-2018.png">
</p>

Figure 18. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity at 4.5 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 13
**Description**: Experiment 13 was run to see if an even higher upflow velocity could preserve system success. Experiment 13 was run at 4 mm/s with a coagulant system concentration of 4.5 mg/L.

**Results**: Effluent turbidity initially spiked to ~50 NTU but rapidly decreased to 16-17 NTU after 3 hours. Flocs in the flocculator were only small, indicating that 4 mm/s might be too fast for the flocs to sufficiently collide with one another and flocculate before entering the sedimentation tank. Visible gelling in the sedimentation tank and the flocculator indicate excess system coagulant, which was hypothesized to have contributed to system failure.

<p align="center">
  <a href="https://www.youtube.com/watch?v=aITr4ERrPCg&feature=youtu.be%22"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Exp13Picnew.png" width=150> </a>
</p>

Figure 19. Click the image or [this link](https://www.youtube.com/watch?v=aITr4ERrPCg&feature=youtu.be%22) for a video of the sedimentation tank during Experiment 13.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-17-2018.png">
</p>

Figure 20. Effluent turbidity vs. Time with a 4 mm/s Upflow Velocity at 4.5 mg/L System Coagulant Concentration

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 14
**Description**: To see whether system failure was a result of inputting too concentrated amounts of coagulant into the system at a given time, Experiment 14 was run at 4 mm/s with the same coagulant system concentration as that of Experiment 13 but with a diluted coagulant stock and an increased coagulant pump speed.

**Results**: Effluent turbidity stabilized around 30 NTU. Like experiment 13, gelling in the sedimentation tank and flocculator was observed. Therefore, it seems like 4 mm/s is too high of an upflow velocity to achieve system success given this sedimentation design.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-18-2018.png">
</p>

Figure 21. Effluent turbidity vs. Time with a 4 mm/s Upflow Velocity at 4.5 mg/L System Coagulant Concentration with Diluted Coagulant Stock and Increased Coagulant Pump Speed

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 15

**Ian's Comment:** This would be a great experiment to include a video from if you have any

**Description**: To gain a better understanding about floc movement the moment when flocs and water first enter the sedimentation tank, a new sedimentation bottom geometry was inserted using a PVC rod. This additional piece had a flat bottom with a 3/16" hole drilled through its entirety. Experiment 15 ran at 3 mm/s using Tank A with a system coagulant dosage of 4.5 mg/L.

<p align = center>
  <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/FlatBottomNew.jpeg" width = 400>
  </p>

Figure 22: Flat bottom insert of the sedimentation tank.

**Results**: Due to the flat geometry of the new insert, flocs built up from the beginning of the experiment, allowing only a small jetstream of water+flocs to flow through the very center of the recirculator. During the first hour of experimentation, the floc buildup at the bottom was growing at a rate of 1/2" every 10 minutes all around in the 1" diameter sedimentation tank. There were no initial signs of floc blanket formation so the experiment was stopped after 1 hour.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-19-2018.png">
</p>

Figure 23. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity at 4.5 mg/L System Coagulant Concentration with Flat Tank Bottom Insert

[Return to Summary of Experiments](#summary-of-experiments)

#### Experiment 16
**Description**: The flat bottom geometry was modified to have a conical shape in order to allow for better resuspension of built-up flocs aggregating at the bottom of the sedimentation tank. Experiment 15 was run at 3 mm/s with a system coagulant dosage of 4.5 mg/L.

<p align = center>
  <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/ConicalBottom.jpg" width = 250>
  <align = center>
    <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/conicalbottom2.jpeg" width = 200>
</p>

Figure 24: Conical bottom insert of the sedimentation tank.

**Results**: While there seemed to have a more stable floc blanket in the recirculator, this experiment was also a failure. Flocs still built up at the bottom of the tank. It is hypothesized that a ring of flocs and coagulant larger than the drilled hole in the insert prevents the flocs from reaching the hole for resuspension, causing buildup.

<p align = center>
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Graphs/7-23-2018.png">
</p>

Figure 25. Effluent turbidity vs. Time with a 3 mm/s Upflow Velocity at 4.5 mg/L System Coagulant Concentration with Conical Tank Bottom Insert

[Return to Summary of Experiments](#summary-of-experiments)

### Future Work
Coming into this project, the research question was to investigate the cause behind floc blanket decay. However, once experimentation began, this question changed to figuring out why a floc blanket does not form under theoretically optimal conditions. Our initial thoughts were that there was an insufficient level of coagulant in the system, but our results suggest that this is not the case. In fact, we have seen there is such a thing as too much coagulant in the system, which may also contribute to system failure.

Therefore, future work will consist of investigating what happens the moment when flocs and water enter the sedimentation tank. This was done by elevating the bottom with a fabricated insert as depicted in Figures 22 and 24. Since the flat and conically-shaped tank inserts failed as flocs built up at the bottom, future work will consist of modifying the geometry further in order to induce optimal resuspension of flocs for floc blanket formation.

As briefly mentioned in the results section for Experiment 16, we hypothesize that there is a ring of flocs and coagulant larger than the drilled hole in the insert prevents the flocs from reaching the hole for resuspension, causing buildup and thus system failure. In order to combat floc buildup, we plan on drilling a larger hole a specific distance from the top in order to fulfill the 10:1 jet expansion ratio. That way, any build up that may form at the bottom of the sedimentation tank may not form.

If this solution does not work, the next step will be to design and fabricate a completely new sedimentation tank that would more closely resemble a jet reverser that is currently in use at AguaClara plants.


### Calculations
We have written code in Python for calculating the system flow rate, water pump speed, coagulant concentration, and coagulant pump speed given an upflow velocity and other parameters. (These calculations are in the process of being integrated into the aguaclara_research repository as revised as well as added functions.)

The calculations in the "Current coagulant dosage calculations" section of our code differ from those of previous HRS teams in that the coagulant pump speed is the quotient of the desired flow rate of coagulant (mL/s) divided by the volume pumped per revolution by the coagulant pump (mL/rev), rather than the desired flow rate of coagulant (mL/s) divided by the flow rate of the coagulant pump (mL/s).

We now also use a similar calculation for water pump speed using values for volume per revolution given by the tubing's specifications, in place of obtaining them experimentally. (Volume per revolution was previously obtained by measuring water output in a set amount of time.)

See the equations below for clarification.

$S$ = pump speed
$Q$ = flow rate
$V$ = volume per revolution

$$S\ \frac{rev}{min} = \frac{Q\ \frac{mL}{min}}{V\ \frac{mL}{rev}}$$

Note: Since certain components of the aguaclara_research library are currently under constructon, to use the library you must first clone the [aide_design git repository](https://github.com/AguaClara/aide_design) , switch to its filter_design branch, and then follow the pip install instructions on the [aguaclara_research git repository](https://github.com/AguaClara/aguaclara_research) README.

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


### Graphing

Below is code written in Python for graphing a column of data from a ProCoDA file. All graphs of experimental effluent turbidity over time in this report were generated by this code.

##### Graphing ProCoDA data without statelog

The functions below (which are in the process of being documented and reviewed) plot a scatterplot of two columns of data from a ProCoDA data file based on start and end times only, instead of states. As now, data can be read for experiments spanning up to 2 days. See the bottom of the document for an example usage of the functions.

```python
import pandas as pd
import matplotlib.pyplot as plt
from aide_design.shared.units import unit_registry as u

def time_to_day_fraction(time):
  '''
  Parameters
  ----------
  time
    string in the form of hh:mm
  '''
  hour = int(time.split(":")[0])
  minute = int(time.split(":")[1])
  return hour/24 + minute/1440


def remove_notes(data):
  '''
  Parameters
  ----------
  data
    pandas.DataFrame object
  '''
  has_text = data.iloc[:,0].astype(str).str.contains('[a-z]', '[A-Z]')
  text_rows = list(has_text.index[has_text])
  return data.drop(text_rows)

def plot_columns(directory, extension, start_datetime, end_datetime, x_column, y_column):
  '''
  Parameters
  ----------
  start_datetime and end_datetime
      must be in the format 'MM-DD-YYYY hh:mm' (24 hr time)
  interval
      in seconds, minutes, or hours
  x_column and y_column
      for now, only integer indices
  directory
      must end in '/'
  extension
      preceeded by '.', such as '.csv'
  '''
  # Locate data file(s)
  start_date = start_datetime.split(' ')[0]
  paths = [directory + "datalog " + start_date + extension]
  data = [remove_notes(pd.read_csv(paths[0], delimiter='\t'))]

  end_date = end_datetime.split(' ')[0]
  if start_date != end_date:
    paths.append(directory + "datalog " + end_date + extension)
    data.append(remove_notes(pd.read_csv(paths[1], delimiter='\t')))

  # Calculate start index
  start_time = time_to_day_fraction(start_datetime.split(' ')[1])
  time_column = pd.to_numeric(data[0].iloc[:, 0])
  interval = time_column[2]-time_column[1]

  start_idx = int(round((start_time - time_column[1])/interval + .5)) #round up

  # Calculate end index and get columns of interest
  end_time = time_to_day_fraction(end_datetime.split(' ')[1])
  if len(paths) == 1:
    end_idx = int(round((end_time - time_column[1])/interval + .5)) #round up
    x = pd.to_numeric(data[0].iloc[start_idx:end_idx, x_column])
    y = pd.to_numeric(data[0].iloc[start_idx:end_idx, y_column])

  else:
    time_column = pd.to_numeric(data[1].iloc[:, 0])
    end_idx = int(round((end_time - time_column[1])/interval + .5)) #round up
    x = list(pd.to_numeric(data[0].iloc[start_idx:, x_column]))
    x += list(pd.to_numeric(data[1].iloc[:end_idx, x_column]) + 1)
    y = list(pd.to_numeric(data[0].iloc[start_idx:, y_column]))
    y += list(pd.to_numeric(data[1].iloc[:end_idx, y_column]))

  plt.figure(figsize=(12,4))
  plt.plot(x, y, 'o', markersize = 2)
  plt.xlabel(list(data[0])[x_column])
  plt.ylabel(list(data[0])[y_column])
  plt.title(list(data[0])[y_column] + " vs " + list(data[0])[x_column])
  plt.minorticks_on()
  plt.grid(which = 'major')
  plt.grid(which = 'minor')
  plt.show()

#example usage
plot_columns('/Users/Me/Documents/Atom/high_rate_sedimentation/ProCoDA Data Files/','.xls', '6-14-2018 12:20', '6-15-2018 10:50', 0, 4)
```

### Other Insights

**Spiking influent turbidity**
The influent turbidity consistently spikes upwards at the start of experiments. While previously we associated the spike with the turning on of the coagulant pump, we now believe it is due to the necessary redirection of flow in the system (of clay and water going to the flocculator instead of waste). The redirection of flow, which involves the opening and shutting of values, seems to introduce a bubble of air into flocculator that congests flow and may be causing clay to accumulate behind the bubble, all the way to the influent turbidimeter.

**ProCoDa method files**
Since losing our ProCoDa program settings after to a computer restart, we have decided to save snapshots of our ProCoDa setpoints and states after making any significant modifications, such as adding setpoints and variables (e.g. pressure from the pressure sensor), changing setpoint values (e.g. tuning the PID constants), and changing state logic (e.g. periodically flushing the system with a higher water pump speed).

We accomplish this by _saving a new method file_ in our datalog directory with a name corresponding to the experiment and date. The method file behaves as a "snapshot" because ProCoDa continues to read and write its program settings to one particular method file in the `C:\ProCoDa Data` directory, usually `ProCoDa 0.pcm` (0 may be replaced with another number), while leaving the manually uploaded method file untouched.

The past method files stored on the HRS computer and our current method file have been saved to our Github repository.

<p align="center">
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Config%20Tab_Method%20Files.PNG" height=275>
</p>

Figure 4. Above is the Configuration in ProCoDa. Click the icon pointed to by the red arrow to save a method file snapshot and the icon pointed to by the blue arrow to open a snapshot.

**Sedimentation tank leaks**
If it appears that water is leaking out of the sedimentation tank from where the floc weir was welded to the recirculator or tube settler, you will need to re-weld the connection.

To identify the exact source(s) of the leaking, it is recommended to fill the sedimentation tank with water mixed with dye and dry the exterior of the tank so that any new beads of liquid that emerge are easily detected. You can also dry the exterior, press a dry paper towel against the area of leakage, and match any wet spots on the paper towel to sources of leakage on the tank.
