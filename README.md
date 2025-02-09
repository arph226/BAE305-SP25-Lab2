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
1. Using the Fluke DMM, we measured the actual resistance of the 1kΩ, 2.2 kΩ, and 5.1 kΩ resistors by attaching each lead to one side of the resistors via alligator clips. The labeled resistance was verified using the resistor color code.  
2. Constructed the series circuit on a soldering breadboard.  
3. Used the soldering iron to apply solder, establishing connections between resistors and the copper pad on the underside of the board. Two wires were soldered for connection to the DC Power Supply.  
4. Connected the DCPS leads to the two wires and set the voltage to 10V.  
5. Measured the voltage drop across each resistor using the Fluke DMM, clipping each lead to each end of the resistor with alligator clips.  
6. Measured the current by interrupting the circuit with the Fluke DMM.  

### Part 2: Parallel Circuit  
1. Measured the actual resistance of the 4.7 kΩ, 6.8 kΩ, 15 kΩ, and 220 kΩ resistors using the Fluke DMM and verified values via the resistor color code.  
2. Measured the voltage output of the DCPS by connecting the power supply leads to the Fluke DMM, ensuring it was within 0.1V of the stated voltage.  
3. Assembled the parallel circuit on a standard breadboard.  
4. Measured the current at each designated point by interrupting the circuit with the Fluke DMM.  

### Part 3: Thevenin Equivalent  
1. Measured the voltage drop across each resistor using the Fluke DMM.  
2. To investigate Thevenin’s theorem, removed **R₅** so that **I₅** would only flow through **R₄** rather than splitting between **R₄** and **R₅**.  
3. Measured the voltage drop across **R₄** after modifying the circuit.  
4. Changed the Fluke DMM to current measuring mode and connected it to the terminals of **R₄**, allowing the measurement of **Iₙ** (short-circuit current).  
5. Removed the DCPS leads and replaced them with a wire joining the disconnected end of **R₁** with the disconnected ends of **R₃** or **R₄**.  
6. Used the Fluke DMM as an ohmmeter to measure the equivalent resistance (**Rₜₕ**) for the entire passive circuit.  


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
