---
title: "Fitness Android app"
excerpt: "App with pose detection and BLE<br/><img src='/images/portfolio/thumbnails/kettlebell.jpg'>"
collection: portfolio
date: 28-January-2022
---
Project done in collaboration with Jop Geraets and Koen Giesen. The project's source code is available [here](https://github.com/RaduLucianR/5USUA0_Luditech/tree/complete).

We went from ideation to prototyping and then to marketing of a smart kettlebell accompanied by an Android app. We called the project Luditech. Luditech would be a company of home fitness equipment whose aim is to create a smart kettlebell that gamifies fitness as their first product. With
this device one can play videogames using the kettlebell as the controller and their phone as a screen.

The Luditech app was written in Java for Android. It features authentication support, a leaderboard where users can see the highest score, BLE connection with the kettlebell, pose detection so they can adjust their pose. It uses Firebase for the database and authentication aspects, and Google's MediaPipe library for the pose detection algorithms.

I was responsible with creating the Android app and arranging the communication with the BLE module inside the kettlebell.

<div style="display: flex; flex-wrap: wrap; justify-content: space-between;">
        <img src="/images/portfolio/kettlebell/kettlebell.jpg" alt="Image 1" style="width:49%; height:10%;">
        <img src="/images/portfolio/kettlebell/circuit.jpg" alt="Image 2" style="width:49%; height:10%;">
        <figcaption style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">The kettlebell from the front and the circuit inside the kettlebell.</figcaption>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-between;">
        <img src="/images/portfolio/kettlebell/app1.jpeg" alt="Image 1" style="width:19%; height:10%;">
        <img src="/images/portfolio/kettlebell/app5.jpeg" alt="Image 2" style="width:19%; height:10%;">
        <img src="/images/portfolio/kettlebell/app2.jpeg" alt="Image 3" style="width:19%; height:10%;">
        <img src="/images/portfolio/kettlebell/app3.jpeg" alt="Image 1" style="width:19%; height:10%;">
        <img src="/images/portfolio/kettlebell/app4.jpeg" alt="Image 2" style="width:19%; height:10%;">
        <figcaption style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">Luditech app's pages. From left to right: Registration page, Login page, Pose detection page, BLE connection page, Leaderboard page.</figcaption>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-between;">
        <img src="/images/portfolio/kettlebell/Posturedetection1.png" alt="Image 1" style="width:30%; height:10%;">
        <img src="/images/portfolio/kettlebell/Posturedetection2.png" alt="Image 2" style="width:30%; height:10%;">
        <img src="/images/portfolio/kettlebell/Posturedetection3.png" alt="Image 3" style="width:30%; height:10%;">
        <figcaption style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">Posture detection trials.</figcaption>
</div>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/kettlebell/firebasedb.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Scores of users stored in Firebase.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/kettlebell/authentication.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Account database in Firebase.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/kettlebell/architecture.jpg' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Architecture of the system.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/kettlebell/datastream.png' style="display: block; margin-left: auto; margin-right: auto; width:90%">
    <figcaption>Datastream through the system.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/kettlebell/seq3.jpg' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Sequence diagram of the sytem.</figcaption>
</figure>