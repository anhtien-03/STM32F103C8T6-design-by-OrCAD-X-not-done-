# STM32F103 4-Layer PCB Design

A personal PCB design project based on the **STM32F103C8T6 microcontroller**, developed using **Altium Designer**. The main goal of this project is to practice multilayer PCB design, including component placement, power distribution, ground planes, signal routing, via transitions, and design rule checking.

## 1. Schematic

The complete schematic was designed around the STM32F103C8T6, including the power supply, decoupling capacitors, oscillator, reset circuit, SWD interface, USB interface, and GPIO expansion.

<img width="1098" height="864" alt="image" src="https://github.com/user-attachments/assets/0e77e288-4f1e-4c8b-a4d0-936962b19e29" />


## 2. PCB Layout – Top Layer

The Top Layer contains the main components and most of the critical signal routing. Particular attention was paid to component placement, short connections, and clean routing around the MCU.
<img width="1281" height="595" alt="image" src="https://github.com/user-attachments/assets/956bcc6b-9d00-4b6f-a63c-e57a9ac111ea" />




<img width="1483" height="680" alt="image" src="https://github.com/user-attachments/assets/ba99d1df-ac29-4fe9-ae7d-ea833b2e4d90" />


## 3. PCB Stackup

The board uses a 4-layer structure:

* **L1 – Top:** Components and signal routing
* **L2 – GND:** Solid ground plane
* **L3 – Power:** 3.3V power plane
* **L4 – Bottom:** Signal routing

![PCB Stackup](images/stackup.png)

## 4. Ground Plane – Layer 2

Layer 2 is dedicated to a continuous **GND plane**. This provides a low-impedance return path for signals and helps reduce noise and EMI.

<img width="1455" height="688" alt="image" src="https://github.com/user-attachments/assets/96ecd209-4cf1-4c15-b28b-08f40c10f37a" />


## 5. Power Plane – Layer 3

Layer 3 is used for **3.3V power distribution**. The power plane provides a low-impedance path for distributing power to the MCU and other circuits through vias.

<img width="1427" height="683" alt="image" src="https://github.com/user-attachments/assets/9481940d-d99e-4e7d-9912-ac19788c347e" />


## 6. Bottom Layer

The Bottom Layer is mainly used for additional signal routing and connections that cannot be completed on the Top Layer.

<img width="1431" height="684" alt="image" src="https://github.com/user-attachments/assets/a4185ca7-5f43-49c6-b1e5-46f09f491ee0" />


## 7. Full PCB – 4 Layer View

The final PCB consists of four copper layers with dedicated ground and power planes. The design was manually routed in Altium Designer and checked using DRC.

<img width="1554" height="748" alt="image" src="https://github.com/user-attachments/assets/0e3052d0-dfae-4445-9fee-f61c0c373249" />


## Key Features

* STM32F103C8T6 MCU
* 4-layer PCB
* Dedicated GND plane
* Dedicated 3.3V power plane
* SWD programming/debugging interface
* External crystal oscillator
* USB interface
* GPIO expansion headers
* Decoupling and power filtering
* Manual signal routing
* Design Rule Check (DRC)

## Learning Objectives

This project was developed as part of my personal learning path in **PCB design and embedded hardware engineering**. It focuses on understanding how multilayer stackups, power distribution, ground planes, signal routing, and return paths affect PCB performance.

