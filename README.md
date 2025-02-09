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
Using the Fluke digital multimeter, we measured the actual resistance of the 1kΩ, 2.2 kΩ, and 5.1 kΩ resistors by attaching the multimeter leads to their terminals with alligator clips. The labeled resistance was verified using the resistor color code. After confirming the resistor values, we proceeded to construct the circuit on a soldering breadboard. We used a soldering iron to apply solder and establish connections between the resistors and the copper pad on the underside of the board. Two wires were soldered to the circuit to allow for connection to the DC power supply. Once the circuit was completed, we connected the DCPS leads to the two wires and set the voltage to 10V. Using the Fluke digital multimeter, we measured the voltage drop across each resistor by clipping the leads to each end of the resistor with alligator clips. Finally, we measured the current by interrupting the circuit with the Fluke digital multimeter to confirm the validity of Kirchhoff’s Voltage Law and Kirchhoff’s Current Law.  

### Part 2: Parallel Circuit  
Using the Fluke digital multimeter, we measured the actual resistance of the 4.7 kΩ, 6.8 kΩ, 15 kΩ, and 220 kΩ resistors following the same method used in Part 1. Next, we measured the voltage output of the DC power supply by connecting the power supply leads to the Fluke digital multimeter to ensure that the output voltage was within 0.1V of the stated value. We then constructed the parallel circuit on a standard prototyping breadboard and measured the current at various points in the circuit by interrupting the circuit and using the Fluke digital multimeter to record the current at each designated measurement location. These measurements were used to verify Kirchhoff’s Current Law.  

### Part 3: Thevenin Equivalent  
Using the Fluke digital multimeter, we measured the voltage drop across each resistor. To investigate Thevenin’s theorem, we removed R₅ so that I₅ would flow only through R₄ and not be split between R₄ and R₅. After modifying the circuit, we measured the voltage drop across R₄. Next, we changed the Fluke digital multimeter to current measuring mode and connected it to the terminals of R₄ to measure Iₙ by creating a short circuit. Finally, we removed the DC power supply leads from the circuit and replaced them with a single wire connecting the disconnected end of R₁ with the disconnected ends of R₃ or R₄. Using the Fluke digital multimeter as an ohmmeter, we measured the equivalent resistance Rₜₕ for the entire passive circuit, allowing us to compare our experimental results with theoretical calculations.  



# Test Equipment
1. Fluke 87 V DMM
4. DC Power Supply

# Test Procedures


# Test Results
The results obtained for step 1 of the Test Procedures are shown in the table below. All resistors were found to be in tolerance

**Resistor Values Table**
|Color Code|Expected Value (&Omega;)|Tolerance(%)|Measured Value (&Omega;)|Within Tolerance|
|----------|----------|----------|----------|----------|
|Brown Black Blue|10M|5|10.25M|yes|
|Orange Orange Red|3.3k|5|3.297k|yes|
|Brown Green Brown|750|5|749.9|Yes|
|Red Red Gold|2.2|5|2.3|yes|

The results obtained for step 2 of the Test Procedures are shown in the table below. The 22&mu;F and 102&mu;F capacitors were not in tolerance, all other capacitors were.

**Capacitor Values Table**
|Expected Value (&mu;F)|Tolerance(%)|Measured Value (&mu;F)|Within Tolerance|
|----------|----------|----------|----------|
|10|20|10.44|Yes|
|1|10|1.1|Yes|
|102|10|1.34|No|
|22|5|6.36|No|

The results obtained for step 3 of the Test Procedures are shown in the table below. The set voltages were very close, if not exactly the same, as the measured voltages. Errors were likely due to DMM measurement since sometimes values would continue to change on the DMM after the probes were attached. This could lead to some measurement error.

**DC Power Source Voltage Output Table**
|Set Voltage (V)|Measured Voltage (V)|
|----------|----------|
|1.56|1.494|
|7.00|7.00|
|12.00|12.01|
|3.3|3.389|

**Function Generator Output Table**
|Measurement Method|Frequency (kHz)|Amplitude (V)|
|----------|----------|----------|
|Cursors|4.81|5.04|
|Counting Squares|5|5|
|Measurement Features|4.66|5.25|
|Fluke DMM|4.66|0.126|


# Discussion


# Conclusion

In summary, this lab aimed to 
