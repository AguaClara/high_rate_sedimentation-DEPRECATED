#High Rate Sedimentation, Summer 2018
#### Anna Hong and Hannah Si
#### July 27, 2018

## Abstract
Sedimentation is a critical process for water treatment plants by which coagulated minerals, dirt, and other particles are removed from the water via gravitational settling. The High Rate Sedimentation (HRS) team hopes to design a sedimentation tank that will yield an effluent with turbidity of 0.3 NTU or lower at a high upflow velocity. While 1 NTU is the World Health Organization's standard for turbidity drinking water, the EPA standard is 0.3 NTU. AguaClara currently achieves this with an upflow velocity of 1 mm/s, but not at upflow velocities of 3 mm/s or greater. Therefore, the goal of HRS team is to to preserve system success while raising upflow velocity in order to provide more clean water in a given time without increasing treatment plant size. Operating at a greater efficiency would eliminate the need for additional building materials and higher construction and maintenance costs.

Since the fall of 2017, the AguaClara High Rate Sedimentation (HRS) team has been investigating the cause behind floc blanket decay, which has been attributed to system failure, at high upflow velocities in the sedimentation tank. The Summer 2018 HRS team first conducted experiments at lower upflow velocities of 1 mm/s and 2 mm/s in a 1" diameter tube to replicate system success. However, after failing to produce a floc blanket at these lower upflow velocities yet succeeding at higher velocities, the Summer 2018 HRS team has focused on optimizing sedimentation at a higher upflow velocity of 3 mm/s. The team confirmed the optimal coagulant dosage to be approximately 4.5 mg/L of PACl and is currently redesigning the sedimentation tank's bottom geometry to enhance resuspension of flocs.

## Methods
### Experimental Apparatus
Below is a picture of the revised lab bench setup of the HRS team followed by a table listing the various components.

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

The guidelines below are not comprehensive. For detailed instructions preparing the High Rate Sedimentation experimental setup, refer to the [HRS Setup Procedures](LINK HERE) document in our Github repository.


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

9. Clean out the influent and effluent turbidimeters.
   a. Even without water running, shut and open the appropriate values to bypass the turbidimeter so that water doesn't leak into it while cleaning
   b. Unlock and take out the black cylinder on top of the turbidimeter.
   c. Unscrew the glass vial, empty and rinse it, then fill it with clean water. Tap water is sufficient.
   d. Screw the vial back in, wipe the bottle and cylinder free from water droplets or fingerprints, and then lock the black cylinder back into the turbidimeter.
   e. If you used the white screws on the outflow turbidimeter tubes to block water passage, remember to unscrew them.

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

The HRS team has been experimenting with two sedimentation tank designs in an effort to understand the reasons for floc blanket decay in the Spring 2018 and Fall 2017 semesters.

1. **Sedimentation tank A** is the sedimentation tank design used by most AguaClara particle removal research teams, including the HRS team in the Fall 2017 semester. The tube settler is relatively short and the floc weir is placed on the left side of the tube settler (when the tube settler points to the left).

<p align="center">
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Sedimentation%20Tank%20A.png" width=300>
</p>

Figure 2. Sedimentation Tank A, the sedimentation tank used by most AguaClara research teams, including the Fall 2017 HRS team.

2. **Sedimentation tank B** is the sedimentation tank design used by the Spring 2018 HRS team. The tube settler is relatively long and the floc weir is placed on the right side of the bend in the recirculator (when the tube settler points to the left).

<p align="center">
  <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/SedTankB.png" width=300>
</p>
Figure 3. Sedimentation Tank B, the sedimentation tank used by the Spring 2018 HRS research subteam.

### Table of Contents

