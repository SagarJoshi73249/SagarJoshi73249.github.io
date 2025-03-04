---
layout: archive
author_profile: true
title: "Robotic System for Glass Handling in Solar Panel Manufacturing"
description: "Automating precision glass handling using ABB IRB 4600 and inverse kinematics"
tags: ["Industrial Robotics", "Motion Planning", "Webots", "Automation"]
image: "/images/glass-handling.png"
permalink: /projects/glass-handling/
---

## **Project Overview**
This project presents an **advanced robotic automation system** for **precision glass handling** in **solar panel manufacturing**. The system integrates an **ABB IRB 4600-20/2.50 robot**, an **inverse kinematics (IK) solver**, and **vacuum-based gripping mechanisms** to efficiently manipulate **large glass sheets** (1.5m x 0.9m, 3mm thick) without causing surface defects.

## **Key Features & Implementation**

### **Inverse Kinematics & Motion Planning Optimization**
- Developed a **custom inverse kinematics (IK) solver** for **real-time trajectory optimization**.
- Implemented **collision-aware motion planning**, adapting to workspace constraints dynamically.
- Utilized **constraint-based IK formulations** to ensure **stable force application** during glass handling.

### **Adaptive Vacuum Gripper System**
- Designed a **multi-point vacuum gripping mechanism** with **Schmalz STGG S 100×55 grippers**.
- Integrated a **venturi generator-based suction system** for high-efficiency glass handling.
- Engineered a **manifold vacuum distribution system** for **uniform grip force** across contact points.

### **ROS2-Based Robotic Control & Automation**
- Developed **ROS2 control nodes** using **rclpy**, integrating **MoveIt! action clients** for precise motion execution.
- Implemented **sensor-driven force feedback loops** for real-time grasping adjustments.
- Created **ROS2 action servers** for high-level task execution and motion coordination.

### **High-Fidelity Simulation & Digital Twin Development**
- Modeled the robotic system in **Webots** for **pre-deployment validation and trajectory testing**.
- Simulated **IK-based pick-and-place operations** to verify **grip stability and collision-free movement**.
- Conducted **virtual testing of force and contact constraints**, ensuring safe glass manipulation.

### **Scalability & Deployment Readiness**
- Designed a **modular robotic framework**, adaptable for **different glass sizes and handling workflows**.
- Implemented **automated fault detection** using **sensor-driven feedback loops**.
- Optimized system for **seamless integration with conveyor-based manufacturing lines**.

![ABB IRB 4600 Handling Glass](/images/DEMO.mp4)

## **Key Takeaways**
 **High-Precision Manipulation**: Integrated **inverse kinematics and trajectory optimization** to **enhance accuracy**.  
 **Intelligent Motion Planning**: Developed a **collision-aware, constraint-driven robotic control pipeline**.  
 **Validated via Digital Twin Simulation**: Conducted **Webots-based simulation** for real-world deployment.  
 **Process Optimization for Manufacturing**: Increased **automation efficiency and throughput**.  
 **Scalable for Multi-Robot Applications**: Designed an **adaptive framework** for **multi-arm handling systems**.  

---

This project highlights **advanced motion planning, robotic automation, and digital twin validation** for **high-precision glass handling**, contributing to **scalable industrial robotics solutions**. 🚀
