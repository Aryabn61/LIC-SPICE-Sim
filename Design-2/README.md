# Experiment 2
Q. For the given circuit below find the DC operating point , gain and AC analysis.Use P=100m W.

![d2dc1](https://github.com/user-attachments/assets/3f261abd-339e-4f7e-a149-4adbe63c4417)

**Aim :** To find the DC operating point of the transistor , gain using transient analysis and AC analysis.

**Theory :**

Two complementary MOSFET transistors, a P-channel (PMOS) and an N-channel (NMOS), are used in CMOS inverter circuits. The input voltage applied to the gates of both transistors regulates which transistor is "on" and which is "off," thereby inverting the input signal to generate the opposite logic level at the output.

**Procedure:**

• Make the circuit connection as above.

• Make the V1 source as 1.8 V DC power supply.

• Find Vb through calculation.

• Set V3 to 0.9 V.

# DC Analysis

For DC analysis we need to find the operating point of the transistor.Make sure that both the transistor is operating in saturation region.

![d2dc1](https://github.com/user-attachments/assets/3f261abd-339e-4f7e-a149-4adbe63c4417)

For the transistor to work as amplifier it should operate in saturation region. 

From the circuit , Vs = 1.8 V.

VG < (1.8-VTH) 

VG < (1.8-0.3906) 

**VG < 1.25 V.**

Therefore Vb = 1.25 V.

![d2dc2](https://github.com/user-attachments/assets/3bb05d9a-8683-4c97-9598-78e15bc9d419)

**DC operating point is (1.47 V, 55µ A).**

# Transient analysis

Set the input voltage to sine with DC offset to 0.9 V , amplitude 50m V and frequency to 1K Hz and run the simulation.

![d2 t2](https://github.com/user-attachments/assets/f442237b-29c5-4b82-848d-9c1887a7331a)

# Output waveform:

![d2t1](https://github.com/user-attachments/assets/02b180ed-1e04-49b2-8616-b946722c3534)

Gain is A = Vout/Vin

A = 1.53/950m

**A = 1.61.**

# AC analysis

Set the voltage to AC amplitude and the run the AC analysis . Set the operatin gfrequency range to 0.1 Hz to 1T Hz.
![dd2ac1](https://github.com/user-attachments/assets/128406c0-d186-48ea-870b-21cb48206e3a)

# Output waveform :

![413645423-0e88e620-960c-46b1-bd4f-bc21f8f7b084](https://github.com/user-attachments/assets/0b09c1c0-c7b9-4123-8668-a7e61f766cbc)

# Result:

• DC operating point : (1.47 V, 55µ A).

• Gain , A = 1.61.

# Inference : 

• If the Vb value is less than 1.25 V then the mosfet M1 will operates in cut-off region and does not conducts.

• For medium gain we need to select the DC operatin gpoint in between cut-off and triode region with reference to voltage transfer characteristics graph(VTC curve).

• In AC analysis we can seed that at starting frequecny range the graph increases as the circuit behaves as low pass filter where the coupling and bypass cpacitors acts and at some frequency range the graph becomes constant and at higher frequencies the internal capacitor or the parasitic capactor gets activated.
