---
layout: page
title: project 3
description: Activity Classification in Distributed Acoustic Sensing Systems
img: assets/img/waterfall.png
importance: 2
category: Work
giscus_comments: 
---

An exploration of Fiber optic-based DAS (distributed acoustic sensing) systems for intrusion detection and classification across extended distances of up to 50 kilometers, all at an affordable cost is presented. Our work focuses on solving the activity classification challenge within fiber optic DAS systems using a machine learning approach. We employ various neural network architectures, each designed with specific inductive biases tailored to the task at hand. The models we evaluate include CNN7 (a 7-layer convolutional neural network), CNN9 (a 9-layer convolutional neural network), CRNN (convolutional recurrent network), and ViT (vision transformer). To feed these models, we use mel-spectrogram features as input images and present the test results for each of these architectures. Our results indicate that CNN9, despite being a deeper version of CNN7 with fewer parameters, outperforms the other three architectures in terms of the weighted f1-score.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/raw_data.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Raw sensor data obtained from the distributed acoustic sensing system.
</div>

The Mel scale is designed to replicate the way the human ear processes sound, as studies have revealed that our perception of frequencies is not linear. In our examination of the data, we observed that the distribution of frequencies related to the activities in the DAS system is also non-linear. Consequently, rather than utilizing traditional spectrograms, we opted to employ log-mel energies, which represent the logarithmic values of the mel spectrogram.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/spectrogram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Mel spectrogram images as feature extraction.
</div>

t-SNE is a statistical technique for visualizing data with many dimensions by mapping each data point to a two- or three-dimensional space. It's effective for reducing the dimensionality of high-dimensional data to make it suitable for visualization in a lower-dimensional space. t-SNE positions data points in such a way that similar objects are close together, while dissimilar objects are far apart in the reduced space. In this project, t-SNE was used to evaluate the use of log-mel energies as features compared to raw data. The results depicted in Figure indicate that log-mel energies offer advantages, as data points from the same class are more tightly clustered, making them a valuable feature for network usage.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/t-sne.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Effect of feature extraction can be seen from the t-sne comparison between raw data and features.
</div>

Training set accuracy, validation set accuracy (smoothed), training loss, and validation loss (smoothed) during training helps us to choose the model that we are going to use.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/learning.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Training set accuracy, validation set accuracy (smoothed), training loss, and validation loss (smoothed) during training.
</div>
