# Experiment-1

Q: In the given below circuit find the DC operating point,Gain using transient analysis and AC analysis for different values of RD and W/L ratio.

![dc opt](https://github.com/user-attachments/assets/f3a5e0b0-b36c-4b9e-83ab-77ce82b5c2bc)

Aim : To find DC operating point,find gain using transient analysis and AC analysis.

# DC Analysis

#For RD = 1K Ω
Set the Input voltage to 0.9 V connected to the gate terminal and VDD to 1.8 V.Select 1K Ω.

Using the equation , P = VI 

ID(Drain Current) = 55µ A

Set the W/L ratio to such a way that it matches with the obtained ID value and make sure that the transistor is operating in the saturation region , i.e VDS >= Vov 

Vov = VGS - VTH

For the above ID value , the obtained W/L ratio is 500/308.

![dc3](https://github.com/user-attachments/assets/ed317ed3-6cd0-4471-8f0d-d522be2ebb4a)

To perform DC analysis select DC operating point and run the simulation.



The obtained DC operating point is (1.74 V , 55µ A).

![dc 1](https://github.com/user-attachments/assets/d3d75b10-c8e8-4850-8024-e2d208245512)

# For RD = 5K Ω

![dc21](https://github.com/user-attachments/assets/8c3287c5-7955-4e61-b5f3-7efeb8afd642)

The Obtained DC operating value is (1.52 V , 55µ A).

![dc22](https://github.com/user-attachments/assets/09936f8c-8bde-428b-8425-0c6abd105910)

# For W/L = 1µ/180n 

![dc31](https://github.com/user-attachments/assets/5df331d7-c15f-4c87-8942-ed55489feadc)

The opbtained DC operating point is (1.63 V,0.00016631 A)

![dc32](https://github.com/user-attachments/assets/dd778d5d-ad2f-478d-a523-c58f202d29f7)

# Transient Analysis

This is used to analyse the change in voltage and current over time with respect to the input signal.

Select the input voltage and change it from DC value to sine with DC offset value 0.9 V , amplitude 50m V and frequency to 1K Hz.Select Transient analysis from run command and select stop time to 5m s.

![t1](https://github.com/user-attachments/assets/47d26a58-0340-4d77-9ef7-20892cc38449)

Input waveform :

![t2](https://github.com/user-attachments/assets/9c4e42ab-a424-4c9e-8874-f1ea67fb6189)

Output waveform : 

![t3](https://github.com/user-attachments/assets/38aa10e9-43bd-4b21-9293-797ff7a2d61d)

#To Find the Gain of the Circuit

Av = Vout/Vin.

From the above graph,

Vout = 1.793 V 

Vin = 900m V

Gain(Av) = Vout/Vin

Av = 1.793/900m

Av=1.999 ≈ 2

# AC analysis

This is used to analyse the circuit with response to different frequencies.

Select the input voltage to sine and set DC offset to 0.9 V , amplitude to 50m V and frequency to 1k Hz. Select the AC amplitude to A. Then in run command select AC analysis and select the type of sweep to decade and select the number of points to 20 and operating frequency from 0.1 Hz to 1T Hz.

![ac22](https://github.com/user-attachments/assets/580bbd44-765e-44c1-8072-370635219ef7)

![t4](https://github.com/user-attachments/assets/107075fe-312c-43a3-b5aa-76bd048d0c86)

Frequency response : 

![ac21](https://github.com/user-attachments/assets/56301bff-2253-4f58-944a-67b4ee7a233f)

# Result : 

• DC operating point:-

For Rd = 1K Ω : (1.74 V , 55µ A).

For RD = 5k Ω : (1.52 V , 55µ A).

For W/L = 1µ/180n : (1.63 V,0.00016631 A).

• Transient analysis :

Gain = 2

• AC analysis : 


