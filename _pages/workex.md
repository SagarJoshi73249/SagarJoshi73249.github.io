---
layout: archive
title: "Work Experience"
permalink: /work-experience/
author_profile: true
---

<style>
    :root {
        --primary-color: #333;
        --secondary-color: #666;
        --accent-color: #0077B5;
        --light-bg: #f8f9fa;
        --dark-bg: #222;
        --card-shadow: 0 4px 6px rgba(0,0,0,0.1);
        --card-hover-shadow: 0 10px 15px rgba(0,0,0,0.15);
        --transition-speed: 0.3s;
    }

    .card-container {
        display: grid;
        grid-template-columns: 1fr;
        gap: 40px;
        margin: 50px 0 60px;
    }

    .card {
        background-color: white;
        border-radius: 12px;
        overflow: hidden;
        box-shadow: var(--card-shadow);
        transition: transform var(--transition-speed), box-shadow var(--transition-speed);
    }

    .card:hover {
        transform: translateY(-5px);
        box-shadow: var(--card-hover-shadow);
    }

    .card-header {
        display: flex;
        align-items: center;
        padding: 30px;
        background-color: rgba(0, 119, 181, 0.05);
        border-bottom: 1px solid rgba(0, 0, 0, 0.05);
    }

    .card-logo {
        width: 80px;
        height: 80px;
        border-radius: 50%;
        background-color: rgba(0, 119, 181, 0.15);
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: 25px;
        flex-shrink: 0;
    }

    .card-logo img {
        width: 60%;
        height: 60%;
        object-fit: contain;
    }

    .card-title-area {
        flex-grow: 1;
    }

    .card-title {
        font-size: 1.5rem;
        margin: 0 0 5px 0;
        color: var(--dark-bg);
    }

    .position-details {
        font-size: 1rem;
        color: var(--secondary-color);
        margin: 0;
        display: flex;
        flex-wrap: wrap;
        gap: 15px;
    }

    .position-details span {
        display: flex;
        align-items: center;
    }

    .position-details span:before {
        content: '';
        display: inline-block;
        width: 6px;
        height: 6px;
        border-radius: 50%;
        background-color: var(--accent-color);
        margin-right: 8px;
    }

    .card-content {
        padding: 30px;
    }

    .card-description {
        margin-bottom: 25px;
    }

    .achievement-list {
        list-style-type: none;
        padding: 0;
        margin: 0;
    }

    .achievement-list li {
        padding-left: 25px;
        position: relative;
        margin-bottom: 15px;
    }

    .achievement-list li:before {
        content: '→';
        position: absolute;
        left: 0;
        color: var(--accent-color);
        font-weight: bold;
    }

    .card-tags {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
        margin-top: 30px;
    }

    .card-tag {
        font-size: 0.8rem;
        background-color: var(--light-bg);
        color: var(--secondary-color);
        padding: 6px 12px;
        border-radius: 50px;
        transition: background-color var(--transition-speed);
    }

    .card-tag:hover {
        background-color: rgba(0, 119, 181, 0.1);
    }

    @media (max-width: 768px) {
        .card-header {
            flex-direction: column;
            text-align: center;
        }
        
        .card-logo {
            margin-right: 0;
            margin-bottom: 15px;
        }
        
        .position-details {
            justify-content: center;
        }
    }
</style>

<p class="page-description">My professional journey in robotics, mechanical engineering, and manufacturing, with a focus on research and development roles.</p>

