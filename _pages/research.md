---
layout: page
title: research
permalink: /projects/
description:
nav: true
nav_order: 2
display_categories: [Past Research, Ongoing Research]
horizontal: false
---

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Hydrology.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<p style="text-align: justify;">My research interests involve hydrologic science/water resources system analysis and computational modeling with an emphasis on predictive science, uncertainty analysis, data analytics, and high-performance computing. My research focuses on advancing our understanding of the interactions between climate, hydrology, and water resources using the data sets and methods including, machine learning, remote sensing, state-of-the-art data assimilation, Bayesian inference, distributed hydrologic modeling, ensemble inference, post-processing, and multi-modeling. In our research group, we study the surface and subsurface hydrologic processes and their interactions to improve the predictability of extreme hydroclimate events under the climate change. In general, we seek solutions in a multidisciplinary manner by bridging the fields of engineering, statistics, and data science.<br>


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
