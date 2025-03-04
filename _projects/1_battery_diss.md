---
layout: archive
author_profile: true
title: "Robotic Compliant Object Prying Using Diffusion Policy Guided by Vision and Force Observations"
description: ""
tags: ["Motion Planning", "ROS2", "Robotics", "Perception"]
image: "/images/hardware_setup.png"
permalink: /projects/RAL-Battery/
---

## **Overview**
With the increasing demand for sustainable battery recycling, robotic systems are being developed to automate disassembly tasks. This project explores **dual-arm coordination, real-time motion planning, and diffusion-based action prediction** for battery disassembly using **ROS2, Nvidia cuMotion, OMPL, and force-vision integration**. The system enables scalable and efficient **autonomous disassembly workflows**, ensuring robustness in handling **uncertain object geometries** and varying battery orientations.

![Robotic Battery Disassembly](/images/steps_system%20(1).png)

## **Key Features & Objectives**
- **Dual-Arm Coordination:**
  - Engineered an optimized control framework for **ABB IRB120 and KUKA iiwa 14**.
  - Integrated **Nvidia cuMotion and OMPL** for high-efficiency motion planning.
  - Implemented coordinated force-torque control for synchronized manipulation.
- **Multi-View Perception & Visuo-Motor Learning:**
  - Developed a **ROS2-based multi-sensor perception pipeline** using **Intel RealSense**.
  - Captured **6D poses of objects** to enhance robot learning for real-time adaptation.
  - Employed **hand-guiding techniques** for **human-in-the-loop data generation**.
- **Diffusion Model-Based Action Prediction:**
  - Applied **diffusion policy learning** to **predict optimal disassembly actions**.
  - Integrated **force feedback and cross-attention mechanisms** to ensure robust execution.
  - Achieved **96% success rate** in diverse battery types and orientations.
- **Closed-Loop Disassembly with Real-Time Data-Driven Trajectories:**
  - Leveraged **differentiable motion paradigms** for scalable robotic autonomy.
  - Enabled **zero-shot transfer capabilities** to unseen objects and battery configurations.
  - Maintained safety and precision through **force-aware trajectory adjustments**.
- **Comprehensive Data Collection & Training:**
  - Collected **demonstration data using hand-guided kinesthetic teaching** for accurate ground truth actions.
  - Captured synchronized **force, vision, and robot state data** at each execution step.
  - Used **human-expert demonstrations** to refine visuo-motor policies and enhance generalization.
  - Processed and augmented collected data with **randomized perturbations** to improve robustness against real-world variability.

![Hardware Setup](/images/hardware_setup.png)

## **Implementation & Methodology**
1. **Dual-Arm Robotic Setup:**
   - ABB IRB120 used for **object stabilization**, KUKA iiwa 14 for **prying operations**.
   - **Multi-modal data acquisition** with force-torque sensors and stereo vision.
2. **Perception & Pose Estimation:**
   - **ROS2-based RealSense depth data streams** processed for real-time 6D pose estimation.
   - **Fusion of vision and force data** using cross-attention networks.
3. **Motion Planning & Control:**
   - **OMPL-based motion planner** optimized for real-time constraints.
   - Utilized **cuMotion library** to ensure **collision-free and dynamically stable paths**.
   - **Closed-loop adaptation** of robotic actions based on sensor feedback.
4. **Learning-Based Disassembly:**
   - **Diffusion models** used for policy learning and action refinement.
   - **Cross-attention mechanisms** enabled robust integration of **force and visual modalities**.
   - **Iterative reinforcement learning** refined policy generalization to varying disassembly tasks.

![System Architecture](/images/overview_system1.png)

## **Key Achievements**
 **High-Precision Battery Disassembly:** Integrated force-aware motion planning to handle varying battery positions and orientations.  
 **Multi-Sensory AI for Robust Execution:** Combined **vision, force, and learned representations** for stable real-world deployment.  
 **Scalable & Generalizable System:** Enabled **zero-shot adaptation** to unseen battery geometries and object layouts.  
 **Real-Time Deployment:** Leveraged **ROS2 and Nvidia cuMotion** for fast, collision-free, and adaptive robotic motion.  
 **Robust Data Collection & Training:** Employed **human-in-the-loop kinesthetic teaching** and **force-enhanced demonstrations** to maximize policy learning effectiveness.  

---
This project showcases an advanced **AI-driven robotic disassembly framework**, combining **ROS2, motion planning, and multi-modal learning** for high-performance automation. For more information about the project, check out our [website!](https://rros-lab.github.io/diffusion-with-force.github.io/)
