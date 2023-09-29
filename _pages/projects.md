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

Some of the key areas I specialize in include
  <ul>
    <li><strong>Advancing Functional Neuroimaging</strong>: I am dedicated to developing innovative techniques for functional neuroimaging, with a focus on near-infrared spectroscopy. My work in this area aims to provide a deeper understanding of brain activity and connectivity through graph theory and other concepts from complex systems that have the potential to unravel the intricate relationships within the brain. </li>
    <li><strong>Transform Healthcare through Diffuse Optics</strong>: I am dedicated to harnessing the potential of near-infrared spectroscopy and diffuse correlation spectroscopy to address real-world challenges in clinical settings. These technologies have the power to revolutionize healthcare by shedding light on the complex neural processes underlying various medical conditions.</li>
    <li><strong>Unraveling the Brain with Biophysical Modeling</strong>: My research extends to biophysical modelling, where I explore the interplay among neural activity, metabolism, and the regulation of blood flow. By understanding this process, we can gain insight into how the brain works in a way that enables us to design novel techniques for measuring other aspects of brain physiology. These techniques, in turn, contribute to our understanding of brain injury, neurodegenerative diseases, and mental health disorders.</li>
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
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
