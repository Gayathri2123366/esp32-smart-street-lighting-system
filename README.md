# esp32-smart-street-lighting-system
IoT-based smart street lighting system using ESP32, LDR, and PIR sensors with adaptive brightness control.
# ESP32 Smart Street Lighting System

## Overview

This project implements an intelligent street lighting system using an ESP32 microcontroller. The system automatically controls streetlight brightness based on ambient light conditions and motion detection, improving energy efficiency and safety.

## Features

* Automatic day/night detection using an LDR sensor
* Motion detection using a PIR sensor
* Adaptive LED brightness using PWM control
* Energy-efficient smart lighting logic
* Simulation implemented using Wokwi

## Components Used

* ESP32 Microcontroller
* LDR Light Sensor Module
* PIR Motion Sensor
* LED
* 220Ω Resistor

## Working Principle

The LDR sensor measures ambient light intensity. When the environment is bright (daytime), the streetlight remains OFF. When it becomes dark (nighttime), the LED operates in dim mode to conserve energy. If motion is detected by the PIR sensor, the LED brightness increases to provide adequate illumination.

## System Logic

Day → LED OFF
Night + No Motion → LED DIM
Night + Motion → LED FULL BRIGHTNESS

## Simulation

The circuit and embedded logic were implemented and tested using the Wokwi ESP32 simulator.

## Future Improvements

* WiFi connectivity using ESP32
* MQTT-based communication
* Smart city monitoring dashboard using Node-RED
* Energy consumption monitoring
* Integration with cloud IoT platforms

## Applications

* Smart city infrastructure
* Energy-efficient street lighting
* Automated outdoor lighting systems
