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
| Radial Distortion | \\( \xi_\mathrm{C} \\) | 0.023217     |     |  

The transformation from the last frame of the head to the camera is known from a previous calibration by
\begin{align} 
{}^{\mathrm{c}}T_0 =  
\begin{bmatrix}
2.17783e-02 &  2.04164e-02 &  9.99554e-01 & 1.35092e-01 \\\ 
1.79227e-02 & -9.99638e-01 &  2.00276e-02 & 7.00945e-04 \\\ 
9.99602e-01 &  1.74785e-02 & -2.21363e-02 & 1.74262e-01 \\\ 
0           &  0           &  0           & 1
\end{bmatrix}   
The calibrateted parameters are: 

Note that the camera is mounted vertical in the robots head.
