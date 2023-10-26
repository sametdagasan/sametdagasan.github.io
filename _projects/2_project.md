---
layout: page
title: project 2
description: a project with a background image and giscus comments
img: assets/img/waterfall.png
importance: 2
category: Work
giscus_comments: true
---

we present an exploration of Fiber optic-based DAS (distributed acoustic sensing) systems for intrusion detection and classification across extended distances of up to 50 kilometers, all at an affordable cost. Our work focuses on solving the activity classification challenge within fiber optic DAS systems using a machine learning approach. We employ various neural network architectures, each designed with specific inductive biases tailored to the task at hand. The models we evaluate include CNN7 (a 7-layer convolutional neural network), CNN9 (a 9-layer convolutional neural network), CRNN (convolutional recurrent network), and ViT (vision transformer). To feed these models, we use mel-spectrogram features as input images and present the test results for each of these architectures. Our results indicate that CNN9, despite being a deeper version of CNN7 with fewer parameters, outperforms the other three architectures in terms of the weighted f1-score.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/raw_data.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spectrogram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/t-sne.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/learning.pdf" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>
