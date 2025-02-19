---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---
Explore my research and development work across various domains.

<div class="card-container">
    {% for project in site.projects %}
    <div class="card" onclick="location.href='{{ project.url | relative_url }}';">
        <div class="card-image">
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }} Image">
        </div>
        <div class="card-content">
            <h3 class="card-title">{{ project.title }}</h3>
            <p class="card-description">{{ project.description }}</p>
            <div class="card-tags">
                {% for tag in project.tags %}
                <span class="card-tag">{{ tag }}</span>
                {% endfor %}
            </div>
            <a href="{{ project.url | relative_url }}" class="project-link">View details →</a>
        </div>
    </div>
    {% endfor %}
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
        margin-bottom: 15px;
        color: var(--dark-bg);
    }

    .card-description {
        color: var(--secondary-color);
        margin-bottom: 20px;
        flex-grow: 1;
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

    .project-link {
        display: inline-block;
        margin-top: 15px;
        color: #000;
        text-decoration: none;
        font-weight: 500;
        font-size: 0.9rem;
        transition: color var(--transition-speed);
    }

    .project-link:hover {
        color: #555;
    }
</style>
