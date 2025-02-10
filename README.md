# BAE305-SP25-Lab2
# Laboratory Report for Lab 2 of BAE305 Spring 2025
# Lab 2 - For Good Measure: Basic Circuits
* By: Abby Phillips and Audrey Suit
* Submitted: February 10th, 2025


## Summary  
The objective of this lab was to analyze basic electrical circuits by applying fundamental circuit laws and theorems, including Kirchhoff’s Voltage Law (KVL), Kirchhoff’s Current Law (KCL), Thevenin’s theorem, and the superposition theorem. The lab involved constructing and analyzing both series and parallel circuits to verify theoretical predictions through experimental measurements.  

To begin, we practiced soldering techniques by assembling a simple series circuit on a solder protoboard. We then measured voltage drops and currents within the circuit using a digital multimeter (DMM) to confirm compliance with KVL and KCL. Next, we built a parallel circuit on a prototyping breadboard and measured its electrical parameters to further validate KCL. Finally, we explored Thevenin’s and Norton’s theorems by simplifying a complex circuit into its equivalent form and comparing calculated values with experimental measurements.  

Through this lab, we gained hands-on experience with circuit construction, soldering, and measurement techniques. Our results demonstrated strong agreement with theoretical expectations, reinforcing our understanding of fundamental circuit analysis principles.  

## Materials  
- Digital Multimeter (Fluke DMM)  
- DC Power Supply (DCPS)  
- Soldering Station  
- Small Piece of Solder  
- Solder Protoboard  
- Resistors:  
  - 1kΩ  
  - 2.2 kΩ (×2)  
  - 5.1 kΩ  
  - 4.7 kΩ  
  - 6.8 kΩ  
  - 15 kΩ  
  - 220 kΩ  

## Assembly Procedures  

### Part 1: Series Circuit  
Using the Fluke digital multimeter, we measured the actual resistance of the 1kΩ, 2.2 kΩ, and 5.1 kΩ resistors by attaching the multimeter leads to their terminals with alligator clips. The labeled resistance was verified using the resistor color code. After confirming the resistor values, we proceeded to construct the circuit below on a soldering breadboard. 

<img width="161" alt="image" src="https://github.com/user-attachments/assets/60e2f5c5-65c9-48bb-9d8f-2e74f1aaa390" />

We used a soldering iron to apply solder and establish connections between the resistors and the copper pad on the underside of the board. Two wires were soldered to the circuit to allow for connection to the DC power supply. Once the circuit was completed, we connected the DCPS leads to the two wires and set the voltage to 10V. Using the Fluke digital multimeter, we measured the voltage drop across each resistor by clipping the leads to each end of the resistor with alligator clips. Finally, we measured the current by interrupting the circuit with the Fluke digital multimeter to confirm the validity of Kirchhoff’s Voltage Law and Kirchhoff’s Current Law.  

### Part 2: Parallel Circuit  
Using the Fluke digital multimeter, we measured the actual resistance of the 4.7 kΩ, 6.8 kΩ, 15 kΩ, and 220 kΩ resistors following the same method used in Part 1. Next, we measured the voltage output of the DC power supply by connecting the power supply leads to the Fluke digital multimeter to ensure that the output voltage was within 0.1V of the stated value. We then constructed the parallel circuit below on a standard prototyping breadboard.

<img width="344" alt="image" src="https://github.com/user-attachments/assets/fa74c05e-a54f-407f-b128-c1ce234d6ff2" />

We then measured the current at various points in the circuit by interrupting the circuit and using the Fluke digital multimeter to record the current at each designated measurement location. These measurements were used to verify Kirchhoff’s Current Law.  

### Part 3: Thevenin Equivalent  
Using the Fluke digital multimeter, we measured the voltage drop across each resistor. To investigate Thevenin’s theorem, we removed R₅ so that I₅ would flow only through R₄ and not be split between R₄ and R₅. This setup is shown below.

<img width="259" alt="image" src="https://github.com/user-attachments/assets/01410e4d-1c44-4665-9d83-fcd639a78596" />

After modifying the circuit, we measured the voltage drop across R₄. Next, we changed the Fluke digital multimeter to current measuring mode and connected it to the terminals of R₄ to measure Iₙ by creating a short circuit. Finally, we removed the DC power supply leads from the circuit and replaced them with a single wire connecting the disconnected end of R₁ with the disconnected ends of R₃ or R₄. Using the Fluke digital multimeter as an ohmmeter, we measured the equivalent resistance Rₜₕ for the entire passive circuit, allowing us to compare our experimental results with theoretical calculations.  


# Test Equipment
1. Fluke 87 V DMM
4. DC Power Supply

# Test Procedures
1. Soldering and Verification: Learn soldering techniques by building a simple circuit on a solder protoboard
- Verify Resistor Values
  - Use the DMM in resistance mode to measure and verify the resistance of R1(1kΩ), R2(2.2kΩ), R3(5.1kΩ) to make sure they are in tolerance
