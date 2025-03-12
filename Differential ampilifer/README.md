# **Differential Amplifier**

# Aim

Design and analyse the MOS differentual amplifier circuit and perform DC analysis , transient analysis and frequency response for the following specifications : 

- Supply voltage(V<sub>DD) = 2.2 V
- Output common mode voltage(V<sub>ocm) = 1.25 V
- Power(P) <= 2.2 mW
- Common mode input voltage (V<sub>icm) = 1.2 V
-  Voltage at point p(V<sub>p) = 0.4 V

# **Cirucit 1**

  - Resistor loaded differential pair

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

# **DC Analysis : **

- Make the circuit as shown above.
- Set the R<sub>D</sub> and R<sub>ss</sub> values as determined by the calculation.
- Vary W/L ratio of both the transistor to get the required V<sub>ocm</sub> and I<sub>S</sub>.
- Set the W/L ratio in such a way that the values are same fot both the transistors.
- Check the V<sub>GS</sub> and V<sub>DS</sub> value of the transistors such that it operates in saturation region.
- **Condtion for saturation region :**

  V<sub>GS</sub>>V<sub>TH</sub> ,

  V<sub>DS</sub>>V<sub>ov</sub>

- Calculate V<sub>incm(min)</sub>,V<sub>incim(max)</sub>,V<sub>out(min)</sub>,V<sub>out(max)</sub>.

  V<sub>incm(min)</sub> = V<sub>TH</sub> + V,sub>p</sub>
  
  V<sub>incm<min)</sub> = 0.366 + 0.4 = 0.766 V.

  V<sub>incm(max)</sub> = V<sub>DD</sub> - (I<sub>D</sub>R<sub>D</sub>) + V<sub>TH</sub>

  V<sub>incm(max)</sub> =

  V<sub>outcm(min)</sub> = V<sub>ov</sub> + V<sub>p</sub> =

  V<sub>outcm(max)</sub> = V<sub>DD</sub> -(I<sub>D</sub>R<sub>D</sub>) =

  # **Transient Analysis : **

  
