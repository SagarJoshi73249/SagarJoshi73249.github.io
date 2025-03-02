---
title: "Smart Plant Health Monitor"
description: "PLant monitoring system integrated with ChatGPT"
tags: ["Engineering", "Mechatronics"]
image: "/images/plant_monitor.jpg"
permalink: /projects/plant-monitor/
---
# Smart Plant Health Monitoring System

## Overview
With the increasing popularity of indoor gardening, maintaining plant health has become a challenge for plant owners. This project presents a **Smart Plant Health Monitoring System** that automates plant care through **real-time monitoring, AI-driven recommendations, and IoT-based control**. The system ensures that plants receive optimal care by integrating **sensors, automated watering mechanisms, and AI assistance via ChatGPT**.

![System Components](/images/plant_system.png)

## Key Features
- **Real-Time Plant Monitoring:** Continuously tracks **soil moisture, temperature, and light levels** to ensure optimal plant health.
- **AI-Powered Recommendations:** Utilizes **ChatGPT integration** to provide personalized plant care tips based on sensor data.
- **Automated Watering System:** Controls a **peristaltic water pump** and **solenoid valve** to dispense water precisely as needed.
- **IoT-Based Remote Access:** Connects to **Blynk IoT** for **real-time monitoring and control** from anywhere.
- **User-Friendly Interface:** Provides a **text-based input system** to retrieve plant-specific care instructions.
- **Modular & Scalable Design:** Supports easy customization and expansion for additional sensors and functionalities.

## Implementation
1. **Sensor Integration:**
   - **Soil Moisture Sensor (LM393):** Determines if watering is needed based on predefined thresholds.
   - **Temperature Sensor (DS18B20):** Monitors plant temperature and alerts users of critical conditions.
   - **LDR Module:** Measures ambient light levels to track sunlight exposure.
2. **Automated Watering System:**
   - Controlled via a **relay module** that activates a **12V peristaltic water pump** and **solenoid valve**.
   - Prevents **overwatering and underwatering** using **sensor feedback loops**.
3. **AI-Powered Care Instructions:**
   - Users input their plant species via a **text-based interface**.
   - The system queries **ChatGPT** for **personalized watering schedules, sunlight needs, and care guidelines**.
4. **IoT Integration & Remote Control:**
   - **Raspberry Pi Model 4B** manages data processing and communicates with **Blynk IoT** for remote monitoring.
   - **Arduino Mega** interfaces with sensors and actuates the watering system.
5. **User Interface & Monitoring:**
   - Real-time data visualization through the **Blynk IoT app**.
   - Displays **sensor readings and AI-generated plant care insights**.

![IoT-Based Plant Care](/images/plant_monitor.jpg)

## Key Achievements
 **Optimized Plant Health:** Real-time monitoring ensures precise care adjustments.  
 **AI-Assisted Guidance:** ChatGPT integration provides expert-level plant care recommendations.  
 **Hands-Free Automation:** Fully automated watering system eliminates human error in plant maintenance.  
 **Remote Monitoring & Control:** IoT integration enables users to manage plant care from anywhere.  
 **Scalable & Adaptable:** Supports future expansion for more sensors and additional plant types.