- Assemble the Circuit
  - Solder the circuit as per the schematic (Figure 1) on the solder protoboard.
  - Solder wires to the terminals of R1 and R3 for power supply connection.
- Measure Circuit Parameters
  - Set the DCPS to 10VDC and connect it to the circuit.
  - Measure and record the voltage drop across each resistor(R1, R2, and R3) by attaching     
    leads on each end of the resistor
  - Measure and record the total circuit current by interrupting the circuit before R1 using the DMM in current mode.
    
2. Series and Parallel Circuit: Analyze a circuit to verify Kirchhoff’s voltage law (KVL) and Kirchhoff’s current law (KCL)
- Series Circuit: Measure Circuit Parameters of the series circuit build previously
  - Set the DCPS to 10VDC and connect it to the circuit.
  - Measure and record the voltage drop across each resistor(R1, R2, and R3) by attaching     
    leads on each end of the resistor
  - Measure and record the total circuit current by interrupting the circuit before R1 using the DMM in current mode.
- Parallel Circuit: Build the parallel circuit in Figure 2
  - Verify resistor values for R1:4.7kΩ, R2:6.8kΩ, R3:15kΩ, R4:220kΩ, and R5: 2.2kΩ
  - Verify that DCPS is within 0.1V of stated voltage (12V)
  - Measure and Record Current Values with the DMM by interrupting the circuit before each resistor
    - Verify Kirchhoff’s Current Law: the total current entering a junction must equal the total current leaving that junction (I1 = I2/3 + I4 + I5)
  - Measure and Record the voltage drops across each resistor by connecting leads on each terminal of the resistors
  - Calculate the expected voltage values using Ohm's Law (V=IR) with the currents recorded in the previous step and resistor values
    - Verify Kirchhoff’s Voltage Law (sum of voltage in a loop in a circuit equals zero).
  -Calculate power delivered by power supply and power dissipated by every resistor

3. Thevenin and Norton Equivalent Circuits: Apply Thevenin’s and superposition theorems to the analysis of electrical circuits.
  - Remove R5 from the circuit.
  - Measure the voltage across R4 (this is VTH)
  - Use DMM in DC current mode and connect to terminals of R4 (Shorts the load terminals allowing us to measure(IN))
  - Disconnect the DCPS replace with one wire joining disconnected end of R1 with disconnected ends of R3/R4
  - Measure the resistance looking back into the circuit (RTH)
  - Calculate VTH, IN, and RTH using circuit analysis and compare with measured values

# Test Results
The results obtained for step 1 of the Test Procedures are shown in the table below. All resistors were found to be in tolerance

**Resistor Value Verification Table: Series Circuit**
|Resistor|Resistance (&Omega;)|
|----------|----------|
|R1|0.981k|
|R2|2.167k|
|R3|4.997k|

The results obtained for step 2 of the Test Procedures are shown in the table below. The 22&mu;F and 102&mu;F capacitors were not in tolerance, all other capacitors were.

**Series Circuit Voltage Drop: Series Circuit**
|Resistor|Voltage Drop (V)|
|----------|----------|
|R1|1.427|
|R2|3.153|
|R3|7.27|

The results obtained for step 3 of the Test Procedures are shown in the table below. The set voltages were very close, if not exactly the same, as the measured voltages. Errors were likely due to DMM measurement since sometimes values would continue to change on the DMM after the probes were attached. This could lead to some measurement error.

**Resistor Values Table: Parallel Circuit**
|Resistor|Resistance (&Omega;)|
|----------|----------|
|R1|4.683k|
|R2|6.74k|
|R3|14.64k|
|R4|217.5k|
|R5|2.151k|

**Measured Current Table: Parallel Circuit**
|Current Label|Measured Current (mA)|
|----------|----------|
|I1|1.80|
|I2/3|0.17|
|I4|0.03|
|I5/IL|1.60|

**Voltages Comparison Table**
|Voltage|Measured Magnitude (V)|Calculated Voltages (V)|
|----------|----------|----------|
|V1|8.39|4.47|
|V2|1.094|2.84|
|V3|2.379|1.29|
|V4|3.474|0.09|

**Thevenin-Norton Equivalents Table**
||Measured Magnitude|Calculated Voltages|
|----------|----------|----------|
|V(TH)|9.56V|7.53V|
|I(N)|2.54 mA|5|
|R(TH)/R(N)|3.774k&Omega;|3.92k&Omega;|

# Discussion
Discussion Question 1: Are the measured currents in agreement with Kirchhoff’s Current Law?
Yes! I1=I2/3+I4+I5

Discussion Question 2: Compare the measured values and the calculated values. Are these in agreement with Kirchhoff’s Voltage Law?
Yes

Discussion Question 3: Calculate the power delivered by the power supply and the power dissipated by every resistor. Is the power delivered by the power supply equal to the total power dissipated?

Discussion Question 4: Using circuit analysis, calculate RTH, IN, and VTH, and compare them with the measured values. Are the calculated values in agreement with the measured values?

# Conclusion

In summary, this lab aimed to 
