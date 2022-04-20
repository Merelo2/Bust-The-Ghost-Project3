# Bust the Ghost - CSC 4301 - Spring 2022 - Dr. Tajjedine Rachidi

## Introduction

In this project, Mohamed Amine Eloudghiri and I will be implementing a simple bust the ghost game using Unity and Probabilistic Programming. The game will be played in the Unity editor. It consists of an 8x20 grid of blocks that can be clicked to attempt to bust the ghost. The ghost is set randomly within the grid. The player will have to click on blocks to attempt to find the ghost. The game ends if the user does not find the ghost.

## Color Code
 - **Red**: The ghost.
 - **Orange**: 1 or 2 cells away from the ghost.
 - **Yellow**: 3 or 4 cells away from the ghost.
 - **Green**: 5 or 6 cells away from the ghost.
## Demo Video

[![](https://img.youtube.com/vi/Gumdupj4l30/0.jpg)](https://www.youtube.com/watch?v=Gumdupj4l30)

## Probabilistic Programming

The Posterior Probability of the Ghost `P(Ghost / Color)` is updated and presented on the cells using Bayesian inference after each click "t."
The used bayesian formula to update each block is the following:

#### `P(Ghost_t)=P(Ghost/Color_t)=P(Ghost_t-1)*P(Color/Distance from Ghost)`

