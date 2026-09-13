# obstacle-avoiding-car-pcb
this project concerns a design   of an simple **ATMEGA 328P**  based  2 wheels obstacles avoiding car.

## Project Overview

The project features a custom Printed Circuit Board (PCB) designed to control a mobile robot, handling power distribution, microcontroller interfacing, motor drivers, and sensor integration.

* **Project File:** `voiture.kicad_pro`
* **Schematic File:** `voiture.kicad_sch`
* **PCB Layout File:** `voiture.kicad_pcb`
* **BOM File:** `BOM.csv`

---

## Design Specifications & Rules

* **Design Tool:** KiCad EDA (v8.0+)
* **Grid & Clearance:**
  * Minimum Track Width: `0.2 mm`
  * Minimum Clearance: `0.2 mm`
  * Default Via Diameter: `0.6 mm` (Drill: `0.3 mm`)
  * Copper-to-Edge Clearance: `0.5 mm`
* **Verification Status:**
  * **ERC Status:** Passed (0 Errors, 0 Warnings)
  * **DRC Status:** Passed (0 Violations, 0 Unconnected Pads)
 
    ####  Peripheral & Hardware Pinout Table for programming
| Hardware Module | Peripheral Signal | ATmega328P Pin (DIP-28) | I/O Type 

| **Motor 1 (Left)** | `IN1` | Pin 4 (`PD2`) | Digital Output

| **Motor 1 (Left)** | `IN2` | Pin 6 (`PD4`) | Digital Output 

| **Motor 1 (Left)** | `ENA` | Pin 11 (`PD5`) | PWM Output

| **Motor 2 (Right)** | `IN3` | Pin 13 (`PD7`) |Digital Output

| **Motor 2 (Right)** | `IN4` | Pin 18 (`PB4`) | Digital Output

| **Motor 2 (Right)** | `ENB` | Pin 12 (`PD6`) | PWM Output

| **Ultrasonic Sensor (HC-SR04)** | `Trig` | Pin 14 (`PB0`) | Digital Output 

| **Ultrasonic Sensor (HC-SR04)** | `Echo` | Pin 17 (`PB3`) | Digital Input 

| **Reset Button** | `Reset` | Pin 1 (`PC6`) | Input 

| **Logic Supply** | `VCC / AVCC` | Pin 7 & Pin 20 | Power In

| **Ground** | `GND` | Pin 8 & Pin 22 | Power In 

| **System Clock** | `XTAL1 / XTAL2` | Pin 9 & Pin 10 | Oscillator 
