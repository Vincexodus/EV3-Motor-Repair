---
title: "EV3 Classroom Add-Ons"
date: 2023-04-12
layout: post
---

Attempt to replicate blocks from EV3 Lab Software that are unavailable in EV3 Classroom

## Unavailable/Unsupported blocks
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/sensor(yellow).png %}" height="400">

<img src="{{ site.base_url }}{% link /assets/classroom-imgs/advanced(blue).png %}" height="400">

These blocks do not exist in lab software, can't replicate them either.

## Replicated blocks (results not completely identical)
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/classroom_draw.png %}" width="400">

Write block is used to draw shapes on screen, symbols like `.`, `a` produces weird/inconsistent results. Unicode characters mostly results in small `...` dots on screen. Current viable characters that works: `+`, `0`.

### Display Shape: Line (Diagonal)
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/shape_line.png %}" width="250">

<img src="{{ site.base_url }}{% link /assets/classroom-imgs/diagonal_classroom.png %}" height="500">

### Display Shape: Line (Vertical & Horizontal)
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/shape_line.png %}" width="250">

<img src="{{ site.base_url }}{% link /assets/classroom-imgs/vertical_horizontal_classroom.png %}" height="500">

### Display Shape: Rectangle
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/shape_rectangle.png %}" width="250">

<img src="{{ site.base_url }}{% link /assets/classroom-imgs/rectangle_classroom.png %}" width="500">
<br>To fill drawn rectangle, set `fill` to 1.

### Display Shape: Circle 
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/shape_circle.png %}" width="250">

<img src="{{ site.base_url }}{% link /assets/classroom-imgs/circle_classroom.png %}" height="500">
<br>To empty fill of drawn circle, simply change condition of radius `distance<= radius` to `distance <= radius_max || distance >= radius_min` as thickness of stroke.

### Touch Sensor: Bumped
<img src="{{ site.base_url }}{% link /assets/classroom-imgs/touchSensor_bump.png %}" height="200">

<img src="{{ site.base_url }}{% link /assets/classroom-imgs/touch_classroom.png %}" width="500">
<br>Works both in `if` statement or two `wait until` statement.

<br>`Shape.lmsp` consist of replicated shape blocks mentioned above.
<br>`Sketch.lmsp` enables sketching on screen by controlling brick buttons.
<br><br>Download the program files [here](https://github.com/Vincexodus/EV3-Tools-and-Guides/tree/main/src)

