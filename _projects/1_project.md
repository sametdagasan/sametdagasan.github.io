---
layout: page
title: Fiber Optic Cable Termination and Signal Loss Detection in DAS Systems
description: 
img: assets/img/raw_data_yeni_bg.png
importance: 2
category: Work
giscus_comments: 
---

Fiber Optic Distributed Acoustic Sensing (DAS) Systems use standard telecommunication fibers to detect acoustic vibrations up to 50 kms along the cable. In this paper we propose algorithms to detect fiber optic cable termination points and optical signal losses using DAS data. Proposed algorithms add traditional Optical Time-Domain Reflectometer (OTDR) measurement functionality to the DAS systems. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/raw_data_yeni.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Raw data obtained by sensor.
</div>

Cable termination detection algorithm models the noise data in DAS signal that consists of electronic noise [e.g. Analog-to-Digital Converter (ADC) noises] and optical laser reflection noise. The cable termination detection algorithm analyzes noise statistics of the sensor data and finds the location where optic noise is no longer present. Signal loss detection algorithm first eliminates the environmental acoustic noise from the DAS signal; then, change point detection algorithm is applied to detect locations where significant signal loss occurs. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/kanal_std.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/weak.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Algorithm results. On the left, the termination point is detected. Right, signal level drops significantly.
</div>

Proposed algorithms are tested in various DAS installations in Turkey. Predicted cable termination and signal loss locations agree with OTDR measurements.