#### Previous Experiments
* [Summary of Previous Experiments](#summary-of-previous-experiments)
1. [Experiment 1](#experiment-1)
2. [Experiment 2](#experiment-2)
3. [Experiment 3](#experiment-3)
4. [Experiment 4](#experiment-4)
5. [Experiment 5](#experiment-5)
6. [Experiment 6](#experiment-6)
* [Sedimentation Tank A vs. B](#sedimentation-tank-a-vs.-b)

#### New Experiments
* [Summary of New Experiments](#summary-of-new-experiments)
7. [Experiment 7](#experiment-7)
8. [Experiment 8](#experiment-8)
9. [Experiment 9](#experiment-9)
10. [Experiment 10](#experiment-10)
11. [Experiment 11](#experiment-11)
12. [Experiment 12](#experiment-12)
13. [Experiment 13](#experiment-13)
14. [Experiment 14](#experiment-14)
15. [Experiment 15](#experiment-15)
16. [Experiment 16](#experiment-16)

#### Summary of Previous Experiments
|Experiment #|Upflow Velocity (mm/s) |Tank Type| Coagulant System Concentration (mg/L)|Floc Blanket Formed| Results|
|:---:|:---------------:|:----:| :-------: |:------| :--- |
|1|3|A|1.4|Yes|Effluent turbidity <= 2.0 NTU.
|2|3|B|1.4|Yes|Effluent turbidity stayed around 4.4 NTU for the first 10 hours of experimentation but increased to 19.5 NTU at 22.5 hours.
|3|1|B|1.4 with initial excess coagulant|No|Effluent turbidity increased to 135 NTU. There was an initial excess in coagulant that may have caused the failure.
|4|1|B|1.4 with appropriate dosage of coagulant|No|Effluent turbidity ended at 20 NTU and there was no observable formation of a floc blanket. Disproves hypothesis that initial excess coagulant caused system failure. New hypothesis that upflow velocity of 1 mm/s is too slow.
|5|3|A|1.4|Yes|Effluent turbidity ended at 26 NTU after 18 hours of experimentation. Floc blanket formation occurred later than it had before in Experiment 1.
|6|1 -> 2| A |1.4| Failure. Effluent turbidity ended at 46 NTU even after increasing the upflow velocity to 2 mm/s after first two hours. Results suggest that 2 mm/s may still be too slow for system success.|
[Table of Contents](#table-of-contents)
#### Experiment 1

<!--I would encourage you to add any photos or videos you've collected during these experiments.  A picture is worth a thousand words! -->

<!--I would also add graphs of ProCoDa data collected, primarily effluent turbidity.  This will provide much better understanding and allow readers to make their own conclusions.  This should be done through Python using the aguaclara_research code. -->
**Description**: The purpose of the first two experiments is to record initial observations of floc blanket formation and decay using both sedimentation tank designs. For Experiment 1, the HRS apparatus was run at an upflow velocity of 3 mm/s for 9.5 hours using tank A in order to confirm whether this higher rate would lead to floc blanket decay causing system failure.

**Results**: At about two and a half hours into the experiment, an opaque floc blanket has formed in the recirculator. By the end of this shorter experiment, the effluent turbidity did not rise above 2.0 NTU, making this a success. Whether this success was due to the floc weir being in an optimal position or having a more robust system will need to be further investigated.
[Table of Contents](#table-of-contents)

#### Experiment 2

**Description**: Experiment 2 ran a test with an upflow velocity of 3 mm/s using tank B at a longer time (22.5 hours). This test would help confirm whether the sedimentation tank design plays a factor in floc blanket decay and thus system failure.

**Results**: At the same time when Experiment 1 ended (9.5 hours), the effluent turbidity reached 4.4 NTU. Movement of flocs at this time was slower than that observed in tank A and the floc blanket was not opaque. Since these observations seemed to be characteristic of  earlier stages of floc blanket formation and decay, the experiment was prolonged to 22.5 hours. By the end of this experiment, system failure was observed with a final effluent turbidity of 19.5 NTU. This slower decay may be due to using a more robust system. Nonetheless, this experiment was concluded to be a partial success. [Table of Contents](#table-of-contents)

<p align="center">
  <a href="https://www.youtube.com/watch?v=JcQjRKY91NI&feature=youtu.be"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Exp2pic.PNG" width=300> </a>
</p>

Figure \_. Click the image or [this link](https://www.youtube.com/watch?v=dMs-pc6IACs&feature=youtu.be) for a video of the sedimentation tank during Experiment 2.


#### Experiment 3
**Description**: The next set of experiments were done at a slower upflow velocity in order to simulate and confirm system success observed at AguaClara treatment plants. This experiment tested a 1 mm/s upflow velocity using tank B. For the first 30 minutes, there was an input of excess coagulant because the coagulant pump speed was not reduced from 20 RPM to 6.7 RPM to reflect this lower upflow velocity.

**Results**: The initial effluent turbidity began at 4.6 NTU and increased throughout the duration of the experiment quite rapidly. By the end of 20 hours, the effluent turbidity was higher than influent turbidity at 135 NTU, making this a failure. It was hypothesized that the influx of large amounts of coagulant at the beginning of the experiment caused coagulant to stick to the walls, causing higher shear and decreased diameter. Coagulant particles may be colliding with other coagulant particles instead of clay particles, which only form small flocs. These small particles are more difficult to capture and thus travel upwards to the tube settler and out in the effluent tube. [Table of Contents](#table-of-contents)

#### Experiment 4

**Description**: To nullify any potential effects from the initial coagulant dosage spike in Experiment 3, this experiment ran at 1 mm/s with the appropriate coagulant pump speed of 6.7 RPM for 8 hours.

**Results**: With a final effluent turbidity of 20 NTU, system failure was observed, disproving that initial excess coagulant was the cause. There was no observable formation of a floc blanket, which means that the smaller flocs that were contaminating the effluent were not being captured and settled out. One key observation was that there seemed to be a gradual increase in floc size within the flocculator as it neared its end. However, the unusually clear sedimentation tank raises the question as to where these bigger flocs ended up going. Since excess coagulant does not seem to be preventing floc blanket formation and that the larger flocs from the flocculator seem to have disappeared, it is hypothesized that the upflow velocity of 1 mm/s is too slow. [Table of Contents](#table-of-contents)

#### Experiment 5

**Description**: To make sure that the changes that we made to our experimental apparatus is not the cause of system failure, Experiment 1 (3 mm/s upflow velocity with tank A) was rerun but for a longer period of 18 hours.

**Results**: As before, an opaque floc blanket formed with the same density gradient of flocs in the recirculator (higher density of flocs at the top compared to the bottom). However, this experiment ended with a slowly rising effluent turbidity of 26 NTU at 18 hours. There were many flocs settled in the tube settler, which may have reached there before the formation of the floc blanket. It seems that the floc blanket formed later than it had before in Experiment 1, allowing the smaller flocs that are more difficult to capture travel up to the tube settler and out the effluent tube. This much higher effluent turbidity suggests that something has changed since Experiment 1, but whether the design of the system was the change has yet to be determined. [Table of Contents](#table-of-contents)

#### Experiment 6

**Description**: Since Experiment 1 was a success at an upflow velocity of 3 mm/s, it was predicted that running the same experiment at a lower upflow velocity of 1 mm/s would also be a success. About 2 hours after the start of the experiment, there was still no signs of floc blanket formation. Since other AguaClara subteams experienced system success at a 2 mm/s upflow velocity, the water and coagulant pump speeds were increased to reflect this higher speed to test the hypothesis that upflow velocity was indeed too slow as formulated after Experiment 4.

**Results**: Ending with an effluent turbidity of 46 NTU, this experiment observed system failure. No floc blanket formed throughout the duration of the experiment even with the increased speeds. While it seemed that there could be a speed too slow for this system to succeed, these results suggest that a different factor is causing system failure. [Table of Contents](#table-of-contents)

#### **Sedimentation Tank A vs. B**
Since the design of the sedimentation tank did not seem to be the deciding factor between system success and failure, the subsequent experiments were conducted using the standard design tank A as it is the configuration that other AguaClara subteams use. <!--Should we include more in this paragraph? We can't really talk about the difference in floc removal...) -->[Table of Contents](#table-of-contents)

### Summary of New Experiments
* Note: All experiments were run using tank A

|Experiment #| Upflow Velocity (mm/s) | Coagulant System Concentration (mg/L)|Results|
|:---:|:---:| :--------: |:------------------------------|
|7|2|1.4|Failure. Effluent turbidity of 37-40 NTU and no formation of floc blanket.|
|8|2|2.8 but increased to 4.2 after ~ 1hr|Effluent turbidity of 33-35 NTU and no formation of floc blanket.|
|9|2|4.2|Failure. Effluent turbidity ranged from 35-40 NTU and no formation of floc blanket.|
|10|3|1.5|Effluent turbidity initially spiked to ~45 NTU yet decreased to a somewhat stable value of ~15 NTU. Floc blanket started to decay at 3 hours into the experiment.|
|11|3|3.0|Effluent turbidity stabilized around 16 NTU by 20.5 hours. It seems like a higher coagulant dosage leads to faster floc blanket formation.|
|12|3|4.5|Initial spike of effluent turbidity to ~22 NTU but rapidly decreased to 2-3 NTU after 1 hour, most likely due to formation of a healthy floc blanket. Suggests that a higher upflow velocity and a higher coagulant dosage contribute to system success.|
|13|4|4.5|Initial spike of effluent turbidity to ~50 NTU but decreased to 16-17 NTU after 3 hours. Visible gelling in the sedimentation tank and the flocculator indicate excess system coagulant.|
|14|4|4.5 but diluted coagulant stock and increased the coagulant pump speed.|Failure. Effluent turbidity stabilized ~30 NTU. Observed gelling in the sedimentation tank and flocculator. It seems like 4 mm/s is to high of an upflow velocity.|
|15|3|4.5|Failure. Inserted a new sedimentation tank bottom in order to see what is happening near the inlet of water and flocs. Buildup of flocs due to the flat surface of the tank bottom.|
|16|3|4.5|Modified the new sedimentation tank bottom to have a conical shape rather than a flat one.|
[Table of Contents](#table-of-contents)

#### Experiment 7
**Description**: The following three experiments ran at upflow velocities of 2 mm/s in order to confirm whether 2 mm/s is indeed too slow to achieve system success. Experiment 7 ran at 2 mm/s with a coagulant system concentration of 1.4 mg/L.

**Results**: Ending with an effluent turbidity of 37-40 NTU, this experiment observed system failure. No floc blanket formed throughout the duration of the experiment, which was around 7 hours. Whether this failure was a result of insufficient levels of coagulant in the system or due to too low of an upflow velocity has yet to be determined. [Table of Contents](#table-of-contents)

#### Experiment 8
**Description**: Experiment 8 ran at 2 mm/s using tank A with a coagulant system concentration of 2.8 mg/L, which was increased to 4.2 mg/L after 1 hour into the experiment.  

**Results**: Since this experiment seemed to be showing the same observations as that of Experiment 7, the coagulant system concentration was increased to 4.2 mg/L, a level that would supply more than enough coagulant to the system. However, effluent turbidity did not deviate from 33-35 NTU and there was no formation of a floc blanket even with the increased coagulant input to the system. [Table of Contents](#table-of-contents)

<p align = center>
  <img src ="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/exp8new2.png" width = 150>
</p>

#### Experiment 9
**Description**: To confirm that insufficient levels of coagulant were not the cause of system failure and that timing was not the issue, Experiment 9 ran at 2 mm/s with a coagulant system concentration of 4.2 mg/L from the beginning.

**Results**: Large flocs formed in the sedimentation tank near the beginning of this experiment, indicating that there is more than enough coagulant in the system. Therefore, an insufficient level of coagulant in the system does not seem to be the cause for system failure. From these experiments, it is now hypothesized that 2 mm/s is still to slow to make a healthy floc blanket and thus cleaner effluent waters. [Table of Contents](#table-of-contents)

<p align="center">
  <a href="https://www.youtube.com/watch?v=dMs-pc6IACs&feature=youtu.be"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Exp9Pic.PNG" width=200> </a>
</p>

Figure \_. Click the image or [this link](https://www.youtube.com/watch?v=dMs-pc6IACs&feature=youtu.be) for a video of the sedimentation tank during Experiment 9.

#### Experiment 10
**Description**: The next series of experiments were run at a higher upflow velocity of 3 mm/s. This was done to further confirm that 2 mm/s was still too slow for floc blanket formation and thus system success. Experiment 10 had a system coagulant dosage of 1.5 mg/L.

**Results**: Effluent turbidity initially spiked to ~45 NTU but decreased to a somewhat stable value of ~15 NTU. While 15 NTU does not meet the turbidity standards for the World Health Organization or the EPA, this experiment may have well reached 0.3 NTU had not the initial spike in effluent turbidity occurred. Unlike the experiments at slower upflow velocities, a healthy floc blanket formed and showed a density gradient as time passed. [Table of Contents](#table-of-contents)

#### Experiment 11
**Description**: Experiment 11 ran at 3 mm/s with a coagulant system concentration of 3.0 mg/L.

**Results**: Effluent turbidity stabilized around 16 NTU by the time 20.5 hours passed. A healthy floc blanket formed about 1.5 hours faster in Experiment 11 than in Experiment 10. Therefore, the trend seems to be that a higher system coagulant dosage leads to faster floc blanket formation and thus system success. [Table of Contents](#table-of-contents)

#### Experiment 12
**Description**: Experiment 12 ran at 3 mm/s with a coagulant system concentration of 4.5 mg/L.

**Results**: Effluent turbidity initially spiked to ~22 NTU but rapidly decreased to 2-3 NTU after 1 hour, most likely due to the formation of a healthy floc blanket early on. As the experiment progressed the floc blanket did experience decay, causing the effluent turbidity to increase to 11-12 NTU. Another key observation is that as you increase the upflow velocity, the size of flocs in the flocculator decrease. For the 3 mm/s experiments, there was a good mixture of small and bigger flocs in the floccualtor. These results suggest that a higher upflow velocity combined with a higher coagulant dosage contribute to system success. As of now, this combination of a 3 mm/s upflow velocity and a system coagulant dosage of 4.5 mg/L seems to demonstrate optimal high rate sedimentation performance. [Table of Contents](#table-of-contents)

<p align = "center">
  <a href="https://www.youtube.com/watch?v=mQuRGDWsnd4&feature=youtu.be"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Experiment12NEW.png" width = 200> </a>
  </p>

Figure \_. Click the image or [this link](https://www.youtube.com/watch?v=mQuRGDWsnd4&feature=youtu.be) for a video of the sedimentation tank during Experiment 12.

#### Experiment 13
**Description**: Experiment 13 was run to see if an even higher upflow velocity could preserve system success. Experiment 13 was run at 4 mm/s with a coagulant system concentration of 4.5 mg/L.

**Results**: Effluent turbidity initially spiked to ~50 NTU but rapidly decreased to 16-17 NTU after 3 hours. Flocs in the flocculator were only small, indicating that 4 mm/s might be too fast for the flocs to sufficiently collide with one another and flocculate before entering the sedimentation tank. Visible gelling in the sedimentation tank and the flocculator indicate excess system coagulant, which was hypothesized to have contributed to system failure. [Table of Contents](#table-of-contents)

<p align="center">
  <a href="https://www.youtube.com/watch?v=aITr4ERrPCg&feature=youtu.be%22"> <img src="https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/Exp13Picnew.png" width=150> </a>
</p>

Figure \_. Click the image or [this link](https://www.youtube.com/watch?v=aITr4ERrPCg&feature=youtu.be%22) for a video of the sedimentation tank during Experiment 13.

#### Experiment 14
**Description**: To see whether system failure was a result of inputting too concentrated amounts of coagulant into the system at a given time, Experiment 14 was run at 4 mm/s with the same coagulant system concentration as that of Experiment 13 but with a diluted coagulant stock and an increased coagulant pump speed.

**Results**: Effluent turbidity stabilized around 30 NTU. Like experiment 13, gelling in the sedimentation tank and flocculator was observed. Therefore, it seems like 4 mm/s is too high of an upflow velocity to achieve system success given this sedimentation design. [Table of Contents](#table-of-contents)

#### Experiment 15
**Description**: To gain a better understanding about floc movement the moment when flocs and water first enter the sedimentation tank, a new sedimentation bottom geometry was inserted using a PVC rod. This additional piece had a flat bottom with a 3/16" hole drilled through its entirety. Experiment 15 ran at 3 mm/s using tank A with a system coagulant dosage of 4.5 mg/L.

<p align = center>
  <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/FlatBottomNew.jpeg" width = 400>
  </p>

**Results**: Due to the flat geometry of the new insert, flocs built up from the beginning of the experiment, allowing only a small jetstream of water+flocs to flow through the very center of the recirculator. During the first hour of experimentation, the floc buildup at the bottom was growing at a rate of 1/2" every 10 minutes all around in the 1" diameter sedimentation tank. There were no initial signs of floc blanket formation so the experiment was stopped after 1 hour. [Table of Contents](#table-of-contents)

#### Experiment 16
**Description**: The flat bottom geometry was modified to have a conical shape in order to allow for better resuspension of built-up flocs aggregating at the bottom of the sedimentation tank. Experiment 15 was run at 3 mm/s with a system coagulant dosage of 4.5 mg/L.

**Results**: While there seemed to have a more stable floc blanket in the recirculator, this experiment was also a failure. Flocs still built up at the bottom of the tank. It is hypothesized that a ring of flocs and coagulant larger than the drilled hole in the insert prevents the flocs from reaching the hole for resuspension, causing buildup. [Table of Contents](#table-of-contents)

<p align = center>
  <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/ConicalBottom.jpg" width = 300>
  <align = center>
    <img src = "https://raw.githubusercontent.com/AguaClara/high_rate_sedimentation/master/Images/conicalbottom2.jpeg" width = 250>
</p>

### Future Work
The cause of floc blanket decay and thus system failure has yet to be determined. Future work will focus on verifying pump speed calculations for the water pump. Coagulant dosage will be experimentally adjusted in order to obtain the formation of a floc blanket. More immediately, experiments running at an upflow velocity of 2 mm/s will be tested with a lower coagulant dosage. <!--How are you planning on updating coagulant dosing? Trial and error or through calculations?-->

**INCLUDE INFORMATION ABOUT NEW SED TANK DESIGN TO INVENT WITH JET REVERSER CAPABILITIES. TALK ABOUT MODIFYING THE SED TANK DESIGN THAT TIM HELPED US MAKE**
-talk about the ring that forms

### Calculations
We have written code in Python for calculating the system flow rate, water pump speed, coagulant concentration, and coagulant pump speed given an upflow velocity and other parameters.<!--Are functions to do this available in aguaclara_research?  If not consider adding them, as these would be generally applicable to most particle removal teams -->

The calculations in the "Current coagulant dosage calculations" section of our code differ from those of previous HRS teams in that the coagulant pump speed is the quotient of the desired flow rate of coagulant (mL/s) divided by the volume pumped per revolution by the coagulant pump (mL/rev), rather than the desired flow rate of coagulant (mL/s) divided by the flow rate of the coagulant pump (mL/s).

We now also use a similar calculation for water pump speed using values for volume per revolution given by the tubing's specifications, in place of obtaining them experimentally. (Volume per revolution was previously obtained by measuring water output in a set amount of time.)

See the equations below for clarification.

$S$ = pump speed
$Q$ = flow rate
$V$ = volume per revolution

$$S\ \frac{rev}{min} = \frac{Q\ \frac{mL}{min}}{V\ \frac{mL}{rev}}$$

<!-- FYI the .shared branch only works if you have downloaded the filter design branch.  You might want to add a comment so others don't have the same problem (until they fix it)-->

<!--Make sure to properly comment your code and define variables.  For example, explain the difference between coagulant_superstock and coagulent_stock-->
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
tubing_water_ID = 17
Q_rev_water = tubing_water[tubing_water_ID]
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

### Other Insights



**Spiking influent turbidity**
The influent turbidity seems to spike upwards when we start the coagulant pump, even when the coagulant is not connected to the system or pumping coagulant. It has been suggested that the vibrations of the pump may be the cause, but we have yet to test this.

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
