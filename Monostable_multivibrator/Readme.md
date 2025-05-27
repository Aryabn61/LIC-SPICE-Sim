# Monostable multivibrator
## Aim
### Generate pulse of width 0.5ms using 555 timer IC.
## Theory
A single o/p pulse of a given width, either high or low, is produced by monostable multivibrators' sole stable state in response to an external trigger pulse. The o/p changes states at the beginning of a timing cycle due to this trigger pulse. It then stays in the second state, which is determined by the time constant of the capacitor C and resistor R, until it returns to its initial state. This state will last until another i/p signal is received. A rectangular waveform that is significantly longer can be produced by monostable multivibrators. When an external trigger pulse is applied, the waveform's leading edge increases in tandem with the trigger.  
## Working
Until it receives a trigger, the monostable multivibrator's output utilizing a 555 timer stays stable. A monostable 555 multivibrator is said to be in a stable condition when both the transistor and the capacitor are shorted. The o/p gets high when the voltage at the 555 IC's second pin drops. We refer to this high condition as a quasi-stable state. A stable state gives way to a quasi-stable state when the circuit is activated. The capacitor then begins charging to VCC when the discharge transistor is turned off. Using a time constant R1C1, the resistor R1 charges the capacitor.  Hence, the voltage of the capacitor increases and finally exceeds 2/3 Vcc, it will change the internal control flip flop, thereby turning off the 555 timer IC. Thus the o/p goes back to its stable state from an unstable state.
The Time duration of the pulse is given by
T = 1.1RC
Where, R is in Ω and C in Farads.
Finally we can conclude that, in the monostable multivibrator using 555 timer, the o/p stays in a low state until it gets a trigger i/p. This type of operation is used in push to operate systems. When the input is triggered, then the o/p will go to high state & comes back to its original state.
## Circuit Diagram:
![image](https://github.com/user-attachments/assets/f09d2014-f234-4cf1-947f-79f882f99862)
## Calculation:
Given that T=0.5ms and assume c=1uF.

T=1.1RC



R =  0.5mS/(1.1×1uF) = 454.54 Ohm.
## Procedure
1.	Build the circuit as per the Circuit diagram.
2.	Calculate the resistor R and capacitor C using the formula ton=1.1RC.
3.	In simulation we used signal generator for triggering the circuit. 
4.	Analyze the capacitor charging and discharging Voltage per time.
5.	Analyze the ton period when input is triggered. 
## Output Waveform
![image](https://github.com/user-attachments/assets/141243cc-a94a-4485-b145-532742e47138)

First waveform is triggering pulse for Monostable Multivibrator, Second waveform is Voltage across the Capacitor and Third waveform is output Pulse of 0.5ms
## Inference
•	The output of the circuit remains LOW in its stable state until a trigger input is applied.

•	Upon receiving the trigger, the output switches to HIGH and stays in that state for a time period determined by the RC time constant.

•	With the capacitor value chosen as 1 µF, the required resistor value was calculated to be approximately 454.54 Ω to achieve a 0.5 ms pulse.

•	This experiment demonstrates the use of a 555 timer in monostable mode for generating precise time delays.

## Conculsion
The 555 timer IC in monostable mode successfully generated a 0.5 ms output pulse in response to a trigger input. The output pulse duration matched the calculated value using the formula T = 1.1 × R × C, demonstrating the timer’s effectiveness in generating precise time delays.


# Simulation in Virtual Lab Astable Multivibrator
## Procedure:
1.	Connect the components as mentioned below: L1-L12, L14-L12, L16-L12, L4-L9, L8-L9, L10-L19, L3-L17, L11-L13, L7-L19, L6-L13, L2-L13, L5-L15, L18-L9.(For eg. click on 1 and then drag to 12 and so on.)
2.	Click on 'Check Connection' button to check the connections.
3.	If connected wrong, click on the wrong connection. Else click on 'Delete all connection' button to erase all the connections.
4.	Intially set R a=3.3 kΩ, R b=6.8kΩ, C=0.1µf, Vcc=5 V.
5.	Click on "Calculate" button.
6.	Now note the output voltage.
7.	Click on "Plot" button to plot Output Voltage, Capacitance Voltage
8.	Click on "Clear" button to clear the data.
9.	Repeat the experiment for another set of resistance value.
10.	Set the Resistance (Ra) value (1 kΩ - 10 kΩ).
11.	Set the Resistance (Rb) value (1 kΩ - 10 kΩ).
12.	Set the Capacitance (C) value (0.1 µf - 10 µf) .
13.	Set supply voltage (Vcc).

## Circuit Diagram
![image](https://github.com/user-attachments/assets/84bdd13c-5c06-4e09-a1a1-41ebcdcf4a6b)

## Otuput Waveform
Voltage Across the Capacitor: 
![image](https://github.com/user-attachments/assets/929fa028-39d0-47d6-bb2d-893dd75a726c)

Output Waveform: -
![image](https://github.com/user-attachments/assets/10f076e5-9dbc-4486-b668-c16dc3c2def0)

# Simulation in Virtual Lab Monostable Multivibrator
## Procedure:
1.	Connect the components as mentioned below: L1-L12, L14-L12, L16-L12, L4-L9, L8-L9, L9-L10, L3-L17, L11-L13, L7-L11, L6-L13, L5-L15.(For eg. click on 1 and then drag to 12 and so on.)
2.	Click on 'Check Connection' button to check the connections.
3.	If connected wrong, click on the wrong connection. Else click on 'Delete all connection' button to erase all the connections.
4.	Intially set R a=10 kΩ, C=1 µf, Vcc=5 V, Tin = 20 msec.
5.	Click on "Calculate" button.
6.	Now note the output voltage.
7.	Click on "Plot" button to plot, Trigger Input Voltage, Output Voltage, Capacitance Voltage
8.	Click on "Clear" button to clear the data.
9.	Repeat the experiment for another set of resistance value and capacitance value.
10.	Set the Resistance (R a) value (1 kΩ - 10 kΩ).
11.	Set the Capacitance (C) value .
12.	Set supply voltage (Vcc).
## Circuit Diagram
![image](https://github.com/user-attachments/assets/bcabfa8b-4c6d-4fd9-85b2-1ae949fdca52)

## Waveform
Triggering pulse input waveform:
![image](https://github.com/user-attachments/assets/1d22377a-19d1-4c3f-a5ac-73992f390170)

Voltage Across the Capacitor: 
![image](https://github.com/user-attachments/assets/786cee74-8f69-4528-b983-a9263b696e1f)

Output Waveform: 
![image](https://github.com/user-attachments/assets/8e9a313b-de9a-41da-a336-7ae45c7bbe49)
