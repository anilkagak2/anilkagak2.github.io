---
layout: page
title: research
permalink: /research/
description: A thematic breakdown of my research along with highlighted papers.
nav: true
nav_order: 2
_styles: >
  .research-category {
    margin-bottom: 1.5rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.5rem;
    overflow: hidden;
    background-color: var(--global-bg-color);
  }
  .category-header {
    padding: 1rem 1.5rem;
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: var(--global-card-bg-color);
    transition: background-color 0.2s ease;
  }
  .category-header:hover {
    background-color: var(--global-hover-color);
  }
  .category-title-container {
    display: flex;
    flex-direction: column;
  }
  .category-title {
    margin: 0 !important;
    font-size: 1.25rem;
    font-weight: 600;
  }
  .category-description {
    margin: 0.25rem 0 0 0 !important;
    font-size: 0.9rem;
    color: var(--global-text-color-light);
  }
  .category-icon {
    transition: transform 0.3s ease;
    font-size: 1.2rem;
    color: var(--global-theme-color);
  }
  .research-category.active .category-icon {
    transform: rotate(180deg);
  }
  .category-content {
    display: none;
    padding: 1.5rem;
    border-top: 1px solid var(--global-divider-color);
  }
  .research-category.active .category-content {
    display: block;
  }
  /* Ensure bibliography entries look good inside the toggle */
  .category-content .publications {
    margin-top: 0;
  }
---

<div class="research-themes">

  <div class="research-category">
    <div class="category-header" onclick="this.parentElement.classList.toggle('active')">
      <div class="category-title-container">
        <h2 class="category-title">Foundational Image Gen</h2>
        <p class="category-description">Architecting efficient, high-resolution diffusion models for edge and large-scale deployment.</p>
      </div>
      <i class="fas fa-chevron-down category-icon"></i>
    </div>
    <div class="category-content">
      <div class="publications">
        {% bibliography -f papers --query @*[keywords~=foundational-image-gen]* %}
      </div>
    </div>
  </div>

  <div class="research-category">
    <div class="category-header" onclick="this.parentElement.classList.toggle('active')">
      <div class="category-title-container">
        <h2 class="category-title">Foundational Video Gen</h2>
        <p class="category-description">Pioneering high-fidelity, spatiotemporal transformers for mobile and server-side synthesis.</p>
      </div>
      <i class="fas fa-chevron-down category-icon"></i>
    </div>
    <div class="category-content">
      <div class="publications">
        {% bibliography -f papers --query @*[keywords~=foundational-video-gen]* %}
      </div>
    </div>
  </div>

  <div class="research-category">
    <div class="category-header" onclick="this.parentElement.classList.toggle('active')">
      <div class="category-title-container">
        <h2 class="category-title">RLHF & Alignment</h2>
        <p class="category-description">Advancing preference optimization and reward flow frameworks for generative model fine-tuning.</p>
      </div>
      <i class="fas fa-chevron-down category-icon"></i>
    </div>
    <div class="category-content">
      <div class="publications">
        {% bibliography -f papers --query @*[keywords~=rlhf-alignment]* %}
      </div>
    </div>
  </div>

  <div class="research-category">
    <div class="category-header" onclick="this.parentElement.classList.toggle('active')">
      <div class="category-title-container">
        <h2 class="category-title">Adaptive & Hardness-Aware</h2>
        <p class="category-description">Developing intelligent systems that adapt model complexity based on input difficulty.</p>
      </div>
      <i class="fas fa-chevron-down category-icon"></i>
    </div>
    <div class="category-content">
      <div class="publications">
        {% bibliography -f papers --query @*[keywords~=adaptive-hardness]* %}
      </div>
    </div>
  </div>

  <div class="research-category">
    <div class="category-header" onclick="this.parentElement.classList.toggle('active')">
      <div class="category-title-container">
        <h2 class="category-title">Efficient RNN/CNN</h2>
        <p class="category-description">Fundamental breakthroughs in low-complexity architectural design and optimization.</p>
      </div>
      <i class="fas fa-chevron-down category-icon"></i>
    </div>
    <div class="category-content">
      <div class="publications">
        {% bibliography -f papers --query @*[keywords~=efficient-architectures]* %}
      </div>
    </div>
  </div>

  <div class="research-category">
    <div class="category-header" onclick="this.parentElement.classList.toggle('active')">
      <div class="category-title-container">
        <h2 class="category-title">Extreme Classification</h2>
        <p class="category-description">Architecting industrial-scale recommendation systems for millions of labels.</p>
      </div>
      <i class="fas fa-chevron-down category-icon"></i>
    </div>
    <div class="category-content">
      <div class="publications">
        {% bibliography -f papers --query @*[keywords~=extreme-classification]* %}
      </div>
    </div>
  </div>

</div>
