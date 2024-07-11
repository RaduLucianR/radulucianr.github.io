---
title: "Finite field algebra library"
excerpt: "<img src='/images/portfolio/thumbnails/algebra.png'>"
collection: portfolio
date: 22-October-2020
---
**Project attribution**: Project done in collaboration with Teodor Lungu. <br>
**Source**: (Part of) The project's source code is available [here](https://github.com/TeodorLungu/2WF90-Assignment2) <br>
**Short description**: Python library with fast arithmetic, polynomial and finite field operations.<br>
**Technologies**: Python. <br>
**What I did**: I implemented many of the operations, like: long division, find primitive, fast addition, multiplication, Euclid's algorithm etc.

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/algebra/main.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Main function that iterates over a list of execises (inputs) and applies the indicated function, then checks the result.</figcaption>
</figure>

Python library that offers arithmetic functions:
* Integer arithmetic
  * Addition, Subtraction, Multiplication, Division
  * Fast Multiplication with Karatsuba's technique
  * Greatest Common Divisor with Euclid's Algorithm
* Modular arithmetic
  * Modular Addition, Subtraction, Multiplication, Inversion
* Polynomial arithmetic
  * Polynomial Addition, Subtraction, Multiplication
  * Polynomial Long Division
  * Euclid's algorithm for polynomials
  * Checking and finding irreducible polynomials
* Arithmetic in finite fields
  * Generate final fields
  * Generating Addition and Multiplication tables
  * Final field Addition, Subtraction, Multiplication, Inverse, Division
  * Finding a Primitive 

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/algebra/division.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Division of two integers.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/algebra/primitive.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Finding a polynomial primitive.</figcaption>
</figure>