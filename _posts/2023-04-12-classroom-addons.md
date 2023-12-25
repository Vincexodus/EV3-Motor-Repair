---
title: "EV3 Classroom Add-Ons"
date: 2023-04-12
layout: post
---

Attempt to Replicate blocks from EV3 Lab Software that are unavailable in EV3 Classroom

## Unavailable/Unsupported blocks
<img src="./assets/imgs/sensor(yellow).png" height="400">

<img src="./assets/imgs/advanced(blue).png" height="400">


## Replicated blocks (results not completely identical)
<img src="./assets/imgs/classroom_draw.png" width="400">

Write block is used to draw shapes on screen, symbols like `.`, `a` produces weird/inconsistent results. Unicode characters mostly results in small `...` dots on screen. Current viable characters that works: `+`, `0`.

### Display Shape: Line (Diagonal)
<img src="./assets/imgs/shape_line.png" align="top" width="250">

<img src="./assets/imgs/diagonal_classroom.png" height="500">

### Display Shape: Line (Vertical & Horizontal)
<img src="./assets/imgs/shape_line.png" align="top" width="250">

<img src="./assets/imgs/vertical_horizontal_classroom.png" height="500">

### Display Shape: Rectangle
<img src="./assets/imgs/shape_rectangle.png" align="top" width="250">

<img src="./assets/imgs/rectangle_classroom.png" width="500">
<br>To fill drawn rectangle, set `fill` to 1.

### Display Shape: Circle 
<img src="./assets/imgs/shape_circle.png" align="top" width="250">

<img src="./assets/imgs/circle_classroom.png" height="500">
<br>To empty fill of drawn circle, simply change condition of radius `distance<= radius` to `distance <= radius_max || distance >= radius_min` as thickness of stroke.

### Touch Sensor: Bumped
<img src="./assets/imgs/touchSensor_bump.png" height="200">

<img src="./assets/imgs/touch_classroom.png" align="top" width="500">
<br>Works both in `if` statement or two `wait until` statement.

<br>`Shape.lmsp` consist of replicated shape blocks mentioned above.
<br>`Sketch.lmsp` enables sketching on screen by controlling brick buttons.
<br>Download the program files [here](https://vincexodus.github.io/EV3-Tools-And-Guides/src)

