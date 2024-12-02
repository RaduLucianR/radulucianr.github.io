---
title: "Bare-metal Sobel"
excerpt: "<img src='/images/portfolio/thumbnails/bareMetal.png'>"
collection: portfolio
date: 29-June-2023
---
**Project attribution**: Project done with Eric Abraham. <br>
**Source**: The project's source code is available [here](https://github.com/RaduLucianR/esl). <br>
**Short description**: Bare-metal C program that parallelizes the Sobel algorithm. <br>
**Technologies**: C <br>
**What I did**: I designed and implemented parts of the custom FIFO, the data-parallel version, and parts of the hybrid version.

The code was written for the [CompSoC platform](http://compsoc.eu/) developed at TU Eindhoven. The CompSoC platform is highly configurable, and can be set to have multiple RISC-V processor tiles, each managing a number of partitions. For this project we had 3 processor tiles, each with 3 partitions that could perform computations in parallel.

The Sobel algorithm is a classical computer vision algorithm that is used to detect edges of objects in images. It consists of 4 phases:
1. Greyscale - transform the image to black & white
2. Convolution - apply smoothing kernels to reduce noise in the image
3. Sobel - apply the Sobel kernel to detect edges
4. Overlay - apply the detected edges over the original image

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/bareMetal/data_parallel.png' style="display: block; margin-left: auto; margin-right: auto; width:60%">
    <figcaption>Data parallel implementation. The image is split in two halves: upper and lower. We apply all steps of the Sobel algorithm on each half separetely, and then we merge them.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/bareMetal/function_parallel.png' style="display: block; margin-left: auto; margin-right: auto; width:60%">
    <figcaption>Function parallel implementation. Each step of the algorithm is executed on a different partition for a full image. This allows us to process different images in parallel for different steps of the algorithm. E.g. when we apply convolution on one image, we can apply greyscale on the next image at the same time.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/bareMetal/hybrid_parallel.png' style="display: block; margin-left: auto; margin-right: auto; width:60%">
    <figcaption>Hybrid parallel implementation. We combine data and function parallel techniques to apply different parts of the Sobel algorithm on halves of images.</figcaption>
</figure>