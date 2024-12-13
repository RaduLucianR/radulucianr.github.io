---
title: "Logistics robots with ROS"
excerpt: "<img src='/images/portfolio/thumbnails/logistics.png'>"
collection: portfolio
date: 07-July-2022
---
**Project attribution**: Project done in a team of 10 Computer Science and Engineering students. <br>
**Source**: The project was done for Starnus Technology, so the files are not open source. <br>
**Short description**: ROS architecture with SPI back-end for RC car. <br>
**Technologies**: ROS, C++, Gazebo, Springboot, Vue. <br>
**What I did**: I designed the ROS architecture, implemented ROS1 C++ nodes, created the Gazebo simulation. Participated in the design of the overall architecture comprising of the Vue web app, the Springboot server and the ROS robot backend.

This was my Bachelor End Project for my Bachelor of Computer Science and Engineering. It was done for a startup from TU Eindhoven called [Starnus Technology](https://www.starnustech.com/), a company that wanted to make modular robotics for logistics applications, like warehouse use. Since then the startup changed their trajectory from robotics to AI software.

Starnus required a web application that could send missions to robots in the warehouse, as well as the actual software that controls the robots from their current location to a destination while avoiding obstacles. I focused on the ROS back-end that achieved the second goal.

### Architecture
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/project_big_picture.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>High-level architecture of the project. I focused on the backend and the robot parts.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/high_level_archi.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>High-level architecture of the technologies of the project.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/detailed_archi.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Detailed architecture of the technologies of the project.</figcaption>
</figure>

### ROS
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/joystick.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Closeup of the robot in the Gazebo simulator. A user can directly control the robot via a package that implements a GUI joystick. This joystick is accessible in the Vue web app as well.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/rosgraph.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>Reduced ROS graph of the robot software. The websocket node and the mission sender node are the ones that we added.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/gazebo_world.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>The robot in a square warehouse in the Gazebo simulator.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/rviz.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>View of rviz that displays the direction vectors of the robot on its path to the destination.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/rtabmap.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>View of RTABmap, the SLAM algorithm that we used to create a map of the warehouse.</figcaption>
</figure>

### Vue web app
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/webapp.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>The web application interface. On the left panel you can see the joystick. On the right panel you can see the square world seen by the robot. The green circle is the robot. The yellow circles are waypoints to which the robot navigates. The yellow square represents a priority area which the robot will priorities in its path, i.e. it will first path through that area on its way to the waypoints.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/logistics/mission_creation.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>A user can create new missions with many destinations for each robot. Here is the panel that can do that.</figcaption>
</figure>