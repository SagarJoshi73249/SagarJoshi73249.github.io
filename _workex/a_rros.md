---
layout: single
title: "Dual-Arm Coordination for Battery Disassembly"
permalink: 
author_profile: true
tags: [robotics, motion-planning, computer-vision, deep-learning, ABB, KUKA, Nvidia]
---

## Realization of Robotic Systems Lab (RROS)
**Research Assistant**  
📍 Los Angeles, CA | 🗓 **May 2024 – Present**  

### **Overview**
At the Realization of Robotic Systems Lab (RROS), my work focuses on **dual-arm coordination** and **autonomous robotic manipulation** for **battery disassembly workflows**. This research is aimed at **improving recycling efficiency and safety** by leveraging **cutting-edge motion planning, visuo-motor learning, and AI-driven action prediction**.

In this project, I am integrating advanced **motion planning algorithms, real-time perception, and machine learning models** to create a scalable, autonomous robotic system capable of handling **uncertain and variable battery geometries**.

---

### **Dual-Arm Coordination & Motion Planning**
The robotic setup consists of:
- **ABB IRB120**: A high-speed industrial arm, used for **precise cutting and handling**.
- **KUKA iiwa 14**: A collaborative lightweight manipulator, enabling **safe and adaptive interactions**.

To **synchronize** both arms efficiently, I implemented:
✅ **Nvidia cuMotion library**: A CUDA-accelerated **motion planning library** that allows real-time trajectory optimization.  
✅ **OMPL (Open Motion Planning Library)**: Used for **path planning**, ensuring optimal movement in **cluttered environments**.  

By leveraging these tools, the robotic arms can execute **coordinated motions**, achieving **safe and efficient battery disassembly**.

🖼️ **Setup Image:**  
![Dual-Arm Coordination Setup](/assets/images/work_experience/rros_dual_arm.jpg)

---

### **Multi-View Perception & Human-In-The-Loop Data Collection**
To **enhance perception and control**, I incorporated:
- **ROS2 + Intel RealSense** for multi-view **6D pose estimation**.
- **Visuo-Motor Learning**: Used to improve robotic control based on real-time sensor feedback.
- **Hand-Guided Data Generation**: Allows human operators to **demonstrate movements**, helping the robot **learn from experience**.

🎥 **Demonstration Video:**  
<video controls>
    <source src="/assets/videos/work_experience/hand_guided_learning.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

---

### **AI-Based Action Prediction for Uncertain Environments**
Battery disassembly presents **unpredictable variations** in:
- Shape
- Size
- Orientation

To address this, I integrated **diffusion-model-based action prediction**:
✔ **Closed-loop control** that adapts in real-time.  
✔ **Model predictive control (MPC)** for robust planning.  
✔ **Generalization across different battery types.**

---

### **Scalable Deployment & Large Model Testing**
To bridge the gap between simulation and reality, I developed a **data-driven trajectory execution framework**:
- **Differentiable Motion Planning**: Enables **scalable autonomy**.
- **Real-Time Policy Updates**: The system continuously refines its approach as it encounters **new object geometries**.
- **Edge Deployment**: Deployed models are optimized for real-world execution.

This project paves the way for **next-generation robotic disassembly and recycling**.

---
