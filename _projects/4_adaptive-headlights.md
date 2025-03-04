---
layout: archive
author_profile: true
title: "Adaptive Headlight System Based on Audi Matrix LED"
description: "Developed an adaptive headlight system that dynamically adjusts beam intensity and direction based on vehicle speed and position. Implemented computer vision algorithms to detect oncoming traffic and prevent glare, enhancing night-time driving safety."
tags: ["Engineering", "Mechatronics"]
image: "/images/adaptive-headlight.png"
permalink: /projects/adaptive-headlights/
---

## Overview
Driving at night presents challenges such as reduced visibility and glare from oncoming headlights. This project focuses on designing and simulating an **adaptive headlight system**, inspired by Audi’s Matrix LED technology, to enhance nighttime driving safety. The system dynamically adjusts **individual LED segments in real-time** to optimize road illumination while reducing glare for oncoming traffic.

![Adaptive Headlight System](/images/matrix_led0.png)

## Key Features
- **Real-Time Vehicle Detection:** Uses a **webcam-based perception module** that employs **image processing and machine learning** to detect oncoming vehicles.
- **Automated Headlight Adjustment:** Dynamically dims or brightens **individual LED segments** based on vehicle positioning.
- **Live Distance Estimation:** Calculates the **x (lateral) and z (longitudinal) coordinates** of approaching vehicles for precise control.
- **Graphical User Interface (GUI):** Provides a **real-time visualization** of the adaptive headlight grid and system performance.
- **Simulation in CARLA:** Tests the system in a **realistic driving environment**, evaluating performance under various traffic densities and weather conditions.
- **Formal Verification:** Ensures safety compliance using **Linear Temporal Logic (LTL) and Signal Temporal Logic (STL).**

## Implementation
1. **Perception Module:** Detects headlights of oncoming vehicles using **OpenCV’s SimpleBlobDetector** and **LAB color space conversion**.
2. **Position Calculation:** Translates detected headlights into **real-world coordinates** using the camera’s field of view and trigonometric principles.
![](/images/matrix_led1.png)
3. **Adaptive Dimming Algorithm:** Adjusts LED brightness based on:
   - **Proximity of oncoming vehicles** (closer vehicles result in dimming).
   - **Vehicle position relative to the host car** (ensuring optimal road illumination).
   - **Handling multiple vehicles simultaneously** with independent segment control.
4. **Simulation & Testing:**
   - The system was simulated using **CARLA**, allowing for controlled experiments in **diverse road and weather conditions**.
   - Performance was validated using metrics like **detection accuracy (95%)**, **response time (~150ms)**, and **glare reduction (70%)**.


## Key Achievements
 **Enhanced Driver Visibility:** Optimized light distribution without causing glare.  
 **High Accuracy & Responsiveness:** 95% detection accuracy and **real-time adjustments in ~150ms**.  
 **Scalable & Modular Design:** Can be adapted for **real-world automotive applications**.  
