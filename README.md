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

* **Target Gain:** 2 V/V
* **Gain Equation:** Vout = Vin * (1 + R2/R1)
* **Feedback Resistor (R2):** 10k Ohms (RG2012L-103)
* **Ground Resistor (R1):** 10k Ohms (RG2012L-103)
* **Operational Amplifier:** OPA333 (OPA333AIDCKR)
* **Power Supply Topology:** Single-Supply
* **Decoupling / Bypass Capacitor:** 100nF
* **I/O Connectors:** SMA (73251-1153)


## PCB Specifications & Layout Constraints
The board was routed with strict adherence to standard manufacturing design rules to ensure zero DRC (Design Rule Check) errors.

* **EDA Tool:** Altium Designer
* **Layer Stackup:** 2-Layer (Top/Bottom Copper)
* **Material:** FR-4
* **Board Dimensions:** 50mm x 50mm
* **Signal Trace Width:** 10 mil (0.254 mm)
* **Power/Ground Trace Width:** 10 mil (0.254 mm)
* **Clearance Rules:** 10 mil (0.254 mm) trace-to-trace/pad
* **Vias:** None utilized in this specific layout iteration

<img width="600" alt="image" src="https://github.com/user-attachments/assets/ab1f144e-8f0d-4981-ac0f-085e1d55dcd3" />


## Repository Structure
This repository is organized to separate source files from manufacturing and documentation outputs:

* `/Docs`: Assembly drawings, schematic PDFs, and 3D layout views.
* `/Fabrication`: Production-ready output files for fab houses, including RS-274X Gerbers, NC Drill files, and a detailed Bill of Materials (BOM).
* `/Hardware`: The core Altium `.PrjPcb` project and raw schematic/layout source files, along with the final DRC report.

## Manufacturing Ready
The files in the `Fabrication` directory can be sent directly to standard board houses (e.g., JLCPCB, PCBWay). The BOM includes exact Manufacturer Part Numbers (MPNs) for seamless assembly.
