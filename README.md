# Custom Macropad
A custom-designed macropad board using Raspberry Pi Pico 2, dual rotary encoders, three switches and a dedicated 1.8 inch SPI display.

## Visuals
<img width="1589" height="1170" alt="image" src="https://github.com/user-attachments/assets/f573fe59-34fe-4fdb-aed9-df04b57d6955" />
<img width="2032" height="1346" alt="image" src="https://github.com/user-attachments/assets/06b68cb2-343c-4eeb-a5d5-c17b6a1405f2" />
<img width="967" height="785" alt="image" src="https://github.com/user-attachments/assets/a9a5b149-e344-47b9-97d0-091ad638d8ad" />
<img width="1038" height="819" alt="image" src="https://github.com/user-attachments/assets/189ce4ba-e983-46ae-ac86-3919173d1de8" />




## Hardware Specifications
* **Microcontroller:** Raspberry Pi Pico 2
* **Display:** 1.8-inch TFT LCD Module (SPI Interface)
* **Inputs:** 3x Buildcon Blue Mechanical Keyswitches & 2x Flyrobo EC11 15mm Rotary Encoders
* **Knobs & Keycaps:** 2x Black Aluminum Alloy 19x19mm Screw-Type Knobs & Trendivibe PBT MA Profile Ball Shape Keycaps
* **PCB Specs:** 2-layer FR4, 124.0 x 104.0 mm, 1.6mm thickness

## Key Design Features
* **Using Berg strip:** Things are fully socketed using Berg strips, allowing for easy swapping, testing and safety during soldering.
* **Ground Plane:** A dedicated copper pour layer has been used across the layout to connect all GND points.

## Pin layout

### Display (J1)

| Pin Name | Connection Type | Pico pin | Working |
| :--- | :--- | :--- | :--- |
| 3V3 | Power | 3V3 | Power |
| GND | Ground | GND | Ground |
| DISP_CS | SPI Chip Select | GPIO 9 | Chip Select |
| DISP_RESET | Shared Reset | GPIO 13 | Hardware Reset |
| DISP_DC | Digital Output | GPIO 12 | Data/Command |
| SPI_MOSI | SPI Data | GPIO 15 | Master Out Slave In |
| SPI_SCK | SPI Clock | GPIO 14 | Serial Clock |
| 3V3 | Power | 3V3 | Backlight |

### Switches

| Pin Name | Connection Type | Pico pin | Working |
| :--- | :--- | :--- | :--- |
| KEY_BACK | Digital Input | GPIO 0 | SW1  |
| KEY_PAUSE | Digital Input | GPIO 1 | SW2  |
| KEY_NEXT | Digital Input | GPIO 2 | SW3  |

### Encoders

| Pin Name | Connection Type | Pico pin | Working |
| :--- | :--- | :--- | :--- |
| ENC1_A | Digital Input | GPIO 3 | Rotary 1 Phase A |
| ENC1_B | Digital Input | GPIO 4 | Rotary 1 Phase B |
| ENC1_SW | Digital Input | GPIO 5 | Rotary 1 Click |
| ENC2_A | Digital Input | GPIO 6 | Rotary 2 Phase A |
| ENC2_B | Digital Input | GPIO 7 | Rotary 2 Phase B |
| ENC2_SW | Digital Input | GPIO 8 | Rotary 2 Click |
