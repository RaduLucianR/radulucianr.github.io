---
title: "Eye-tracking visualizer"
excerpt: "<img src='/images/portfolio/thumbnails/eyetracking.png'>"
collection: portfolio
date: 03-July-2020
---
Project done in a SCRUM team along with Mino Keuren, Teun Kortekaas, Valentijn van den Berg, Rick van der Heijden and Kelvin Toonen.

Website written in Python with the Flask library that provides visualizations for eye-tracking data.
The visualizations were made with the Bokeh library.
The used dataset was of metro maps, however the website can display any eye-tracking data for any other use case.

The website provides the following visualizations:
* Heat map
* Gaze stripes
* Eye cloud
* Time plot

My main contributions were with the heat map and time plot.

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/eyetracking/GUI.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>Graphical User Interface used by the end-user to analyze eye-tracking data. It contains: (1) A menu for the different visualizations and the dashboard where the interactions and filters can be controlled. (2) Button that would open the Settings for this visualization. (3) Several tools for exploring the graph. (4) Sliders to change the look of the graph.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/eyetracking/attention_map_2.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Heat map. The gradient goes from green (least attention) to red (highest attention). It can be used to observe the focus
    points of the person that looks at the metro map.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/eyetracking/attention_map_display.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Filtered heat map that highlights the highest-value points.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/eyetracking/eye_clouds.png' style="display: block; margin-left: auto; margin-right: auto; width:60%">
    <figcaption>Eye clouds. The bigger circles show the most interesting areas for the end-user.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/eyetracking/gaze_stripes_interval.png' style="display: block; margin-left: auto; margin-right: auto; width:85%">
    <figcaption>Gaze stripes show the areas and the order in which the end-users looked at them.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/eyetracking/time_plot.png' style="display: block; margin-left: auto; margin-right: auto; width:60%">
    <figcaption>The time plot shows the transition between areas on the metro maps. The eye-tracking dataset is split into 5 clusters
    and the time plot highlights the transition between them. The larger circles on the time plot signify a higher attention given by the end-user.
    </figcaption>
</figure>