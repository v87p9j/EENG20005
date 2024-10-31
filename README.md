java c
EENG20005 Coursework Script
Overview 
Submission 
.     SummaⅥve submission: A technical report in Week 23 accompanied by a package of all simulaⅥon models and codes.
.     Mid-term formaⅥve submission: A technical report for Part 1 and 2 in Week 12.
Laboratory sessions 
.     3 × 3-hour live sessions in Week 7, 8, 9
.     2 × 2-hour drop-in sessions in Week 10, 11
Report elements 
A.   DescripⅥon of approach/methodology
B.   MathemaⅥcal working
C.   SimulaⅥon waveform.
D.   Diagrams - phasor diagram, circuit diagram
E.   Results in data points presented in a table or a visualised graph (e.g. curve)
F.   Analysis and discussion of results
Part 1. AC power system 
Summary 
Design and analysis of an AC power system covering power generaⅥon, transmission, distribuⅥon and load.
Learning outcomes 
.     Design of ideal transformers
.     Electric power systems
.     Constant-power load vs. passive load
.     Phasor diagrams for analysing phase/amplitude relaⅥonships of sinusoidal signals
.     Power and impedance triangles
o  Power factor and impedance angles
.     Measurement and calculaⅥon of voltage, current and power quanⅥⅥes
o  Real (acⅥve), reacⅥve and apparent power
.    Power factor correcⅥon
.     Single-phase vs. three phase system
.    Composite and unbalanced load
Tools 
Simulink Simscape Power Systems (components in black)
.    Part1_Part2_library.slx
.    Part1_template.slx
How to use: copy components from Part1_Part2_library.slx into templates.
It is advised to save separate simulaⅥon ﬁles for each case study.

Case 1A Single-phase AC system 
Build a Simulink simulaⅥon model of a single-phase AC power system consisⅥng of the power generaⅥon, transmission, distribuⅥon and a load. The speciﬁcaⅥons are as below divided into Groups 1~5 determined by the last digit of the student number. Assuming ideal AC sources, transformers and transmission lines. 


Spec. 1 (* 0 or 1) 
Spec. 2 (* 2 or 3) 
Spec. 3 (* 4 or 5) 
Spec. 4 (* 6 or 7) 
Spec. 5 (* 8 or 9) 
Generator voltage 
VG 
20 kV 




Transmission line voltage 
VLine 
100 kV 




Consumer voltage 
V1 
10 kV 




Consumer 1 power 
P1 
200 kW 
180 kW 
150 kW 
120 kW 
100 kW 
Line frequency 
fo 
50 Hz 




* Last digit of student number
Task 1.1 
Show a circuit diagram of the whole system and describe it. Mark any voltage/current quanⅥⅥes or measurement points that you may refer to later.
Design the ideal transformers as needed in the system. How many transformers are required and what are their turn raⅥos?
Task 1.2 
Back to the provided speciﬁcaⅥons, work out the following currents analyⅥcally, assuming ideal condiⅥons.
- Generator current IG
- Transmission line current Iline
- Consumer load current Iload
Provide validaⅥon of the results by measuring out the waveforms in simulaⅥon.
Task 1.3 What are the beneﬁts of transmitting power at a higher voltage? What if the generator and transmission voltages are both aligned to the consumer voltage (hint: observe the current   under this hypotheⅥc scenario).
Case 1B Complex load While drawing a 200 kW, the industrial consumer 1 runs under a 0.75 power factor due to the load being an inducⅥve electric machine. Revise the simulaⅥon model starⅥng with a  constant load block in Sim代 写EENG20005 Coursework ScriptJava
代做程序编程语言ulink.
Task 1.4 
Work out the below quanⅥⅥes analyⅥcally. Measure out these quanⅥⅥes in simulaⅥon – do the simulaⅥon results agree with the analyⅥcal results?
- Generator real power PG
- Generator reacⅥve power QG
- Generator current IG
- Transmission line current Iline
- Consumer load current Iload
Compare the currents in Case 1.1 and Case 1.2 - what is the consequence of a load with signiﬁcant reacⅥve power?
Task 1.5 
Can you measure the real, reacⅥve and apparent power only using voltage and current probes? Demonstrate this in the simulaⅥon, and compare the result with a power meter. Explain the diﬀerence between the two results.
Task 1.6 
Replace the constant load block with a passive load formed by R and L components in series, which sⅥll saⅥsﬁes the same power and voltage speciﬁcaⅥons in this case. Work out the values analyⅥcally and validate the design in simulaⅥon. Use the power triangle to help your design. 
Case 1C Power factor correcⅥon (PFC) For the industrial customer, the naⅥonal grid imposes a ﬁnancial penalty unless their power factor can be improved to >0.95 lagging. A passive capacitor bank is used for correcⅥng the  power factor from Case 1B to 0.95. Set the ground reference to generator neutral point.Task 1.7 Show a circuit diagram describing the load. Mark any voltage/current quanƟƟ es that you may refer to later.Calculate the required capacitance value. Draw a power triangle for the power factor correcƟ on case. Validate the design in simulaƟ on.Task 1.8 Draw a phasor diagram for the load voltage and current quanƟƟ es including the PFC capacitor banks on each of the R, L, C components. Use the generator voltage as the reference.Task 1.9 Observe the grid-side power and currents. What are the benefits of PFC for the grid?
Case 1D (advanced task) Three-phase AC system 
Convert the single-phase system in Case 1B to an equivalent three-phase system while saⅥsfying the load speciﬁcaⅥons with a power factor of 0.75. For simpliﬁcaⅥon, assume the three-phase system is fully balanced without a neutral line. The load is star connected. 
Task 1.10 
Draw a circuit diagram of the whole system and describe it. Mark any voltage/current quanⅥⅥes or measurement points that you may refer to later.
Measure the total instantaneous power transmi廿ed by the three-phase system and compare it against the single-phase case in Case 1B - show waveforms and comment on the diﬀerence. 
Task 1.11
Measure the phase and line voltages on the load side. Comment on the waveforms and quanⅥⅥes comparing the phase and line voltages. Express the voltages and currents mathemaⅥcally.
Task 1.12 
If the grid frequency is set to 60 Hz, instead of 50 Hz, how would the passive RL load need to be changed to saⅥsfy the same power speciﬁcaⅥons?
Case 1E (advanced task) Composite load and unbalanced load 
Task 1.13 Based on the model in Case 1B, assume there is a second consumer drawing an S of 100 kVA and a power factor of 0.9. Work out the composite power factor of the loads and validate it  in simulaⅥon.
Task 1.14 
Based on the model in Case 1D, add a neutral line into the three-phase system and distribute the load power between Phase A, B, C unequally as 3:2:1 (instead of 1:1:1) represenⅥng an    unbalanced load. Assume star connecⅥons on both ends, work out the neutral line current analyⅥcally caused by the unbalanced load and validate it in simulaⅥon.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
