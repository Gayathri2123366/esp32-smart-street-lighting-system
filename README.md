# ESP32 Smart Street Lighting System

## Overview

This project implements an intelligent street lighting system using an ESP32 microcontroller. The system automatically controls streetlight brightness based on ambient light conditions and motion detection, improving energy efficiency and safety.

The system was designed and validated using the Wokwi ESP32 simulator before hardware implementation.

---

## Live Simulation

You can run the complete circuit simulation here:

https://wokwi.com/projects/458642497868369921

---

## System Architecture

```
        LDR Sensor
           │
           │ (Ambient Light)
           ▼
        ESP32 Controller ─────► LED Street Light
           ▲
           │
     PIR Motion Sensor
```

The ESP32 reads the LDR sensor to determine day or night conditions.
If it is night, the LED operates in **energy-saving dim mode**.
When the PIR sensor detects motion, the LED switches to **full brightness**.

---

## Features

* Automatic day/night detection using LDR sensor
* Motion detection using PIR sensor
* Adaptive brightness control using PWM
* Energy-efficient street lighting logic
* ESP32-based IoT-ready architecture
* Simulation implemented using Wokwi

---

## Components Used

* ESP32 Development Board
* LDR Light Sensor Module
* PIR Motion Sensor
* LED
* 220Ω Current Limiting Resistor

---

## Working Principle

The LDR sensor measures ambient light intensity.

System behavior:

```
Daytime → LED OFF
Night + No Motion → LED DIM
Night + Motion Detected → LED FULL BRIGHTNESS
```

This adaptive lighting logic reduces energy consumption while ensuring safety.

---



## Applications

* Smart city infrastructure
* Energy-efficient street lighting
* Automated outdoor lighting
* Smart traffic monitoring systems

---

## Future Improvements

* WiFi connectivity using ESP32
* MQTT-based communication
* Remote monitoring dashboard (Node-RED)
* Cloud-based smart city integration
* Energy consumption monitoring

---

## Author

Gayathri Devarapu

