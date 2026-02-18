# KiCadLibrary

This repository contains the **custom KiCad libraries** I use across all of my electronics projects.

It includes:

- ✅ **Schematic Symbols**
- ✅ **PCB Footprints**
- ✅ **3D Models**

All libraries are maintained together to ensure consistency, accuracy, and repeatability across designs.

---

## Repository Structure

The repository is organized to align with KiCad’s library system:

- **Symbols** – Custom schematic symbols
- **Footprints** – PCB footprints for layout
- **3D Models** – 3D models used for rendering and mechanical verification

These libraries are designed to be referenced via a single KiCad environment variable.

---

## Installation & Setup

### 1. Clone or Download the Repository

Clone the repository (recommended):

```bash
git clone https://github.com/scostella/KiCadLibrary.git
```

### 2. Configure the KiCad Environment Variable

Open KiCad
Go to Preferences → Configure Paths
Add a new environment variable:
  Name: MY_KICAD_LIBS
  Path: Absolute path to the KiCadLibrary directory

### 3. Add Libraries to KiCad
Once the environment variable is set, add the libraries as usual:
#### Symbol Libraries
Open the Symbol Editor
Preferences → Manage Symbol Libraries
```code
${MY_KICAD_LIBS}/symbols/Custom.kicad_sym
```
#### Footprint Libraries
Open the Footprint Editor
Preferences → Manage Footprint Libraries
```code
${MY_KICAD_LIBS}/footprints/Custom.pretty
```
---

## Limited Liability and Disclaimer

This project is provided as an **open‑source hardware design** and is offered **as‑is**, without warranty of any kind.

By using this design, documentation, or any assembled hardware provided by the author, you agree to the following:

- You assume **all responsibility** for proper electrical design, wiring, installation, and use
- The author makes **no guarantees** regarding suitability for any specific application
- The author shall not be held liable for:
  - Damage to equipment
  - Electrical failures
  - Personal injury
  - Property damage
  - Losses resulting from improper use, installation, or modification

Use of this project or any associated hardware constitutes acceptance of these terms.

---

## Reference Projects

This project integrates with the Arduino CMRI ecosystem. The following projects provide related hardware, firmware, and configuration support:

- **Arduino Mega CMRI WiFi**  
  Arduino sketch for Mega 2560 to operate as CMRI Node with an ESP8266-ESP01 providing WiFi connectivity.
  https://github.com/scostella/Arduino_Mega_CMRI_WiFi

- **ESP8266 WiFi Setup Utility**  
  ESP sketch to program the ESP8266-ESP01 to work with the Arduino Mega 2560 and connection configuration for your WiFi network.
  https://github.com/scostella/ESP8266WiFiSetup

- **Arduino Mega CMRI WiFi Shield**  
  KiCad design for a shield for the Arduino Mega 2560 facilitating easy integration with the ESP8266-ESP01 and the CMRI modules listed below.
  https://github.com/scostella/Arduino_Mega_CMRI_WiFi_Shield

- **KiCad Custom Library**  
  Library containing all project parts in all designs.
  https://github.com/scostella/KiCadLibrary

- **Arduino Accessory Controller**  
  KiCad design for a board to control accessories up to 1 amp.
  https://github.com/scostella/Arduino-Accessory-Controller

- **Arduino IR Sensor Module - 8 Port**  
  KiCad design for a board to use TCRT5000 IR module to sense object presence which can also be used in the Arduino Mega CMRI WiFi module to group sensors to create virtual block detection.
  https://github.com/scostella/Arduino_IR_Sensor_Module_-_8_Port

- **Arduino Tortoise Controller with Feedback - 8 Port**  
  KiCad design for a board to control Circuitron Tortoise Slow Motion Switch machines and provide feedback on switch position either controlled internally by the voltage applied to the tortoise or an external signal.
  https://github.com/scostella/Arduino_Tortoise_Controller_with_Feedback_-_8_Port

- **Arduino Light Controller**  
  KiCad design for a board to control low amperage lighting and other loads (<10ma) using the Arduino's 5V source.
  https://github.com/scostella/Arduino-Light-Controller

These projects may be used together to form a complete CMRI‑controlled lighting and I/O system.

---

## Repository Contents

```text
/
├── 3dmodels
├── footprints
├── symbols 
└── README.md

