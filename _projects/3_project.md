---
layout: page
title: Model, Color and License Plate Recognition System Using Cameras Placed in Moving Vehicles
description: 
img: assets/img/CarCamBG.jpg
importance: 4
category: Work
related_publications: 
---


The project is a security-focused system that uses an IP camera mounted on a vehicle to recognize and process data about nearby vehicles. It provides output information, including license plates, color, brand, and model of vehicles within a 3-5 meter range. The project involves several steps, including dataset creation and training of learning algorithms. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/CarCamFull.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Scenario of tracking a vehicle. 
</div>

The project aims to improve stolen vehicle detection using license plate recognition. Traditional systems use fixed MOBESE or police vehicle cameras to compare recognized plates with a blacklist database. However, this method can fail when thieves replace the stolen vehicle's plate. In this project, a mobile system mounted on moving vehicles is proposed. It recognizes license plates from rear vehicle images, identifies color, brand, and model, and compares this data with registered information to detect illegal or stolen vehicles. This approach enhances stolen vehicle detection.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/CarCamFull2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Big Picture.
</div>

Tests are conducted under varying weather conditions, resulting in recognition accuracies of 95% for license plate recognition, 96% for brand recognition, 70% for model recognition, and 94% for color recognition.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/CarCam1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/CarCam2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Frames from a demo video taken on traffic while the system is online. 
</div>