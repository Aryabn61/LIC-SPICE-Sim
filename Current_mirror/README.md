# **Current Mirroring Experiment**

Aim : Design and Analyze Current mirror circuit as active load in amplifier circuit.

Given :

V<sub>dd</sub>=1.8 V.\
P <=1 mW.\
A<sub>v</sub>>-10 V/V.

Circuit diagram : 

![image](https://github.com/user-attachments/assets/efbf9c25-9402-4c19-b28b-53f7f284ae52)

# FOR L = 180 nm
# **1:1 Ratio :**
# **DC Analysis:**

The drain current with channel length modulation is expressed as:\
I<sub>D</sub> = (1/2)μnC<sub>ox</sub>(W/L)(VGS - Vth)^2\
I<sub>Total</sub> = P/V<sub>DD</sub>\
I<sub>Total</sub> = I<sub>ref</sub> + I<sub>x</sub>\
Since the ratio is 1:1 I<sub>ref</sub> = I<sub>x</sub>\
I<sub>ref</sub> = I<sub>Total</sub>/2\
I<sub>Total</sub> = 1 mW/1.8 V\
I<sub>Total</sub> = 0.555 mA\
I<sub>ref</sub> = 0.555 m/2\
I<sub>ref</sub> = 0.2778 mA.\
For matched transistors in a 1:1 ratio:\
W1/L1 = W2/L2\
In order to determine the current value based on the specified ratio, the W/L values for M1, M2, and M3 are 10	µm/180nm, 10	µm/180nm, and 10	µm/180nm, respectively.
Since Vin is chosen to be in the saturation range, the value that is provided is 0.6275V.\
![dcc1](https://github.com/user-attachments/assets/95e36a79-88c3-475e-9337-1e2d8a0cadc5)
**OUTPUT :**
![dc1](https://github.com/user-attachments/assets/0bef1396-cc00-4844-af59-bd3e28b1a31e)
# **Transient Analysis :**
- Change the input voltage to sine and change the amplitude to 50 mV , frequency to 1 kHz and offset voltage to 0.6275 V.
- Click on run command.
- Select transient analysis and choose 10 ms for stop time.
- Click on ok.
![trc1](https://github.com/user-attachments/assets/4172d700-db34-4a56-8582-af6e871d451f)
**OUTPUT :**
![tc1](https://github.com/user-attachments/assets/278d9154-94ae-4060-a1df-3b9e31824269)
**Result :**\
  The expected gain was greater than or equal to 10 V/V and the obtained gain is 13.77 V/V.\
# **AC Analysis :**
![acc1](https://github.com/user-attachments/assets/fc6a349b-eb4c-4595-b5ef-d1a30ee1e57a)
**Procedure :**
- Change the V<sub>in</sub> to AC and set AC amplitude to 1.
- Click on run simulation and choose AC analysis.
- Select type of sweep to decade , frequency range to 0.1 - 1 THz.
- Click on Ok.
**OUTPUT :**
![ac1](https://github.com/user-attachments/assets/b62e9885-1f53-4750-aecd-938eb7307f74)
  **Result :**
  The Expected gain in dB is 20 and the obtained gain is 26.23 dB.

|  Parameter    | Theory value | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 20dB         | 26.23dB         |
|Av(in V/V)     | 10           | 13.77           |

# **1:2 Ratio :**

# **DC Analysis :**
![dcc1](https://github.com/user-attachments/assets/9563e1fd-256d-4e39-a258-cc066a7b8ea8)

I<sub>ref</sub> = 0.185 mA.
In order to determine the current value based on the specified ratio, the W/L values for  M2 and M3 are 6	µm/180nm and 6	µm/180nm, nd M1 is 3	µm/180nm respectively. Since Vin is chosen to be in the saturation range, the value that is provided is 0.763 V.
**OUTPUT :**
![dc1](https://github.com/user-attachments/assets/e5b6ec50-aabb-4064-b76d-25a4b68014cd)

# **Transient Analysis :**
![trcc1](https://github.com/user-attachments/assets/e3cba872-2513-454a-b176-d6a62736028f)
- Change the input voltage to sine and change the amplitude to 50 mV , frequency to 1 kHz and offset voltage to 0.763 V.
- Click on run command.
- Select transient analysis and choose 10 ms for stop time.
- Click on ok.
**OUTPUT :**
![tr1](https://github.com/user-attachments/assets/ebc5946d-fc20-4bdf-bb98-9c7732ee3523)
**Result :**\
  The expected gain was greater than or equal to 10 V/V and the obtained gain is 12.11 V/V.\
# **AC Analysis :**
![acc1](https://github.com/user-attachments/assets/877ded48-bcea-470e-84e5-f4cc3dd7fab3)
**Procedure :**
- Change the V<sub>in</sub> to AC and set AC amplitude to 1.
- Click on run simulation and choose AC analysis.
- Select type of sweep to decade , frequency range to 0.1 - 1 THz.
- Click on Ok.
**OUTPUT :**
![ac1](https://github.com/user-attachments/assets/fdf6b91c-cbf0-4527-baed-000313b8488a)

|  Parameter    | Theory value | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 20dB         | 25.57dB         |
|Av(in V/V)     | 10           | 12.11           |

# **1:3 Ratio :**

# **DC Analysis :**
![dcc1](https://github.com/user-attachments/assets/657a9148-6e8e-40ba-827e-a6330b54645d)

I<sub>ref</sub> = 0.13875 mA.
In order to determine the current value based on the specified ratio, the W/L values for  M2 and M3 are 9	µm/180nm and 9	µm/180nm, nd M1 is 3	µm/180nm respectively. Since Vin is chosen to be in the saturation range, the value that is provided is 0.8566 V.

![dc1](https://github.com/user-attachments/assets/14391144-8b51-403c-9b9c-5363a40fdfd3)

# **Transient Analysis :**
![trcc1](https://github.com/user-attachments/assets/13678852-1123-4151-950b-cec60bf80b77)
- Change the input voltage to sine and change the amplitude to 50 mV , frequency to 1 kHz and offset voltage to 0.8566 V.
- Click on run command.
- Select transient analysis and choose 10 ms for stop time.
- Click on ok.
**OUTPUT :**
![tr1](https://github.com/user-attachments/assets/66b97c0a-8b8d-41b1-8ee3-7d4b9987d403)
**Result :**\
  The expected gain was greater than or equal to 10 V/V and the obtained gain is 13.167 V/V.\
# **AC Analysis :**

![acc1](https://github.com/user-attachments/assets/75d335b9-82e0-4163-b028-5962f52e496a)
**Procedure :**
- Change the V<sub>in</sub> to AC and set AC amplitude to 1.
- Click on run simulation and choose AC analysis.
- Select type of sweep to decade , frequency range to 0.1 - 1 THz.
- Click on Ok.
**OUTPUT :**
![ac1](https://github.com/user-attachments/assets/a796e1a0-fe17-4325-8314-fa81e533276c)

|  Parameter    | Theory value | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 20dB         | 24.85dB         |
|Av(in V/V)     | 10           | 13.167          |

# **1:5 Ratio :**

# **DC Analysis :**
I<sub>ref</sub> = 0.0925 mA.
In order to determine the current value based on the specified ratio, the W/L values for  M2 and M3 are 6	µm/180nm and 6	µm/180nm, nd M1 is 3	µm/180nm respectively. Since Vin is chosen to be in the saturation range, the value that is provided is 0.6875 V.
**OUTPUT :**
![dc1](https://github.com/user-attachments/assets/91a844e7-a3b3-473c-83f3-fac221a78bc3)
# **Transient Analysis :**

- Change the input voltage to sine and change the amplitude to 50 mV , frequency to 1 kHz and offset voltage to 0.6875 V.
- Click on run command.
- Select transient analysis and choose 10 ms for stop time.
- Click on ok.
**OUTPUT :**
![tr1](https://github.com/user-attachments/assets/2ef6931e-dc4d-488e-b02b-1af88d0cb6a6)
  **Result :**\
  The expected gain was greater than or equal to 10 V/V and the obtained gain is 14.031 V/V.\
# **AC Analysis :**
**Procedure :**
- Change the V<sub>in</sub> to AC and set AC amplitude to 1.
- Click on run simulation and choose AC analysis.
- Select type of sweep to decade , frequency range to 0.1 - 1 THz.
- Click on Ok.
**OUTPUT :**
![ac1](https://github.com/user-attachments/assets/21caed29-4972-4228-a44b-629a20eee195)

|  Parameter    | Theory value | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 20dB         | 27.14dB         |
|Av(in V/V)     | 10           | 14.031          |

# **2:1 Ratio :**

# **DC Analysis :**
![DCC1](https://github.com/user-attachments/assets/1ee6e807-99c9-4bf1-b38f-3162a2501d20)

I<sub>ref</sub> = 0.555 mA.
In order to determine the current value based on the specified ratio, the W/L values for  M2 and M3 are 6	µm/180nm and 6	µm/180nm, nd M1 is 3	µm/180nm respectively. Since Vin is chosen to be in the saturation range, the value that is provided is 0.835 V.
**OUTPUT :**
![dc1](https://github.com/user-attachments/assets/039c929e-0470-4648-b702-7cdb043c13ff)

# **Transient Analysis :**
- Change the input voltage to sine and change the amplitude to 50 mV , frequency to 1 kHz and offset voltage to 0.835 V.
- Click on run command.
- Select transient analysis and choose 10 ms for stop time.
- Click on ok.
**OUTPUT :**
![trc1](https://github.com/user-attachments/assets/89c62e7f-6b43-49a7-9aaf-45e3e4ea3011)
**Result :**\
  The expected gain was greater than or equal to 10 V/V and the obtained gain is 9.86 V/V.\
![tr1](https://github.com/user-attachments/assets/8e59821b-e57c-4a08-aecd-32e599f39b43)

# **AC Analysis :**

![acc1](https://github.com/user-attachments/assets/53798423-ba56-49fc-a3f9-f72c5ad40959)
**Procedure :**
- Change the V<sub>in</sub> to AC and set AC amplitude to 1.
- Click on run simulation and choose AC analysis.
- Select type of sweep to decade , frequency range to 0.1 - 1 THz.
- Click on Ok.
**OUTPUT :**
![ac1](https://github.com/user-attachments/assets/898cb03f-d52c-4f18-b78b-82a2a19e34e9)

|  Parameter    | Theory value | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 20dB         | 22.53dB         |
|Av(in V/V)     | 10           | 9.86            |

# FOR L = 500 nm

|Ratio|  Av(in dB)    | Av(in V/V) | 
|-----|---------------|------------|
|1:1  |11.15          |14.9        |    
|1:2  |12.85          |16.31       |   
|1:3  |11.01          |14.35       |
|2:1  |9.789          |19.83       |

# FOR L = 1 	µm

|Ratio|  Av(in dB)    | Av(in V/V) | 
|-----|---------------|------------|
|1:1  |12.60          |15.3        |    
|1:2  |9.55           |15.98       |   
|1:3  |10.95          |16.13       |
|2:1  |12.56          |16.87       |
# **Inference :**

The current mirror circuit accurately copies the reference current with very little variation, ensuring reliable current mirroring across different W/L ratios.  

Even when the W/L ratio changes while keeping the same proportion, the drain current (Id) stays nearly the same, confirming the circuit's effectiveness.  

The amplifier gain is slightly higher than expected due to small differences in transistor properties or minor simulation effects.  

When the mirror ratio increases (from 1:1 to 1:2), the gain also increases as expected.

Overall, the results closely match theoretical predictions, proving that the simulation and circuit design are working correctly.

# **PART B** 

**Aim :**
Design the differential amplifier using the same design specification as Experiment-3. Perform DC analysis,trasient and AC analysis.

# **DC Analysis :**

![dcc1](https://github.com/user-attachments/assets/933f5ad7-7907-4834-ac74-a83421925e9a)

**OUTPUT :**

![dc1](https://github.com/user-attachments/assets/e7b2ce77-6b16-4642-8f28-1f2b8abb0af6)

# **Transient Analysis :**

![trc1](https://github.com/user-attachments/assets/806bb9a2-05e1-4271-9012-304c229d22f4)

**OUTPUT :**

![a3](https://github.com/user-attachments/assets/b9e84eb5-4cba-404f-b093-b96f7067e975)

# **AC Analysis :**

![acc1](https://github.com/user-attachments/assets/14927e62-b634-450d-ba6d-885af7174ba9)

**OUTPUT :**

![ac1](https://github.com/user-attachments/assets/fe854a5b-b352-4d8a-8644-59ea5d78264a)

# **Inference :**
The circuit operates as a differential amplifier based on a current mirror, with the output (Vout) being controlled by the difference between V2 and V3.Stable current replication is guaranteed by the PMOS current mirror (M1-M2).This circuit is helpful for signal processing and amplification in analog designs because it uses the NMOS differential pair (M3-M4) for amplification.
