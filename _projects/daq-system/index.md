---
layout: post
title: Data Acquisition System
description:  High-speed data acquisition system developed for generic fluid systems.
              Includes 12 thermocouple inputs, 12 pressure transducer inputs, 4 load cell inputs, 1 pyrotechnic output.
              Runs Synnax software locally and communicates with command and control computer over fibre-optic at up to 800m of range.
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
