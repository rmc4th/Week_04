# Week 4 Coding Assignment 
# Name: "PacMan"
___

# Description

## Task Overview
Write javascript code that changes the direction of an animated figure when it reaches the edge of the browser screen.

## Background
Starter code (`starter01.html`) and images (`PacMan1.png`, `PacMan2.png`, `PacMan3.png`, and `PacMan4.png`) were provided.

The four images each represent a "PacMan" figure with the following orientation-mouth states respectively: right-open, right-closed, left-open, left-closed.

The `starter01.html` file was a simple 'html' document with code written between `<script>` tags. The code made a two-dimensional array from the four images ([right-open, right-closed][left-open, left-closed]). The code then was primarily two functions `Run()` and `checkPageBounds()`. 

The function `Run()` controlls the motion of the image. The provided code advanced the image one 'frame' by refreshing the current image with the appropriate subsequent image based on the current image and position within the window. To complete the function a recursive call to the Run() function needs to be added.

The function `checkPageBounds()` signature was provided but not impleented. This function is called by the function `Run()`. The function `checkPageBounds()` takes the current direction (a toggle value of 0 or 1 for R-L, L-R motion, respectively). and the image width as arguments and had to update the value of direction, changing it if the image had reached the edge of the window.

## Exercise
When completed the image moves horizontally back and forth across the window. To achieve this completion of the following two tasks is necessary.
1. Complete the implementation of the function `Run()`. Add a function call using the `setTimeout()` function that recursively calls `Run()`. 
2. Complete the implementation of the function `chekPageBounds()`. 

## Result
The resulting `starter01.html` is contained in this repository.

# Installation
The resulting code was tested on Google Chrome. Once loaded, the animation starts with a mouse click in the window.

# Support
For questions contact rmc4th@yahoo.com

# Roadmap
For the exercise, the image can actually encroach over the boundary if the window size is not an even multiple of the image advancement. This was not a concern for the purpose of the exercise but to address it this code adds a buffer to the screen check equal to the advancement distance. This causes the image to come up a bit short of the edges. A further refinement would be to advance the odd value distance and 'touch the wall' before reversing direction. 

# License Information
This work was done as part of MIT xPRO Professional Certificate in Coding. The code above comes with the following license:

MIT License

Copyright (c) 2020 John Williams

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
