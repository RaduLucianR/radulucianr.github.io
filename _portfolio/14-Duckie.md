---
title: "DuckieBot with ROS & YOLO"
excerpt: "<img src='/images/portfolio/thumbnails/duckie.jpg'>"
collection: portfolio
date: 25-June-2023
---
**Project attribution**: Project done with Ahmed Ghanem. <br>
**Source**: The project's files are available [here](https://github.com/RaduLucianR/ros-duckie). <br>
**Short description**: DuckieBot with ROS2 and YOLOv5 <br>
**Technologies**: Python, ROS2, YOLOv5 <br>
**What I did**: I assembled the DuckieBot, extended its ROS2 architecture to use a YOLOv5 model, I made a custom dataset and trained YOLOv5 on it.

We assembled a [Duckiebot](https://duckietown.com/platform/) as part of the Embedded Visual Control course at TU Eindhoven.

We trained a YOLOv5 computer vision model on a custom dataset with traffic signs. Initially, we used [this](https://universe.roboflow.com/usmanchaudhry622-gmail-com/traffic-and-road-signs) traffic signs dataset available on [Robotflow](https://roboflow.com/). However, I deemed it insufficient for our case, so I extended it by annotating custom traffic signs on our own. You can see the final dataset [here](https://universe.roboflow.com/whatever-7klrp/traffic-sign-hmdah/dataset/1). My dataset includes more angles, more distortion, and images that closer resemble the environment that the Duckiebot would drive in. This makes it much more precise in its distinction between particular traffic signs, e.g. 20 km speed traffic sign vs 30 km speed traffic sign.

### DuckieBot
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/duckie/leftturn.gif' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>The DuckieBot taking a left turn because it detects a left-turn sign.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/duckie/duckie_control.gif' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Controlling the DuckieBot with the 20 km speed sign and the stop sign. The DuckieBot accelerates when detecting the 20 km speed sign and stops when detecting the stop sign.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/duckie/duckie_stop.gif' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>The DuckieBot stops when detecting duckies, because it doesn't want to injure duckies :)</figcaption>
</figure>

### ROS
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/duckie/ros_graph.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>The graph of ROS2 nodes running on the DuckieBot.</figcaption>
</figure>

### YOLO model
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/duckie/confusion_matrix.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Confusion matrix of the YOLO model. Notice that duckies are often confused with the background.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/duckie/pr_curve.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Precision-Recall curve of the YOLO model.</figcaption>
</figure>