---
permalink: /camera
layout: page
title: Camera
usemathjax: true
---

In contrast to our previous work, we used only the simple robots head-mounted RGB camera to collect the measurements.
The nominal intrinsic paramterers of the camera are:

| Name              | Symbol                 | Values     | Unit   |
| ----------------- | ---------------------- | ---------- |------- |
| Resolution        |   /                    | (640, 480) | Pixel  |
| Frustum           |   /                    | (57, 43)   | Degree |
| ----------------- |                        | ---------- | ------ |
| Focal Length      | \\( f_\mathrm{C} \\)   | 523.1053    Pixel  |
| Camera Center     | \\( c_\mathrm{C} \\)   | (323.9319, 244.0806) | Pixel  |
| Radial Distortion | \\( \xi_\mathrm{C} \\) | 0.023217     |\begin{align} 
{}^{\mathrm{c}}T_0 =  
\begin{bmatrix}
0 & -1 & 0 & -2.5 \\\ 
1 & 0  & 0 & 2.0 \\\ 
0 & 0  & 1 & 0.1 \\\ 
0 & 0  & 0 & 1
\end{bmatrix}        |  

The calibrateted parameters are: 

Note that the camera is mounted vertical in the robots head.
