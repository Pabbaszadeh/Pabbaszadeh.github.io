---
layout: page
permalink: /research/
title: research
description:
nav: true
nav_order: 5
---

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Rsearch_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<p style="text-align: justify;">My research interests involve hydrologic science/water resources system analysis and computational modeling with an emphasis on predictive science, uncertainty analysis, data analytics, and high-performance computing. My research in general focuses on advancing our understanding of the interactions between climate, hydrology, and water resources using the data sets and methods including, machine learning, remote sensing, state-of-the-art data assimilation, Bayesian inference, distributed hydrologic modeling, ensemble inference, post-processing, and multi-modeling. My diverse background and contribution to engineering projects have provided me with a broad overview of climate-water interactions and motivated me to seek solutions in a multidisciplinary manner by bridging the fields of engineering, statistics, and data science. This page gives a brief overview of past research efforts and summarizes my current research directions.<br><br>

<strong style="font-size: 24px;">Past Research</strong><br>
Below is the summary of some of the projects that I worked on in collaboration with Ph.D. students, postdocs, faculties, and scientists from multiple departments and national agencies.<br><br>

<strong style="font-size: 16px;">Hydrologic Data Assimilation:</strong><br>
Coupling a deterministic four-dimensional variational (4DVAR) assimilation method with the Particle Filter (PF) ensemble data assimilation system, to produce a robust approach for dual-state-parameter estimation. In our proposed method, the Hybrid Ensemble and Variational Data Assimilation framework for Environmental systems (HEAVEN), we characterize the model structural uncertainty in addition to model parameter and input uncertainties. Link to <a href=" https://doi.org/10.1029/2018WR023629">paper</a><br>

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Figure1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<br>

The following figure shows the Evolutionary Particle Filter with MCMC (EPFM) algorithm. In this algorithm, the prior distribution undergoes an evolutionary process based on the designed mutation and crossover operators of GA. The merit of this approach is that the particles move to an appropriate position by using the GA optimization and then the number of effective particles is increased by means of MCMC, whereby the particle degeneracy is avoided and the particle diversity is improved. Link to <a href=" https://doi.org/10.1016/j.advwatres.2017.11.011">paper</a><br><br>

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Figure 2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<br>

<strong style="font-size: 16px;">Drought Monitoring and Forecasting:</strong><br>
Assimilating two remotely sensed datasets, namely, Soil Moisture Operational Product System (SMOPS) and MODIS (Moderate Resolution Imaging Spectroradiometer) evapotranspiration (MODIS16 ET), at the 1-km spatial resolution, into the Variable Infiltration Capacity (VIC) hydrologic model using EPFM (Evolutionary Particle Filter with MCMC) approach for drought monitoring across Apalachicola–Chattahoochee–Flint (ACF) Basin in the southeastern United States.<br><br>

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Research_3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>