---
title: "OpenGL Sandbox"
excerpt: "<img src='/images/portfolio/thumbnails/opengl.png'>"
collection: portfolio
date: 28-October-2020
---
**Project attribution**: Project done in collaboration with Teodor Lungu. <br>
**Source**: The project's source code is available in a private Github repository. <br>
**Short description**: 3D scene of a playground with a carousel and first-person camera.<br>
**Technologies**: Java, [OpenGL](https://www.opengl.org/), [GLSL](https://en.wikipedia.org/wiki/OpenGL_Shading_Language), [JOGL](https://jogamp.org/jogl/www/). <br>
**What I did**: I implemented some of the 3D objects, the first-person and third-person cameras, the Bezier curve algorithm ([De Casteljau](https://en.wikipedia.org/wiki/De_Casteljau%27s_algorithm)), the train and its animation.

Amusement park scene created from scratch with JOGL, the Java binding of OpenGL. The scene includes:
* Custom made 3D models directly in OpenGL
* Texture mapped on a path
* Phong shader for lightning
* Bezier curve to model the path
* Basic animation of the carousel and of the train on the path
* First-person camera
* Third-person camera
* Checkbox to enable/disable features
* Sliders to control size of the carousel and its speed of rotation

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/opengl/allview.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>Overview of the created scene, including: carousel, train, path, trees, light poles, stall.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/opengl/controlpoints.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>Control points of the Bezier curve that draws the path.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/opengl/cpcarousel.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>The carousel with the path, showing the checkbox options.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/opengl/cptrees.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/opengl/firstperson.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>First-person view.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/opengl/maximumsize.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>Maximum size carousel.</figcaption>
</figure>
