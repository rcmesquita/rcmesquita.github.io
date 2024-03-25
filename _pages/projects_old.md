---
layout: page
title: projects
permalink: /projects/
description: 
  My research interests span a wide range of topics within the realm of computational neuroscience and biomedical imaging. 
nav: false
display_categories: [work] #, fun]
horizontal: false
---

This is a list of general research topics I have been working on:
  <ul>
    <li><strong>Diffuse Optics</strong>: I am dedicated to developing innovative optical methods for functional neuroimaging at the macroscale, with a focus on near-infrared spectroscopy (NIRS) techniques. My work in this area aims to build instrumentation and novel data analysis methods that can provide more accurate and reliable information about deep tissue physiology</li>
    <li><strong>Human Functional Neuroimaging</strong>: most developments in diffuse optics can be combined with biophysical modelling to better understand the interplay among neural activity, metabolism, and the regulation of blood flow. By understanding these relationships, we can gain insight into the details of brain function and the limitations of neuroimaging methods. In parallel, the knowledge of these relationships allow us to unravel the intricate relationships within the brain and its complexity.</li>
    <li><strong>Clinical Applications</strong>: the advancements of diffuse optics can be translated into clinical settings to address real-world challenges. I believe diffuse optics have the power to revolutionize healthcare by addressing niches that other current existing techniques fall short, particularly in situations where continuous, bedside monitoring can make a difference.<li>
  </ul>  
  
  
Below you can find some of the ongoing research projects I have been working on.

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}i
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div> 

