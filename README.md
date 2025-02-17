# BAE305-SP25-Lab2
# Laboratory Report for Lab 2 of BAE305 Spring 2025
# Lab 2 - For Good Measure: Basic Circuits
* By: Abby Phillips and Audrey Suit
* Submitted: February 10th, 2025


## Summary  
The objective of this lab was to analyze basic electrical circuits by applying fundamental circuit laws and theorems, including Kirchhoff’s Voltage Law (KVL), Kirchhoff’s Current Law (KCL), Thevenin’s theorem, and the superposition theorem. The lab involved constructing and analyzing both series and parallel circuits to verify theoretical predictions through experimental measurements.  

To begin, we practiced soldering techniques by assembling a simple series circuit on a solder protoboard. We then measured voltage drops and currents within the circuit using a digital multimeter (DMM) to confirm compliance with KVL and KCL. Next, we built a parallel circuit on a prototyping breadboard and measured its electrical parameters to further validate KCL. Finally, we explored Thevenin’s and Norton’s theorems by simplifying a complex circuit into its equivalent form and comparing calculated values with experimental measurements.  

Through this lab, we gained hands-on experience with circuit construction, soldering, and measurement techniques. Our results demonstrated strong agreement with theoretical expectations, reinforcing our understanding of fundamental circuit analysis principles. We found the data from our circuits agreed with KCL and our power delivered by the power supply was equal to the total power dissapated. However, our circuit did not agree with KVL 

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

We used a soldering iron to apply solder and establish connections between the resistors and the copper pad on the underside of the board. 

![image](https://github.com/user-attachments/assets/7479e52d-d2fd-4928-bf8d-cbbd82384d60)

Two wires were soldered to the circuit to allow for connection to the DC power supply. Once the circuit was completed, we connected the DCPS leads to the two wires and set the voltage to 10V. Using the Fluke digital multimeter, we measured the voltage drop across each resistor by clipping the leads to each end of the resistor with alligator clips. Finally, we measured the current by interrupting the circuit with the Fluke digital multimeter to confirm the validity of Kirchhoff’s Voltage Law and Kirchhoff’s Current Law.  

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

The results obtained for step 2 of the Test Procedures are shown in the table below. The set voltages were very close, if not exactly the same, as the measured voltages. Errors were likely due to DMM measurement since sometimes values would continue to change on the DMM after the probes were attached. This could lead to some measurement error.

**Resistor Values Table: Parallel Circuit**
|Resistor|Resistance (&Omega;)|
|----------|----------|
|R1|4.683k|
|R2|6.74k|
|R3|14.64k|
|R4|217.5k|
|R5|2.151k|

The measured currents for each component of the parallel circuit in step 2 of the Test Procedures is shown in the table below. Current values agree with Kirchhoff's Current Law (KCL)
**Measured Current Table: Parallel Circuit**
|Current Label|Measured Current (mA)|
|----------|----------|
|I1|1.80|
|I2/3|0.17|
|I4|0.03|
|I5/IL|1.60|

The measured and calculated voltages for each component of the parallel circuit in step 2 of the Test Procedures is shown in the table below. Some discrepancies can be seen in voltage values, especially V4. This will be discussed in the discussion section of the lab.

**Voltages Comparison Table**
|Voltage|Measured Magnitude (V)|Calculated Voltages (V)|
|----------|----------|----------|
|V1|8.39|8.43|
|V2|1.094|1.15|
|V3|2.379|2.49|
|V4|3.474|6.6|

The measured and calculated Thevenin-Norton Equivalents for the parallel circuit in step 3 of the Test Procedures is shown in the table below. The measured and calculated magnitudes are close to one another, but there is a 2V discrepancy in the Thevenin voltage which could be due to tolerance variations in resistors or power supply variations.

**Thevenin-Norton Equivalents Table**
||Measured Magnitude|Calculated Magnitude|
|----------|----------|----------|
|V(TH)|9.56V|7.53V|
|I(N)|2.54 mA|1.92 mA|
|R(TH)/R(N)|3.774k&Omega;|3.92k&Omega;|

# Discussion
Discussion Question 1: Are the measured currents in agreement with Kirchhoff’s Current Law?
Yes, the measured currents are in agreement with Kirchhoff's Current Law which states "the algebraic sum of the currents flowing into (or out of) a node in an electrical circuit at any instant of time is zero" in the lab manual. This statement can be represented by the following equation for our circuit: I1=I2/3+I4+I5. When plugged into this equation, the measured values are in agreement with this law.

Discussion Question 2: Compare the measured values and the calculated values. Are these in agreement with Kirchhoff’s Voltage Law?
The measured values not in agreement with Kirchhoff's Voltage law which states, "the algebraic sum of the voltage drops across circuit elements around any closed loop in an electrical circuit at any instant of time is zero." This can be represented by the equation: Vin=V1+V2+V3+V4. When we plug in our measured values to this equation, we get that the sum of voltages is about equal to 15.3V, which does not equal the voltage into the circuit, meaning they are not in agreement with Kirchhoff's Voltage Law. Our calculated values based on the measured current add to 18 V which is a more significant discrepancy. This could be due to discrepancies in current or voltage measurements or tolerances of circuit components.


Discussion Question 3: Calculate the power delivered by the power supply and the power dissipated by every resistor. Is the power delivered by the power supply equal to the total power dissipated?

The power delivered can be calculated by the equation P=V^2/Req, or P=144V/6680&Omega;= 0.0216W= 21.6mW. The power dissipated by each resistor is calculated by P=IV using above voltage and current measurements.
| **Resistor** | **Power Dissipated (W)** |
|-------------|------------------------|
| R1          | 0.01517 W             |
| R2          | 0.0001948 W           |
| R3          | 0.0004231 W           |
| R4          | 0.0001958 W           |
| R5          | 0.0055 W           |

Total Calculated Power Dissipated= 0.0214W= 21.5mW. The power delivered by the power supply is about equal to the total power dissipated by the circuit. 

Discussion Question 4: Using circuit analysis, calculate RTH, IN, and VTH, and compare them with the measured values. Are the calculated values in agreement with the measured values?

As seen in the Thevenin-Norton Equivalents table above, the calculated values for RTH and IN are very similar. The Vth calculated value is 2V off from the measured value, which could be the result of tolerance variations in resistors, power supply variations or wiring losses from solder joints.

# Conclusion

In summary, this lab aimed to apply fundamental circuit laws and theorems such as Kirchhoff's Voltage and Current Laws (KVL and KCL), Thevenin, Norton, and superposition. To analyze basic electrical circuits using these laws and theorems we constructed a series circuit via soldering and a parallel circuit to compare theoretical predictions with measured values. We utilized the Fluke DMM for measurements and became familiar with the solder protoboard for constructing the circuit. By measuring a variety of values such as current, resistance, and voltage, and using simplification techniques such as Thevenin-Norton analysis, we gained hands on experience in analyzing circuits. We found that the data from our circuits were in agreement with KCL and the power dissipated was equivalent to the power delivered the power supply. However, there were slight discrepancies with KVL and Thevenin-Norton equivalencies, possibly due to measurement errors or component tolerances. Possible improvements, such as stable contact with DMM leads to avoid fluctuating readings and improving soldering technique to prevent innacuracies, can be made for better results in future experimentation.
