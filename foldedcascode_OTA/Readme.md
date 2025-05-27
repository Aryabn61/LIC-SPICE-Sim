
# Folded Cascode OTA
## Introduction
ADCs, filters, and signal processing systems all commonly include operational transconductance amplifiers (OTAs), which are crucial components of analog circuit design.  The Folded Cascode OTA is distinct from other OTA architectures because to its wide output swing, high gain, and tiny single-stage construction.  Unlike typical cascode amplifiers, which have restricted voltage swing due to stacked transistors, the folded cascode topology enhances headroom by folding the current route of the input differential pair across a complimentary branch.  This study presents the design, theoretical analysis, and modeling of a Folded Cascode OTA.  The performance advantages of this design are demonstrated through the use of LTspice, DC, AC, transient, and noise simulations.  The results confirm that a better trade-off is achieved by the folded cascode design.

## Working Methodology
By combining differential input processing with cascode current mirroring, the folded cascode operational transconductance amplifier (OTA) used in this design provides high gain and enhanced voltage swing.  The NMOS transistor M11 serves as a tail current source, supplying a steady bias current to the input stage, which is made up of NMOS transistors M9 and M10 arranged as a differential pair.  The distribution of this bias current is modulated by the differential voltage that is applied between the gates of M9 and M10.  The signal is transferred to the upper half of the circuit by the NMOS cascode transistors (M6 and M5), which route the resultant currents upward and fold them into the drains of PMOS transistors (M4 and M3).The PMOS transistors M1 and M2 form a cascode current mirror that senses these variations and generates a single-ended output voltage at the node Vout.
To enhance gain, NMOS cascode devices (M6–M8) are used to increase the output impedance. Bias voltages Vb, Vc, and Vd are applied to maintain all       MOSFETs in saturation, ensuring linear operation and optimal transconductance. Vb sets the operating point for the PMOS cascode devices, Vc biases the NMOS cascode transistors, and Vd establishes the current in the differential pair's tail source. Additionally, a load capacitor C1 at the output node introduces a dominant pole, defining the amplifier's bandwidth and contributing to its frequency stability. This folded cascode configuration enables a wide input/output voltage swing and high DC gain while maintaining power efficiency, making it highly suitable for low-voltage, high-speed analog applications.

## Circuit Diagram

![IMG-20250516-WA0054](https://github.com/user-attachments/assets/b3de5cb8-6c39-42f2-b3ac-e7ac56b77438)

## Technical Specification
•	Voltage Gain (Av): 60–75 dB .



•	Unity Gain Bandwidth (UGB): ~80 MHz




•	Power Consumption: ~36 µW .




•	Load Capacitance: 0.1 pF – 1 pF (external compensation capacitor).





•	Input-Referred Offset Voltage: < 5 mV .





•	Common-Mode Rejection Ratio (CMRR): > 60 dB .





•	Power Supply Rejection Ratio: > 60 dB .





•	Noise Performance: Input-referred noise dominated by M9/M10 pair.

## Advantages
•	High Voltage Gain




•	Wide Bandwidth



•	Stable Operation



•	Low Power Consumption



•	Low Noise




•	Low Offset Voltage




•	Good Common-Mode and Power Supply Rejection




•	Compact Load Capacitance Range




## Simulation Result


Input wave


![image](https://github.com/user-attachments/assets/2080b442-8361-4bdb-80bf-20ecc91faa26)



Transient Analysis output:


![IMG-20250517-WA0004](https://github.com/user-attachments/assets/f1ca426b-a9dc-4161-b932-682ce5c09509)




DC Analysis Output: 



![image](https://github.com/user-attachments/assets/cf92a448-c275-4c32-a094-4533e3b1b470)



Ac Analysis Output:

![IMG-20250517-WA0004](https://github.com/user-attachments/assets/9dc4cf19-8dd7-4f90-b0ef-f20b7369ea03)



## Inference
The folded cascode OTA described offers  excellent performance with high voltage gain, wide bandwidth, and stability, making it ideal for low-power, precision applications. Its low noise, minimal offset voltage, and strong immunity to common-mode and power supply noise enhance its reliability and accuracy. The flexibility in handling different load capacitances and the efficient power consumption further make it suitable for integrated circuit designs that require high performance and low energy usage

## Conclusion
The folded cascode OTA with the specified characteristics provides a robust solution for high-gain, low-noise amplification in applications requiring precise signal processing. Its low power consumption, high bandwidth, and stability across varying load capacitances make it an ideal choice for energy-efficient integrated circuits. The low offset voltage and strong rejection of common-mode and power supply noise further enhance its reliability, ensuring accurate and consistent performance in practical scenarios.

## REFERENCE
•	Design of Analog CMOS Integrated Circuits Book by - Behzad Razavi


•	https://peopke.engr.tamu.edu/spalermo/ecen474/lecture14_ee474_folded_cascode_ota.pdf


•	https://www.researchgate.net/figure/Basic-folded-cascode-operational-amplifier_fig1_338486493



## 9. Contributors

- Arya B N (USN: 4NI23ec015)
- Disha N B (USN: 4N23EC028)  
