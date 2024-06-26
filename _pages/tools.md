---
layout: page
permalink: /tools/
title: tools
description: A list of developed solutions available for other researchers. #Edit the `_data/repositories.yml` and change the `github_users` and `github_repos` lists to include your own GitHub profile and repositories.
nav: true
nav_order: 4
---

Over the years, our research efforts have led to novel solutions that we attempt to make available to the wider community in applied research and companies interested in accelerating neuroscience and/or healthcare. 


## patents

* Busch, David R.; Parthasarathy, Ashwin B.; Baker, Wesley B.; Chandra, Malavika; Mesquita, Rickson C.; Licht, Daniel J.; Yodh, Arjun G.; Abramson, Kenneth (2020). *Pressure modulation, motion detection, individualized geometry, and improved optic-skin coupling to improve long term clinical monitoring with diffuse optics.* US 10,827,976. USPTO [(link)](https://patents.google.com/patent/US10827976B2/en)

* Baker, Wesley B.; Yodh, Arjun G.; Busch, David R.; Parthasarathy, Ashwin B.; Mesquita, Rickson C.; Chandra, Malavika (2019). *Probes and pressure modulation algorithms for reducing extratissue contamination in hemodynamic measurement.* US 10,342,488. USPTO [(link)](https://patents.google.com/patent/US10342488B2/en)

* Floyd, Thomas F.; Yodh, Arjun G.; Mesquita, Rickson C. (2018). *Fiber optic flow and oxygenation monitoring using diffuse correlation and reflectance.* US 10,064,554. USPTO [(link)](https://patents.google.com/patent/WO2013090658A1/en)

---

## instruments

<div class="row justify-content-sm-center" style="margin-top: 20px;">
    <div class="col-sm-8 mt-3 mt-md-0">
        <h5><strong>real-time metabolic monitor</strong></h5>
        The metabolic monitor is a hybrid optical system combining diffuse optical spectroscopy (DOS) and diffuse correlation spectroscopy (DCS) to measure simultaneous blood flow and oxygenation. By combining these two physiological parameters one can estimate relative changes in metabolic rate of oxygen (MRO<sub>2</sub>) to provide a noninvasive, all-optical measurement of metabolic and hemodynamic of tissue in vivo. Our current version of the metabolic monitor employs a commercial frequency-domain (FD) DOS with 8 sources (each source has 4 wavelengths) and 4 detectors, and a homemade DCS module with 1 source and 16 detectors. The system is used for research purposes, only (i.e., it is not yet approved for wide clinical use).
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/dcs-unicamp.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

## software

<div class="row justify-content-sm-center" style="margin-top: 20px;">
    <div class="col-sm-6 mt-3 mt-md-0">
        <h5><strong>neuronavigator</strong></h5>
        VMTK-Neuro is a suite of visual manipulation tools for neuroimages developed at the University of Campinas, Brazil. The fNIRS neuronavigation tool was part of José A. Iván's Ph.D. under the supervision of Dr. Wu Shin-Ting, and a Windows-based version can be downloaded <a href="http://www.dca.fee.unicamp.br/projects/mtk/rubianesD/files/VMTK-NIRS_Neuronavegation_ICP.zip" target="_new">here</a>. The neuronavigation function requires the <a href="https://polhemus.com/motion-tracking/all-trackers/fastrak" target="_new">Fastrak Polhemus</a> digitizer. Please check the <a href="https://www.dca.fee.unicamp.br/projects/mtk/rubianesD/videos.html" target="_new">tutorial webpage</a> (in Portuguese) to see how to install and use the neuronavigator.
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/vmtk-neuronavigator.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


---

<!-- ## GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
  {% if site.data.repositories.github_users.size > 1 %}
  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.html username=user %}
  </div>

  ---

{% endfor %}
{% endif %}
{% endif %} -->

## public repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %} 
