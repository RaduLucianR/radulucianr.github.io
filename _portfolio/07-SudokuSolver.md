---
title: "Sudoku solver"
excerpt: "Java brute force solver<br/><img src='/images/portfolio/thumbnails/sudoku.png'>"
collection: portfolio
date: 17-January-2021
---
Project done in collaboration with Vlad Pintilie and Teodor Lungu.

Brute force Sudoku solver written in Java. The app can load and solve Sudoku problems. If the current position is easy enough, it can also apply reasoning to find the next move. Moreover, the app has an undo function so one can see the solution backwards. Not all Sudoku puzzles are solvable by this app.

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/sudoku/default.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Default view of the Java Swing app. The left panel contains the display of the Sudoku puzzle. The right panel serves as a log. The top bar serves usual functions for reading a Sudoku starting position from a file, dumping the Sudoku board to a file, clearing the Sudoku board, and solving the puzzle.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/sudoku/reasoning.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Sequence of applying reasoning by pressing Ctrl+R for an easy Sudoku puzzle. Note the log information on the right panel.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/sudoku/whilesolving.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>After selecting the "Solving" function, the algorithm will try and solve the puzzle. During the solving the user can see in real-time the numbers tried by the algorithm on the left panel. Note the log information on the right panel: the mode has been set to SOLVE.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/sudoku/solved.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>When the puzzle is solved it will appear with green numbers.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/sudoku/undo.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>The user can press Ctrl+Z to undo the last move. This is a sequence of pressing undo after a puzzle was solved by the algorithm. During a move/step multiple numbers can be deduced; these numbers are highlighted with light blue. Note the log information on the right panel.</figcaption>
</figure>