<div class="card-container">
    <!-- RROS Lab Experience -->
    <div class="card">
        <div class="card-header">
            <div class="card-logo">
                <img src="{{ site.baseurl }}/images/rros-logo.png" alt="RROS Lab Logo" onerror="this.src='{{ site.baseurl }}/assets/images/placeholder.png'">
            </div>
            <div class="card-title-area">
                <h3 class="card-title">Research Assistant</h3>
                <div class="position-details">
                    <span>Realization of RObotic Systems Lab (RROS)</span>
                    <span>May 2024 – Present</span>
                    <span>Los Angeles, CA</span>
                </div>
            </div>
        </div>
        <div class="card-content">
            <div class="card-description">
                <p>Working on advanced dual-arm robotic coordination for complex manipulation tasks, with a focus on battery disassembly workflows. The research involves integrating state-of-the-art motion planning algorithms with multi-view perception systems to enable robust automation of challenging disassembly operations.</p>
            </div>
            <ul class="achievement-list">
                <li><strong>Dual-Arm Robotic Coordination for Battery Disassembly</strong>
                    <ul>
                        <li>Engineered a dual-arm motion planning system for ABB IRB120 and KUKA iiwa 14, integrating Nvidia cuMotion library and OMPL for high-efficiency motion planning.</li>
                        <li>Developed a MoveIt! package for coordinated dual-arm trajectory planning, handling collision-aware and constraint-based manipulations.</li>
                        <li>Implemented custom motion planners for synchronized manipulation, optimizing for precision and task efficiency.</li>
                    </ul>
                </li>
                <li><strong>ROS2-Based Motion Planning & Control</strong>
                    <ul>
                        <li>Developed Python-based ROS2 control scripts using rclpy, implementing MoveIt! action clients for robotic motion execution.</li>
                        <li>Integrated ROS2 action servers and clients to coordinate task-level execution for multi-arm manipulation.</li>
                        <li>Implemented hand-eye calibration packages, enabling camera-to-end-effector alignment for enhanced perception-based grasping.</li>
                        <li>Built custom ROS2 nodes for real-time motion planning and execution, integrating sensor feedback loops for adaptive control.</li>
                    </ul>
                </li>
                <li><strong>Multi-View Perception & Visuo-Motor Learning</strong>
                    <ul>
                        <li>Designed a multi-view vision system using Intel RealSense cameras and ROS2 data streams to capture 6D object poses for visuo-motor learning.</li>
                        <li>Implemented camera-based localization and object tracking for dynamic manipulation tasks.</li>
                    </ul>
                </li>
                <li><strong>Closed-Loop Diffusion-Based Action Prediction</strong>
                    <ul>
                        <li>Operationalized diffusion-model-based action prediction to handle uncertain object geometries, ensuring robust disassembly across varying battery positions and orientations.</li>
                        <li>Integrated force-torque feedback loops for real-time corrective actions during manipulation.</li>
                        <li>Developed a differentiable optimization framework for tuning grasping and manipulation strategies dynamically.</li>
                    </ul>
                </li>
                <li><strong>Simulation & Reinforcement Learning for Grasping</strong>
                    <ul>
                        <li>Application of GraspIt! for grasp synthesis and evaluation, developed grasp evaluation pipelines using GraspIt! and MoveIt!, allowing the system to rank stable grasp candidates for manipulation.</li>
                        <li>Implementing a reinforcement learning (RL)-based grasping policies for KUKA iiwa using Stable Baselines3 (PPO, SAC) + Isaac Gym, optimizing performance for novel object geometries.</li>
                    </ul>
                </li>
                <li><strong>Wire Disassembly Using Language-Guided Manipulation</strong>
                    <ul>
                        <li>Extending the diffusion-based framework for language-conditioned robotic control, integrating natural language prompts to guide wire disassembly workflows.</li>
                        <li>Developing a language-to-motion policy for interpreting textual commands into manipulation trajectories, enhancing adaptability in unstructured environments.</li>
                    </ul>
                </li>
                <li><strong>ROS2 Implementation & Middleware Development</strong>
                    <ul>
                        <li>Developed custom ROS2 nodes for real-time motion planning, vision processing, and force-torque feedback.</li>
                        <li>Optimized ROS2 middleware communications using rclpy, ensuring low-latency data exchange and real-time execution.</li>
                        <li>Created modular ROS2 packages for trajectory optimization and multi-arm coordination, contributing to internal research repositories.</li>
                    </ul>
                </li>
                <li><strong>Dockerized ROS2 & CuMotion Deployment</strong>
                    <ul>
                        <li>Implemented cuMotion in Docker using NVIDIA Container Toolkit, enabling GPU-accelerated motion planning in ROS2 environments.</li>
                        <li>Containerized ROS2 nodes and robotic simulation environments using Docker, ensuring portable and scalable deployment.</li>
                    </ul>
                </li>
            </ul>
            <div class="card-tags">
                <span class="card-tag">ROS2</span>
                <span class="card-tag">NVIDIA cuMotion</span>
                <span class="card-tag">ABB Robots</span>
                <span class="card-tag">KUKA Robots</span>
                <span class="card-tag">Motion Planning</span>
                <span class="card-tag">Diffusion Models</span>
                <span class="card-tag">Multi-view Perception</span>
                <span class="card-tag">RealSense Cameras</span>
                <span class="card-tag">tf2</span>
                <span class="card-tag">Human-in-the-loop</span>
                <span class="card-tag">Learning from Demonstration</span>
            </div>
        </div>
    </div>
    <!-- Zhao Research Group Experience -->
    <div class="card">
        <div class="card-header">
            <div class="card-logo">
                <img src="{{ site.baseurl }}/images/zhao-grp-logo.png" alt="Zhao Research Group Logo" onerror="this.src='{{ site.baseurl }}/assets/images/placeholder.png'">
            </div>
            <div class="card-title-area">
                <h3 class="card-title">Research Assistant</h3>
                <div class="position-details">
                    <span>Zhao Research Group</span>
                    <span>September 2023 – January 2024</span>
                    <span>Los Angeles, CA</span>
                </div>
            </div>
        </div>
        <div class="card-content">
            <div class="card-description">
                <p>Contributed to research on advanced biometric sensing technologies by developing innovative soft, stretchable EMG sensors. The project focused on creating comfortable, high-fidelity sensors capable of capturing detailed muscle activity data for medical applications and human-machine interfaces.</p>
            </div>
            <ul class="achievement-list">
                <li>Engineered a soft stretchable EMG sensor with a micro-needle array in a serpentine pattern for improved muscle readings, significantly enhancing signal quality while maintaining user comfort.</li>
                <li>Optimized the design for UV resin 3D printing processes, overcoming manufacturing challenges related to feature resolution and material properties.</li>
                <li>Enhanced adhesion characteristics while maintaining flexibility, solving a key challenge in wearable sensor technology by balancing mechanical properties.</li>
                <li>Conducted extensive testing and validation of sensor performance across different motion scenarios and muscle activation patterns.</li>
            </ul>
            <div class="card-tags">
                <span class="card-tag">EMG Sensors</span>
                <span class="card-tag">Micro-needle Arrays</span>
                <span class="card-tag">Soft Electronics</span>
                <span class="card-tag">Stretchable Sensors</span>
                <span class="card-tag">UV Resin 3D Printing</span>
                <span class="card-tag">Serpentine Patterns</span>
                <span class="card-tag">Biomechanics</span>
                <span class="card-tag">Material Optimization</span>
            </div>
        </div>
    </div>
    <!-- Cosmos Cable Glands Experience -->
    <div class="card">
        <div class="card-header">
            <div class="card-logo">
                <img src="{{ site.baseurl }}/images/cosmos-logo.png" alt="Cosmos Cable Glands Logo" onerror="this.src='{{ site.baseurl }}/assets/images/placeholder.png'">
            </div>
            <div class="card-title-area">
                <h3 class="card-title">Junior Engineer Intern</h3>
                <div class="position-details">
                    <span>Cosmos Cable Glands</span>
                    <span>June 2021 – August 2021</span>
                    <span>Mumbai, India</span>
                </div>
            </div>
        </div>
        <div class="card-content">
            <div class="card-description">
                <p>Participated in the complete product development lifecycle for industrial cable gland products, from initial design through manufacturing to final testing and validation. Gained comprehensive experience in applying engineering principles to create reliable industrial components that meet stringent industry standards.</p>
            </div>
            <ul class="achievement-list">
                <li>Facilitated design, manufacturing, and testing of various types of cable glands, resulting in the successful production of 3 distinct product models with varying specifications and applications.</li>
                <li>Applied Geometric Dimensioning and Tolerancing (GD&T) principles to meet predefined manufacturing standards, ensuring consistent quality and interchangeability across production runs.</li>
                <li>Conducted ISO standard tests on prototypes and production samples, achieving an 18% increase in structural durability compared to previous product generations.</li>
                <li>Researched optimal material specifications to balance client requirements for cost, mechanical properties, and performance metrics under various environmental conditions.</li>
                <li>Collaborated with production engineers to optimize manufacturing processes, reducing waste and improving efficiency in the production line.</li>
            </ul>
            <div class="card-tags">
                <span class="card-tag">Geometric Dimensioning & Tolerancing</span>
                <span class="card-tag">ISO Standards</span>
                <span class="card-tag">Product Development</span>
                <span class="card-tag">Material Selection</span>
                <span class="card-tag">Manufacturing Processes</span>
                <span class="card-tag">Quality Control</span>
                <span class="card-tag">Durability Testing</span>
                <span class="card-tag">Industrial Components</span>
            </div>
        </div>
    </div>
</div>