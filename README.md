# BC--LM2596--ADJ
## 1. Project Overview

The BC–LM2596–ADJ project is a DC–DC buck converter based on the LM2596 adjustable regulator, designed to efficiently step down a higher DC voltage to a stable, adjustable lower output. The circuit supports up to 3A output current and is suitable for embedded systems, power electronics, and prototyping applications. The schematic and PCB were designed using KiCad, following standard power PCB layout practices.

-----

## 2. Key Learning Objectives

Understand the working principle of a DC–DC buck (step-down) converter using the LM2596-ADJ.

Learn schematic capture, component selection, and value calculation for switching regulators.

Gain hands-on experience in power PCB layout techniques, including high-current routing, grounding, and loop minimization.

Understand the importance of input/output filtering and ripple reduction.

Apply design rule checks (DRC) and electrical rule checks (ERC) in KiCad.

Learn basic thermal considerations for power components.

Develop skills in generating manufacturing outputs such as Gerber, BOM, and pick-and-place files.
-----

## 3. Tools & Software Used
- **KiCad EDA**
  - Schematic Editor  
  - PCB Layout Editor  
  - 3D Viewer
 
 ---

## 4. Project Files
- Schematic design files (`.kicad_sch`)  
- PCB layout files (`.kicad_pcb`)  
- 3D render images  
- Manufacturing-ready Gerber files  

---

## 5. Block-Level Working Explanation

Input Power Block: Receives the DC input voltage and provides initial filtering to reduce noise and transients.

Control & Switching Block (LM2596-ADJ): Regulates the output by high-frequency switching and duty-cycle control based on feedback.

Inductor & Diode Block: Stores and transfers energy during switching cycles to achieve efficient voltage step-down.

Output Filter Block: Smooths the switching waveform using capacitors to provide a stable DC output.

Feedback Network: Uses a resistor divider to set and maintain the desired adjustable output voltage.

## 6. Bill of Materials (BOM)

| Reference | Qty | Value / Part No.    | Footprint                     |
| --------- | --- | ------------------- | ----------------------------- |
| **U1**    | 1   | LM2596S-ADJ         | TO-263-5_TabPin3              |
| **L1**    | 1   | 47 µH               | L_Bourns_SRR1208_12.7×12.7 mm |
| **D1**    | 1   | SS34 Schottky Diode | D_SMA                         |
| **D2**    | 1   | LED                 | LED_0603_1608Metric           |
| **C1**    | 1   | 100 nF              | CP_Elec_8×10                  |
| **C2**    | 1   | 100 µF              | C_0603_1608Metric             |
| **C3**    | 1   | 100 nF              | C_0603_1608Metric             |
| **C4**    | 1   | 220 µF              | CP_Elec_8×10                  |
| **R1**    | 1   | 47 kΩ               | R_0603_1608Metric             |
| **R2**    | 1   | 1 kΩ                | R_0603_1608Metric             |
| **RV1**   | 1   | 10 kΩ Potentiometer | Bourns 3296W (THT)            |
| **J1–J4** | 4   | 1×1 Pin Header      | PinHeader_1x01_P2.54 mm       |



## 7. Images & Renders

- **Schematic**


- **PCB Layout**
 <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a9a6f146-5755-47d6-8a8f-e9a6d766c865" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a72df87b-d163-44ae-8c2f-fc700208cdd4" />
 
- **3D View**
<img width="1249" height="725" alt="image" src="https://github.com/user-attachments/assets/e6bdbdfb-e660-406e-8802-f5c029f7c29e" />
<img width="1114" height="830" alt="image" src="https://github.com/user-attachments/assets/a21908d7-4499-4781-9e9b-be11cc6ff08c" />

---

## 8. Disclaimer
This project is intended for educational and reference purposes only. While the design has been tested at a basic level, it is not certified for commercial or safety-critical applications. Users are responsible for verifying the design, component ratings, and safety requirements before practical deployment.
---

## 9. Author
- **Name:** SUJIT KUMAR
- **Toolchain:** KiCad EDA  



