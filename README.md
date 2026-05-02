# 12-Channel IR Sensor Array with Multiplexer

## Overview
This project implements a 12-channel infrared (IR) sensing system using LTH-1550-01 reflective sensors and a 16-channel analog multiplexer (HEF4067/CD74HC4067). The system reads multiple analog signals using a single ADC pin on a microcontroller such as the ESP32.

It is suitable for line-following robots, object detection, and surface sensing applications.

---

## Features
- 12 IR reflective sensors
- Single ADC input using multiplexer
- Reduced GPIO usage
- Expandable up to 16 channels
- Stable analog signal output
- PCB-friendly design

---

## Components Required

### Sensors and IC
- 12 × LTH-1550-01 IR sensors
- 1 × HEF4067 or CD74HC4067 multiplexer IC

### Passive Components
- 12 × 10kΩ resistors (pull-up for phototransistor)
- 12 × 220Ω resistors (IR LED current limiting)
- 1 × 100nF ceramic capacitor (decoupling)
- 1 × 10kΩ resistor (optional pull-down on SIG)
- Optional: 10µF capacitor (power stabilization)

### Microcontroller
- ESP32 (recommended) or Arduino

---

## Circuit Design

### IR LED Connection
