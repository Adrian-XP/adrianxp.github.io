---
title: Module's Requirements
---

## Module Requirements
In this project, I'm on the controller/transmitter system to control the submarine

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| Surface mounted, 3.3V switching power regulatore | 3.2 Volts | 3.3 Volts | No |
| Surface mounted microcontroller | 1 PIC or ESP | 8-bit PIC | No |
| Wireless Communication | Able to send or receive a Wi-Fi data | Send and receive Wi-Fi Data to MQTT | Yes |
| Motor Drive Topology | Dual H-Bridge | MOSFET-based H-Bridge | No |
| Actuator Support | 1x Brushless DC Motor | 2x BLDC with Encoder feedback | No |
| Feedback | Status LEDs | 0.96" OLED Display for live diagnostics | Yes |
| External Antenna | Internal PCB Trace Antenna | 2.4GHz Dipole Antenna | Yes |
| Emergency Stop | Software "Kill" command | Physical Switch | No |
