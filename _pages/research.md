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

<br>
<p style="text-align: justify;">Welcome to our research lab, where we are dedicated to advancing hydrologic science and water resources system analysis through cutting-edge research. Our focus lies in predictive science, uncertainty analysis, data analytics, and high-performance computing, with a primary emphasis on addressing the challenges posed by climate change. At the heart of our research is a multidisciplinary approach that integrates engineering, statistics, and data science to deepen our understanding of the interactions between climate, hydrology, and water resources. Leveraging state-of-the-art methodologies such as machine learning, remote sensing, and advanced data assimilation techniques, we develop predictive models capable of simulating complex hydrologic processes with unprecedented accuracy and reliability. Through innovative techniques such as Bayesian inference, ensemble simulation, and multi-modeling approaches, we enhance the reliability of our predictive models and decision-making processes in the face of uncertain future climate conditions. In our research group, we study surface and subsurface hydrologic processes and their interactions to improve the predictability of extreme hydroclimate events under climate change. Furthermore, our lab is committed to developing novel methodologies for post-processing and analyzing large-scale hydrologic datasets. By extracting actionable insights from these datasets, we aim to inform more effective water resource management practices and policy decisions. Through our collaborative and interdisciplinary approach, we strive to contribute to the development of sustainable and resilient water resource systems that can withstand the challenges posed by a changing climate.<br>


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
