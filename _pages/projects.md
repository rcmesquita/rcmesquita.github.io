---
layout: page
title: projects
permalink: /projects/
description: 
  My research interests span a wide range of topics within the realm of computational neuroscience and biomedical imaging. 
nav: false
display_categories: [work, fun]
horizontal: false
---

Some of the key areas I specialize in include
  <ul>
    <li><strong>Graph Theory and Complex Systems</strong>: I apply graph theory and concepts from complex systems to analyze brain networks and their dynamics. This allows us to unravel the intricate relationships within the brain.
    <li><strong>Clinical Applications</strong>: I am dedicated to harnessing the potential of functional near-infrared spectroscopy and diffuse correlation spectroscopy to address real-world challenges in clinical settings. These technologies have the power to transform healthcare by shedding light on the complex neural processes underlying various medical conditions.
    <li><strong>Biophysical Modeling of Neurovascular Coupling</strong>: My research extends to biophysical modeling, where I explore the intricate relationship between neural activity and blood flow regulation. This area of study has profound implications for our understanding of neurovascular coupling, a fundamental aspect of brain function.
  </ul>


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
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
