---
permalink: /camera
layout: page
title: Camera
usemathjax: true
---

In contrast to our previous work, we used only the simple robots head-mounted RGB camera to collect the measurements.
The nominal intrinsic paramterers of the camera are:

The calibrateted parameters are: 

| Name              | Symbol                 |  Unit  | Nominal Values       | Calibrated Values    |
|-------------------|:----------------------:|:------:|:--------------------:|:--------------------:|
| Resolution        |   /                    | Pixel  | (640, 480)           | /                    |
| Frustum           |   /                    | Degree | (57, 43)             | /                    |
| ----------------- |                        | ------ | -------------------- | -------------------- |
| Focal Length      | \\( f_\mathrm{C} \\)   | Pixel  | 523.1053             | 518.1601             |
| Camera Center     | \\( c_\mathrm{C} \\)   | Pixel  | (323.9319, 244.0806) | (323.8356, 249.8531) |
| Radial Distortion | \\( \xi_\mathrm{C} \\) | Pixel  | 0.023217             | 0.001327             |

The transformation from the last frame of the head to the camera is known from a previous calibration by

$$
\begin{align}
\mathrm{old:}\,\,{}^{\mathrm{c}}T_0 =
\begin{bmatrix}
0.021778 &  0.204164 &  0.999554 & 0.135092 \\\
0.017923 & -0.999638 &  0.002003 & 0.000701 \\\
0.999602 &  0.017479 & -0.022136 & 0.174262 \\\
0        &  0           &  0         & 1
\end{bmatrix}
\end{align}
$$

The new calibrated frame is 

$$
\begin{align}
\mathrm{new:}\,\,{}^{\mathrm{c}}T_0 =
\begin{bmatrix}
0.027059 & -0.00143 &  0.999632 &  0.140637 \\\
0.011088 & -0.99993 & -0.001738 & -0.000161 \\\
0.999572 & 0.111314 & -0.027042 &  0.174157 \\\
0        &  0       &  0        & 1
\end{bmatrix}
\end{align}
$$

Note that the camera is mounted vertical in the robots head.
