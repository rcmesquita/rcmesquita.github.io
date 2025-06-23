---
layout: page
title: research themes
permalink: /research_themes/
nav: false
horizontal: false
---

<!--
Optical imaging through near-infrared as unifying theme 
-->

Light has long been used for characterizing a broad spectrum of samples. One of the simplest techniques relies on light absorption, which provides information on the presence and concentration of molecules in a sample based on their specific absorption characteristics. Light scattering experiments reveal sample morphology, including the size and refractive indices of scatterers, as well as the structural organization of scatterer collections. Techniques such as dynamic or quasi-elastic light scattering provide insight into the motion of scatterers by analyzing temporal variations in scattered light intensity. These optical spectroscopic techniques are well-established for simple, homogeneous, and optically thin samples.

Diffuse optics focuses on light propagation in highly scattering media (also called turbid media), where scattering dominates over absorption. Such media are can be found in various fields, including biology, environmental science, and atmospheric studies. For example, colloids, which are suspensions of particles in a fluid, scatter light significantly and are a common subject of study in diffuse optics. Near-infrared light (~700-900 nm) is also extensively scattered by biological tissues, due to their heterogeneity. Similarly, environments like soil, water, and atmospheric conditions contain particles and impurities that scatter light. Diffuse optics provides a framework for understanding and predicting light behavior in these complex, inhomogeneous media.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Scattering_10.jpg" title="Light propagation in a turbid medium" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Modeling light propagation in diffusive media can be approached through deterministic analytical or computational models, as well as stochastic methods like Monte Carlo simulations. Regardless of the approach, these models have one common goal: given the optical properties of the medium such as absorption and scattering coefficients, they aim to estimate observable experimental quantities, such as the light intensity detected at the medium's surface. 

Diffuse optical techniques use these measured optical quantities to recover the optical properties of a diffusive medium. These experimental techniques can be broadly classified into static and dynamic methods. Static methods focus on slow variations in absorption and scattering, while dynamic methods monitor speckle fluctuations in scattered light, which are sensitive to the motion of scatterers. 


### Functional Near-Infrared Spectroscopy (fNIRS)

Functional Near-Infrared Spectroscopy (fNIRS) typically refers to the use of continuous-wave near-infrared light to monitor relative changes in the detected light intensity of highly scattering media over time. In fNIRS, these changes are primarily interpreted as changes in absorption. fNIRS is widely adopted in functional neuroscience, as changes in absorption reflect changes in cerebral oxygenation, providing a non-invasive method to study brain activity. Recent advances in photonics and microelectronics have enabled the development of wearable, high-density fNIRS devices, making it possible to study brain function in natural environments, which is challenging with other neuroimaging techniques like fMRI or PET. In addition, fNIRS is more robust to motion artifacts compared to EEG, making it valuable for studying early brain development. Our lab has studied newborns and neonates as young as 20 days old using fNIRS.

In our lab, we focus on using fNIRS to explore the spatiotemporal relationships between different brain regions and their relevance to brain health and development. We also develop and evaluate more precise methods to improve fNIRS reproducibility across and within subjects, with a focus on studying functional neuroplasticity, i.e., the brain's remarkable ability to adapt and learn. This has applications ranging from cognitive and developmental neuroscience to rehabilitation.


### Diffuse Optical Spectroscopy (DOS)

Diffuse Optical Spectroscopy (DOS) employs time-resolved or frequency-domain techniques to quantify media's absorption and scattering properties. Time-resolved methods measure the number of photons detected over time after a light pulse, while frequency-domain techniques involve modulating the light source and analyzing the detected light's amplitude and phase shift.

By separating absorption from scattering, DOS provides quantitative information about tissue composition, such as blood oxygen saturation, total hemoglobin concentration, and water content in deep tissues like the brain or muscle. For this reason, DOS has been widely adopted in medical research targeting diagnostics and monitoring. Examples include the use of FD-DOS for tumor detection and chemotherapy follow-ups, and the monitor of patients diagnosed with chronic diseases or acute injuries. The ability to provided quantitative information is particularly valuable for longitudinal measurements. 

However, accurately separating absorption and scattering is an ill-posed problem, and there are a few intrinsic limitations such as partial volume effects. In our lab, we are interested in developing methods to improve the accuracy of DOS measurements, particularly in the frequency domain.


### Diffuse Correlation Spectroscopy (DCS)

Diffuse Correlation Spectroscopy (DCS) measures temporal or spatial fluctuations in scattered light, caused by moving scatterers in the medium. In biological applications, DCS provides an indirect measure of blood flow, since red blood cells are the major moving scatterers in tissue. The technique offers a non-invasive, real-time method for assessing tissue perfusion, making it particularly useful in clinical settings. In addition combining DCS with DOS allows for estimates of tissue metabolism, including the metabolic rate of oxygen consumption, a critical parameter for clinical applications.

Our lab uses DCS to monitor blood flow in critical scenarios, such as in neuro-intensive care units (ICUs) for patients with acute brain injuries (e.g., stroke or trauma) and during surgical procedures. We develop custom devices to optimize temporal resolution and measurement precision, enabling us to advance beyond blood flow assessments and gain a more comprehensive understanding of tissue physiology from optical methods. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <a href="/diffuse-optics/">
            Quantitative Optical Imaging: Methods, Models, and Instrumentation
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        Network Neuroscience with fNIRS: Complexity, Connectivity, and Brain Dynamic
    </div>
    <div class="col-sm mt-3 mt-md-0">
        Clinical and Translational Neurophotonics
    </div>
</div>

<!--
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <a href="/diffuse-optics/">
            {% include figure.html path="assets/img/diffuse-optics.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ComplexSystems.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ML4H.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

-->

