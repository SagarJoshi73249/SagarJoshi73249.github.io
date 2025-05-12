---
layout: archive
author_profile: true
title: "Task-Aware Diffusion Policy with Language Guidance for Multi-task Disassembly"
description: "Developed a hierarchical diffusion policy architecture for multi-task robotic disassembly using KUKA iiwa, integrating vision, force, and language modalities for real-time manipulation."
tags: ["Diffusion Models", "Multi-task Learning", "Language-Guided Robotics", "ROS2"]
image: "/images/language-guided.png"
permalink: /projects/CASE-task-aware/
---

## **Overview**
This project addresses the complexity of robotic disassembly in **high-mix manufacturing settings** by introducing a **task-context-aware diffusion policy** that leverages **natural language commands**, **vision**, and **force feedback**. We propose a hierarchical learning architecture capable of **interpreting task goals from language**, dynamically adapting policies for multiple disassembly actions using a **single multi-task diffusion model**.

![Task Context Illustration](/images/language_guided.png)

## **Key Features & Innovations**

### **Language-Guided Policy Learning**
- Developed a **language-conditioned diffusion policy** enabling task selection through natural language commands.
- Utilized **CLIP embeddings** to encode task and sub-task context, guiding robot action selection across complex scenes.

### **Hierarchical Task Decomposition**
- Modeled disassembly procedures as **parent tasks and sub-task modes** (e.g., approach, grasp, pull).
- Enabled **explicit sub-task awareness** to improve transition reliability and execution efficiency.

### **Adaptive Sensor Modality Weighting**
- Introduced a **FiLM-based feature modulation mechanism** that dynamically adjusts the reliance on vision and force sensors depending on sub-task.
- Enhanced performance in **contact-rich manipulations** requiring fine-tuned force control.

### **Cross-Modal Policy Architecture**
- Incorporated **cross-attention between image and force features** to fuse sensory input and improve generalization to unseen connector types.
- Modeled policies using **delta 6-DoF actions** for continuous low-level control.

### **Hardware Setup & Real-World Deployment**
- Deployed on a **KUKA LBR IIWA 14 robot** equipped with **dual RealSense wrist-mounted cameras** and integrated **force-torque sensing**.
- Evaluated performance on the **NIST Task Board** featuring multiple connector types requiring distinct manipulation strategies.

### **Zero-Shot Task Adaptation**
- Demonstrated **zero-shot generalization** to novel connector geometries and configurations.
- Achieved **95% task success rate** across diverse connector types with a **57% reduction in task execution time**.

![Framework Overview](/images/overview_system.png)

## **Results**
- Outperformed baseline diffusion models trained without language or force by **57%** in success rate.
- Enabled **human-in-the-loop disassembly sequences** where task order was specified via language.
- Improved **mode-switching speed**, reducing idle time and increasing task throughput.

## **Key Takeaways**
**Task-Driven Diffusion Modeling**: Hierarchically structured diffusion policies lead to better task efficiency and adaptability.  
**Language + Vision + Force**: Combining these modalities unlocks robust robotic behavior in ambiguous environments.  
**Multi-task Generalization**: One model handles multiple disassembly tasks with **minimal demonstrations**.  
**Real-World Ready**: Demonstrated success on physical robots with diverse hardware and connector configurations.

---

This research showcases the potential of **language-conditioned multi-modal diffusion policies** in enabling **flexible and intelligent robotic disassembly** across complex real-world scenarios.  
 [Project Website](https://rros-lab.github.io/diffusion-with-force.github.io/)
