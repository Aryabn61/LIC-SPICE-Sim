# **Current Mirroring Experiment**

Aim : Design and Analyze Current mirror circuit as active load in amplifier circuit.

Given :

V<sub>dd</sub>=1.8 V.\
P <=1 mW.\
A<sub>v</sub>>-10 V/V.

Circuit diagram : 

![image](https://github.com/user-attachments/assets/efbf9c25-9402-4c19-b28b-53f7f284ae52)

# **DC Analysis(1:1 ratio) :**

I<sub>Total</sub> = P/V<sub>DD</sub>\
I<sub>Total</sub> = I<sub>ref</sub> + I<sub>x</sub>\
Since the ratio is 1:1 I<sub>ref</sub> = I<sub>x</sub>\
I<sub>ref</sub> = I<sub>Total</sub>/2\
I<sub>Total</sub> = 1 mW/1.8 V\
I<sub>Total</sub> = 0.555 mA\
I<sub>ref</sub> = 0.555 m/2\
I<sub>ref</sub> = 0.2778 mA.\
In order to determine the current value based on the specified ratio, the W/L values for M1, M2, and M3 are 10um/180nm, 10um/180nm, and 10um/180nm, respectively.
Since Vin is chosen to be in the saturation range, the value that is provided is 0.6275V.\
![dc c1](https://github.com/user-attachments/assets/041df0d8-acb1-49ec-a13f-9c00fb85c60e)\
**OUTPUT :**\
![dc 11](https://github.com/user-attachments/assets/bc3c2d6f-ad95-4cbb-ae66-c9e81ee0412f)\
# **Transient Analysis :**
- Change the input voltage to sine and change the amplitude to 50 mV , frequency to 1 kHz and offset voltage to 0.6275 V.
- Click on run command.
- Select transient analysis and choose 10 ms for stop time.
- Click on ok.
  ![tc1](https://github.com/user-attachments/assets/0baf3973-db29-43a0-868e-99156c9e73da)\
**OUTPUT :**\
![t11](https://github.com/user-attachments/assets/33bff03f-ce0b-4ad7-ae89-d6887aef8a15)\
**Result :**\
  The expected gain was greater than or equal to 10 V/V and the obtained gain is 13.77 V/V.\
# **AC Analysis :**
![acc1](https://github.com/user-attachments/assets/57736abe-c8d7-4af5-8717-57b3c1940db9)\
**Procedure :**\
- Change the V<sub>in</sub> to AC and set AC amplitude to 1.
- Click on run simulation and choose AC analysis.
- Select number of points to decade , frequency range to 0.1 - 1 THz.
- Click on Ok.
**OUTPUT :**/
  ![ac1](https://github.com/user-attachments/assets/5b02d312-6042-481a-ade4-286e55a4e34a)\
  **Result :**
  The Expected gain in dB is 20 and the obtained gain is 25.23 dB.

  |Parameter    | Theory value | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 20dB         | 25.23dB         |
|Av(in V/V)     | 10           | 13.77           |
