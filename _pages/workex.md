---
layout: archive
title: "Work Experience"
permalink: /work-experience/
author_profile: true
---
Explore my professional journey and research contributions in robotics and mechanical engineering.

<div class="card-container">
    <div class="card">
        <div class="card-image">
            <img src="/assets/images/rros-lab.jpg" alt="RROS Lab">
        </div>
        <div class="card-content">
            <h3 class="card-title">Research Assistant</h3>
            <p class="position-details">Realization of RObotic Systems Lab (RROS) | May 2024 – Present | Los Angeles, CA</p>
            <p class="card-description">
            • Engineered a system for dual-arm coordination on ABB IRB120 and KUKA iiwa 14, integrating Nvidia cuMotion library and OMPL for high-efficiency motion planning in battery disassembly workflows<br>
            • Incorporated multi-view perception using ROS2 and RealSense data streams for 6D pose capture<br>
            • Operationalized diffusion-model-based action prediction for handling uncertain object geometry<br>
            • Developed real-time deployment workflow with data-driven trajectories
            </p>
            <div class="card-tags">
                <span class="card-tag">Robotics</span>
                <span class="card-tag">ROS2</span>
                <span class="card-tag">NVIDIA cuMotion</span>
                <span class="card-tag">Machine Learning</span>
            </div>
        </div>
    </div>
    
<div class="card">
        <div class="card-image">
            <img src="/assets/images/zhao-research.jpg" alt="Zhao Research Group">
        </div>
        <div class="card-content">
            <h3 class="card-title">Research Assistant</h3>
            <p class="position-details">Zhao Research Group | September 2023 – January 2024 | Los Angeles, CA</p>
            <p class="card-description">
            • Engineered a soft stretchable EMG sensor with a micro-needle array in a serpentine pattern for improved muscle readings<br>
            • Optimized design for UV resin 3D printing<br>
            • Enhanced adhesion while maintaining flexibility in the sensor design
            </p>
            <div class="card-tags">
                <span class="card-tag">Biomedical</span>
                <span class="card-tag">Sensors</span>
                <span class="card-tag">3D Printing</span>
                <span class="card-tag">Materials</span>
            </div>
        </div>
    </div>
    
<div class="card">
        <div class="card-image">
            <img src="/assets/images/cosmos-cable.jpg" alt="Cosmos Cable Glands">
        </div>
        <div class="card-content">
            <h3 class="card-title">Junior Engineer Intern</h3>
            <p class="position-details">Cosmos Cable Glands | June 2021 – August 2021 | Mumbai, India</p>
            <p class="card-description">
            • Facilitated design, manufacturing, and testing of various types of cable glands, resulting in production of 3 distinct product models<br>
            • Applied GD&T to meet predefined manufacturing standards<br>
            • Conducted ISO standard tests, attaining an 18% increase in structural durability<br>
            • Researched optimal material specifications for client-driven cost, properties, and performance criteria
            </p>
            <div class="card-tags">
                <span class="card-tag">Manufacturing</span>
                <span class="card-tag">Product Design</span>
                <span class="card-tag">Testing</span>
                <span class="card-tag">Standards</span>
            </div>
        </div>
    </div>
    
<div class="card">
        <div class="card-image">
            <img src="/assets/images/djs-racing.jpg" alt="DJS Racing">
        </div>
        <div class="card-content">
            <h3 class="card-title">Senior Brakes Engineer</h3>
            <p class="position-details">DJS Racing | University Project</p>
            <p class="card-description">
            • Led and mentored a 12-member team to a national competition<br>
            • Applied DFMA principles to design and manufacture custom calipers, rotors, and pedal box assemblies<br>
            • Achieved 22% weight reduction, improved ergonomics, and 27% cost reduction<br>
            • Conducted research on controlled braking for a Driverless Formula Student car
            </p>
            <div class="card-tags">
                <span class="card-tag">Automotive</span>
                <span class="card-tag">Team Leadership</span>
                <span class="card-tag">DFMA</span>
                <span class="card-tag">Mechanical Design</span>
            </div>
        </div>
    </div>
</div>

<style>
    :root {
        --primary-color: #333;
        --secondary-color: #666;
        --light-bg: #f8f9fa;
        --dark-bg: #222;
        --card-shadow: 0 4px 6px rgba(0,0,0,0.1);
        --card-hover-shadow: 0 10px 15px rgba(0,0,0,0.15);
        --transition-speed: 0.3s;
    }

    .card-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
        gap: 30px;
        margin: 50px 0 60px;
    }

    .card {
        background-color: white;
        border-radius: 8px;
        overflow: hidden;
        box-shadow: var(--card-shadow);
        transition: transform var(--transition-speed), box-shadow var(--transition-speed);
        cursor: pointer;
        height: 100%;
        display: flex;
        flex-direction: column;
    }

    .card:hover {
        transform: translateY(-5px);
        box-shadow: var(--card-hover-shadow);
    }

    .card-image {
        height: 200px;
        overflow: hidden;
    }

    .card-image img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        transition: transform 0.5s ease;
    }

    .card:hover .card-image img {
        transform: scale(1.05);
    }

    .card-content {
        padding: 25px;
        flex-grow: 1;
        display: flex;
        flex-direction: column;
    }

    .card-title {
        font-size: 1.3rem;
        margin-top: 0;
        margin-bottom: 8px;
        color: var(--dark-bg);
    }

    .position-details {
        font-size: 0.9rem;
        color: var(--secondary-color);
        margin-bottom: 15px;
        font-style: italic;
    }

    .card-description {
        color: var(--secondary-color);
        margin-bottom: 20px;
        flex-grow: 1;
        font-size: 0.9rem;
        line-height: 1.5;
    }

    .card-tags {
        display: flex;
        flex-wrap: wrap;
        gap: 6px;
        margin-top: auto;
    }

    .card-tag {
        font-size: 0.7rem;
        background-color: var(--light-bg);
        color: var(--secondary-color);
        padding: 4px 10px;
        border-radius: 50px;
    }
</style>