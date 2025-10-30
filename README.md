# Electronic Monitoring System Project

## Project Overview
This project is a **medium-complexity electronic monitoring system** based on a microcontroller. It reads data from sensors (temperature and light), displays information on an LCD, controls LEDs and a buzzer, and allows user interaction via buttons.

---

## Defined Design Requirements
- Designed a **medium-complexity electronic board** including:
  - LCD  
  - Temperature sensor  
  - Buzzer  
  - LEDs  
  - Buttons  
  - Voltage regulator  
- Created a **block diagram** representing the main components and their interconnections.  
- Implemented the system at the **discrete component level**.  
- Developed the **layout for the electronic board**.

---

## Block Diagram
    +-------------------+
    |  Voltage Regulator|
    |       LM7805      |
    +---------+---------+
              |
              v
     +--------+--------+
     |  Microcontroller |
     |    PIC16F877A    |
     +---+---+---+---+--+
         |   |   |   |
         v   v   v   v
       LCD  LEDs Buzzer Sensors
                |         |
                |         +------> Temperature Sensor (TMP36)
                |         +------> Light Sensor (LDR)
         Buttons

---

## Block Description

### 1. Voltage Regulator (100)
- Uses **LM7805** to provide stable +5V.  
- Powers microcontroller and other components.

### 2. Microcontroller (200)
- **PIC16F877A** or similar.  
- Connected to LCD, LEDs, buzzer, sensors, and buttons.

### 3. LCD (300)
- 16x2 display.  
- Displays real-time sensor data and system status.

### 4. LEDs (400)
- Four LEDs controlled via **BC817 transistors**.  
- Indicate system states or alerts.

### 5. Buzzer (500)
- Activated via **BC817 transistor**.  
- Provides audible notifications.

### 6. Temperature Sensor (600)
- **TMP36** analog sensor.  
- Sends analog voltage to microcontroller.

### 7. Light Sensor (700)
- **LDR** with voltage divider.  
- Measures ambient light.

### 8. Buttons (800)
- Three push buttons with **pull-down resistors**.  
- Allow user to interact (mode change, reset, etc.).

### 9. Connector (900)
- For programming or external module connection.  
- Provides power and communication pins.

---

## PCB Manufacturing Sponsor

This PCB was kindly sponsored by **PCBWay**, who provided fabrication support for this project.

I would like to thank PCBWay for:
- High PCB manufacturing quality  
- Fast order processing & delivery  
- Professional communication and support  

More about their services:  
➡️https://m.pcbway.com/

## 🖼️ PCB Preview

### 🔹 Top View
![PCB Top View](./PCBWay/pcb_top.jpg)

### 🔹 Bottom View
![PCB Bottom View](./PCBWay/pcb_bottom.jpg)

## Summary
This project demonstrates the design, implementation, and layout of a medium-complexity electronic board capable of **monitoring environmental parameters**, **displaying data**, and **interacting with users** through LEDs, buzzer, and buttons.






