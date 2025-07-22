---
layout: post
title: Propulsion Data Acquisition System
description:  High-speed data acquisition system developed for propulsion/fluid systems.
              Includes thermocouple, pressure transducer, and load cell inputs, and pyrotechnic output.
              Runs Synnax node locally and communicates with control computer over fibre-optic (800m range).
skills: 
- Data acquisition
- Sensor systems
- Control
- Networking
main-image: /daq.jpg 
order: 1
---

## Hardware
- DIN-mounted components across 24V (sensors, actuators) and 5V (control logic) subsystems.
- Safety-oriented design with safety relay circuits with e-stops for valve actuation.

{% include image-gallery.html images="daq-build-2.jpg, daq-2.jpg" height="400" %}

## Control and sequencing
- Instance (node) of Synnax Labs software running on NUC (Linux)
- Custom safety logic running in real-time on NUC
- Non-safety-critical logic and control controlled by networked (optical) PC at control station
- Developed simulated DAQ/fluid system to SITL test when away from fluid/sensor system. 
{% include image-gallery.html images="daq-build-1.JPG, synnax.png" height="400" %}
