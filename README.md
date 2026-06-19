# Non-Inverting Amplifier - PCB & Hardware Design

A complete, production-ready Altium Designer project for a non-inverting operational amplifier circuit. This repository contains the verified schematic, PCB layout, 3D renders, and complete manufacturing data (Gerbers, NC Drill, BOM).

## Project Overview
The objective of this project was to take a standard analog circuit from theoretical calculation to a fully manufacturable printed circuit board. 

### 3D Board Renders
<img width="600" alt="image" src="https://github.com/user-attachments/assets/de03c2ad-7ecb-4238-90ed-f309aaa1a792" />
Top View

<img width="600" alt="image" src="https://github.com/user-attachments/assets/c7d7add1-d0ac-4add-a4a1-e480ccb37605" />
Bottom View

## Circuit Design & Verification
Rather than relying on default textbook values, the core schematic was rigorously cross-referenced and verified against alternative technical models to ensure optimal component selection and mathematical accuracy before routing.

* **Target Gain:** [e.g., 10 V/V]
* **Gain Equation:** Vout = Vin * (1 + R2/R1)
* **Feedback Resistor (R2):** [e.g., 90k Ohms]
* **Ground Resistor (R1):** [e.g., 10k Ohms]
* **Operational Amplifier:** [e.g., LM358 / TL072]

*(Optional: Drag and drop a screenshot of your SPICE simulation or Bode plot here to prove the gain mathematically).*

## PCB Specifications & Layout Constraints
The board was routed with strict adherence to standard manufacturing design rules to ensure zero DRC (Design Rule Check) errors.

* **EDA Tool:** Altium Designer
* **Layer Stackup:** 2-Layer (Top/Bottom Copper)
* **Material:** FR-4
* **Board Dimensions:** [e.g., 40mm x 30mm]
* **Signal Trace Width:** [e.g., 10 mil]
* **Power/Ground Trace Width:** [e.g., 20 mil]
* **Clearance Rules:** [e.g., 10 mil trace-to-trace]
* **Vias:** [e.g., 12 mil hole / 24 mil diameter]

## Repository Structure
This repository is organized to separate source files from manufacturing and documentation outputs:

* `/Docs`: Assembly drawings, schematic PDFs, and interactive 3D PDFs for quick review.
* `/Fabrication`: Production-ready output files for fab houses, including RS-274X Gerbers, NC Drill files, and a detailed Bill of Materials (BOM).
* `/Hardware`: The core Altium `.PrjPcb` project and raw schematic/layout source files, along with the final DRC report.

## Manufacturing Ready
The files in the `Fabrication` directory can be sent directly to standard board houses (e.g., JLCPCB, PCBWay). The BOM includes exact Manufacturer Part Numbers (MPNs) for seamless assembly.
