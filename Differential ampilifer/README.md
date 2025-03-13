# **Differential Amplifier**

# Aim

Design and analyse the MOS differentual amplifier circuit and perform DC analysis , transient analysis and frequency response for the following specifications : 

- Supply voltage(V<sub>DD</sub>) = 2.2 V
- Output common mode voltage(V<sub>ocm</sub>) = 1.25 V
- Power(P) <= 2.2 mW
- Common mode input voltage (V<sub>icm</sub>) = 1.2 V
-  Voltage at point P(V<sub>p</sub>) = 0.4 V

# **Cirucit 1**

  - Resistor loaded differential pair


![dc circuit](https://github.com/user-attachments/assets/913cdd77-451c-4afc-ba46-a4968a4ceeed)

The above given crcuit is a NMOS differential amplifier circuit which consists of two NMOS transistors which is designed as differential pair . The NMOS transistors(M1 and M2) act as the differential pair that amplifies the difference between the two input signal and the output are taken from Vout.

**Design**

Calculations : 
- **Determine I<sub>ss (Source current) :**

   I<sub>ss</sub> = Power/V<sub>DD</sub>
  
   I<sub>ss</sub> = 2.2 mW/ 2.2 V = 1 mA
  
   Therefore , I<sub>D1</sub> = I<sub>D2</sub> = 0.5 mA.

- **Finding R<sub>ss :**

  R<sub>ss</sub> = V<sub>p</sub> / I<sub>ss</sub>
  R<sub>ss</sub> = 0.4/1 m = 0.4 kΩ

- **Finding R<sub>D :**

  Using the equation , V<sub>DD</sub> = I<sub>D</sub>R<sub>D</sub> + v<sub>ocm</sub>

  R<sub>D</sub> = (V<sub>DD</sub> - V<sub>ocm</sub>)/I<sub>D</sub>

  R<sub>D</sub> = (2.2-1.25)/0.5 m = 1.9 kΩ

# **DC Analysis :**

![dc circuit](https://github.com/user-attachments/assets/29f2dac0-9353-4cd9-8ba0-a75745d2dca9)


- Make the circuit as shown above.
- Set the R<sub>D</sub> and R<sub>ss</sub> values as determined by the calculation.
- Vary W/L ratio of both the transistor to get the required V<sub>ocm</sub> and I<sub>S</sub>.
- Set the W/L ratio in such a way that the values are same fot both the transistors.
- Check the V<sub>GS</sub> and V<sub>DS</sub> value of the transistors such that it operates in saturation region.
- **Condtion for saturation region :**

  V<sub>GS</sub>>V<sub>TH</sub> ,

  V<sub>DS</sub>>V<sub>ov</sub>

![1](https://github.com/user-attachments/assets/45366000-4fe9-4b33-9b4e-afab52c4988b)

![DC values](https://github.com/user-attachments/assets/d8582160-521b-438b-a04c-b4c22d3f921f)

- Calculate V<sub>incm(min)</sub>,V<sub>incim(max)</sub>,V<sub>out(min)</sub>,V<sub>out(max)</sub>.

  V<sub>incm(min)</sub> = V<sub>TH</sub> + V,sub>p</sub>
  
  V<sub>incm<min)</sub> = 0.366 + 0.4 = 0.766 V.

  V<sub>incm(max)</sub> = V<sub>DD</sub> - (I<sub>D</sub>R<sub>D</sub>) + V<sub>TH</sub>

  V<sub>incm(max)</sub> = 1.616 V.

  # **Transient Analysis :**

![tran cir](https://github.com/user-attachments/assets/b87beb73-38e5-43a0-b38f-1aaed388f55f)

  Theoretical gain of the circuit is ,

  A<sub>v</sub> = -G<sub>m</sub>R<sub>D</sub>

  where G<sub>m</sub> = (2I<sub>D</sub>)/V<sub>ov</sub>

  G<sub>m</sub>= 2.27 mS.

  A<sub>v</sub> = -4.31 V/V.

  **Procedure :**

 - Change the DC input to AC signal.
 - Use SINE function in advanced.
 - Enter the values of DC offset , amplitude,frequency.
 - Then click on run command.
 - Choose "Transient".
 - Set stop time to 10ms and click ok.

![trans 1 final](https://github.com/user-attachments/assets/8ac30538-66a2-4d87-ad56-a20a56f694da)

**Transient analysis for V<sub>incm(min)</sub> = 0.766 V**

![trans 1 vincmmin final](https://github.com/user-attachments/assets/6d669e1c-70f5-4a9e-a21b-70f556f167ef)

**Transient analysis for V<sub>incm(man)</sub> = 1.616 V**

![trans 1 vincmmax final](https://github.com/user-attachments/assets/73a49fbd-d957-41c9-8db9-4827bcf9e0e2)

# **AC Analysis :**

![ac cir](https://github.com/user-attachments/assets/113e8933-adc4-4ca9-863c-9d24314a7482)

**Procedure :**
- In voltage source select advanced and set the AC amplitude of M1 transistor to 1 ans M2 transistor to -1.
- In simulation tab select AC Analysis.
- Then select **Type of Sweep as Decade**.
- Select the frequency range from 0.1 Hz to 1 THz.
- The obtained **differential gain is  13.12 dB**.
- 3dB Bandwidth is .

![AC1](https://github.com/user-attachments/assets/ff9d4273-a2f3-4899-8c86-17337a12b7de)


|Parameter      |Theory value  | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 12.68 dB     | 13.12 dB        |
|Av(in V/V)     | 4.31         | 4.52            |

# **Circuit 2**

- **Current source loaded differential amplifier pair**

 This is a differential amplifier built using two transistors and a current source. Both the transistor should have same W/L values to obtain a differential pair. This circuit improves Common Mode Rejection Ratio(CMRR) and high gain.

![c2](https://github.com/user-attachments/assets/ede5ecf1-dbe6-4af6-b67e-6aad8247b08b)

# **DC Analysis :**

- Make the circuit as shown above.
- Set the R<sub>D</sub> and R<sub>ss</sub> values as determined by the calculation.
- Vary W/L ratio of both the transistor to get the required V<sub>ocm</sub> and I<sub>S</sub>.
- Set the W/L ratio in such a way that the values are same fot both the transistors.
- Check the V<sub>GS</sub> and V<sub>DS</sub> value of the transistors such that it operates in saturation region.
- **Condtion for saturation region :**

  V<sub>GS</sub>>V<sub>TH</sub> ,

  V<sub>DS</sub>>V<sub>ov</sub>
  
![dc c2](https://github.com/user-attachments/assets/9cc45ea1-b3ce-4010-8d37-42ccdddea163)

# **Transient Analysis :**

 **Procedure :**

 - Change the DC input to AC signal.
 - Use SINE function in advanced.
 - Enter the values of DC offset , amplitude,frequency.
 - Then click on run command.
 - Choose "Transient".
 - Set stop time to 10ms and click ok.
   
![c2 trans](https://github.com/user-attachments/assets/251395c7-126b-4fa6-821e-2c5537948282)

![trans c2](https://github.com/user-attachments/assets/0406661a-e882-411c-b3a9-76b826e3a98c)

   A<sub>v</sub> = -4.38 V/V.
   
# **AC Analysis :**

**Procedure :**
- In voltage source select advanced and set the AC amplitude of M1 transistor to 1 ans M2 transistor to -1.
- In simulation tab select AC Analysis.
- Then select **Type of Sweep as Decade**.
- Select the frequency range from 0.1 Hz to 1 THz.
- The obtained **differential gain is  13.19 dB**.
  
![c2 ac](https://github.com/user-attachments/assets/0ee2776f-8175-4307-8276-6394fc7d7f3a)

![ac c2](https://github.com/user-attachments/assets/59bd2fa2-9f49-421d-9889-c8e086fee86a)


|Parameter      |Theory value  | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 12.82 dB     | 13.19 dB        |
|Av(in V/V)     | 4.38         | 4.56            |
# **Circuit 3**

**MOSFET loaded differential amplifier pair**

A MOSFET-loaded differential amplifier is an advanced version of a differential pair where active MOSFETs replace resistive loads to improve gain, linearity, and performance.Connect the MOSFET at V<sub>p</sub> and the W/L value of the MOSFET should be same as M1 and M2.

![c3](https://github.com/user-attachments/assets/e42b2caf-f4d4-48c2-a0e1-aeea6327ed34)

# **DC Analysis :**

W.K.T

V<sub>DS</sub> = V<sub>GS</sub> - V<sub>TH</sub> ( V<sub>DS</sub> = V<sub>p</sub> = 0.4 V )

0.4 + 0.36624 = V<sub>G</sub> ( since source is grounded )

V<sub>bias</sub> = V<sub>G</sub> = 0.76624 V ( Bias voltage at the gate for 3rd n type mosfet)

- Make the circuit as shown above.
- Set the R<sub>D</sub> and R<sub>ss</sub> values as determined by the calculation.
- Vary W/L ratio of both the transistor to get the required V<sub>ocm</sub> and I<sub>S</sub>.
- Set the W/L ratio in such a way that the values are same fot both the transistors.
- Check the V<sub>GS</sub> and V<sub>DS</sub> value of the transistors such that it operates in saturation region.
- **Condtion for saturation region :**

  V<sub>GS</sub>>V<sub>TH</sub> ,

  V<sub>DS</sub>>V<sub>ov</sub>
  
![dc c3](https://github.com/user-attachments/assets/a045c11a-c8f9-4dd2-be82-a9ea4110acb6)

# **Transient Analysis :**

 - Change the DC input to AC signal.
 - Use SINE function in advanced.
 - Enter the values of DC offset , amplitude,frequency.
 - Then click on run command.
 - Choose "Transient".
 - Set stop time to 10ms and click ok.
   
![c3 trans](https://github.com/user-attachments/assets/b81d5715-947f-411b-97e7-73fb5dc0aeb5)

![trans c3](https://github.com/user-attachments/assets/18113f7e-66b4-45dd-a4cc-b70c64269f61)

  A<sub>v</sub> = -4.33 V/V.
  
# **AC Analysis :**

**Procedure :**
- In voltage source select advanced and set the AC amplitude of M1 transistor to 1 ans M2 transistor to -1.
- In simulation tab select AC Analysis.
- Then select **Type of Sweep as Decade**.
- Select the frequency range from 0.1 Hz to 1 THz.
- The obtained **differential gain is  13.25**.
    
![c3 ac](https://github.com/user-attachments/assets/28a92e2a-950e-4680-9b14-059ed9d60063)

![ac c3](https://github.com/user-attachments/assets/df6b2f1b-81ec-4f31-bd89-b0bce11d4286)


|Parameter      |Theory value  | Practical value |
|---------------|--------------|-----------------|
|Av(in dB)      | 12.72 dB     | 13.25 dB        |
|Av(in V/V)     | 4.33         | 4.59            |
# **Final Result**

| **Parameter** | **Circuit 1** | **Circuit 2** | **Circuit 3** |
|--------------|--------------|--------------|--------------|
| **V(out1)**  | 1.25V  | 1.25V  | 1.8V  |
| **V(out2)**  | 1.25V  | 1.25V  | 1.8V  |
| **V(vp)** | 0.400141V | 0.480819V | 0.400143V |
| **Id(M1)** | 0.5 mA | 0.5 mA | 0.51 mA |
| **Id(M2)** | -0.5 mA | -0.5 mA | -0.51 mA |
| **Id(M3) (Tail Current Source)** | Not present | 1 mA (set with ideal current source) | 3.99 mA |
| **Total Tail Current** | 1.13 mA | 1 mA | 3.99 mA |

# **Inference :**

The behavior of a differential amplifier with three distinct load configurations—resistor, current source, and NMOS—was investigated in this experiment. The performance of the amplifier is impacted differently by each configuration, particularly with regard to stability and voltage gain.

## Comparison of Differential Pair Circuits

| Feature               | **Circuit 1**                  | **Circuit 2**                  | **Circuit 3**                  |
|-----------------------|--------------------------------|--------------------------------|--------------------------------|
| **Current Source**    | Resistor (400 Ω)               | Ideal Current Source (1 mA)    | Active Current Source (NMOS)   |
| **Practicality**      | Less Practical                 | Suitable for AC Analysis       | Realistic for Circuit Design   |

# **Key Inference :**

- Voltage Gain: In the resistor design, the gain is marginally lower than in the NMOS configuration. Because of the high output impedance of the current source, the gain is likewise higher than that of the resistor.
- The bias current stayed constant at roughly 0.61mA in all configurations, indicating that the circuit was appropriately biased.
- Common-Mode Voltage (Vocm): The output voltage was steady at approximately 1.1V, in accordance with the design parameters.

# **Conclusion :**

This experiment shows that a differential amplifier's performance is greatly impacted by the type of load used, whether it be an NMOS, resistor, or current source. Current source and NMOS loads are preferred for high-performance applications because they increase gain, stabilize, and guarantee appropriate biasing. This study reinforces fundamental ideas in analog circuit design by highlighting how crucial it is to choose the right load arrangement in order to maximize amplifier behavior.
