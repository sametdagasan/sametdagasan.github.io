---
layout: page
title: project 3
description: Activity Classification in Distributed Acoustic Sensing Systems
img: assets/img/waterfall.png
importance: 2
category: Work
giscus_comments: 
---

We developed two methods for train detection and tracking in fiber optic DAS systems, categorized into waterfall-based and spectrogram-based approaches. The former uses classical computer vision techniques, while the latter employs image processing techniques. Additionally, a neural network-based learning method is proposed. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/wf.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Waterfall image of a railroad for 11 minutes. 
</div>


Physical factors, such as temperature and strain, have a notable impact on the acquired signal in the system. In a typical DAS system, the maximum fiber optic cable length is limited to 50 km due to channel attenuation and physical constraints. The system uses a 100 ns pulse, resulting in a 10-meter spatial separation between adjacent channels. Since light travels through fibers at a speed of approximately 2.01 × 10^8 m/s, the system's sampling frequency is 2 kHz. Waterfall images are generated with signal processing using raw data obtained by sensor. 


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/algorithm.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Components of the waterfall-based detection and tracking algorithm.
</div>

Algorithm comprises of 3 modules: Bounding box detection, boundary detection and tracking. 

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/mett.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Computation of gradients and line fitting for train trace.
</div>

In the boundary detection module, the start and end points of train traces are detected using patches found in the bounding box detection module.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spectrogram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Log mel energy of a train passing.
</div>

 spectrogram provides the spectral information necessary to tell apart two signals that may appear similar because their main frequencies are similar, like low frequency noises. We use this representation to detect and track the train traces.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spectrogram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Preprocessing results of direct segmentation.
</div>

The purpose of the preprocessing is to mask noises and indicate railroad tracks. Preprocessing comprises of 4 components. We need to normalize the data through all the channels in order to compensate for the inconsistencies caused by the sensor.
