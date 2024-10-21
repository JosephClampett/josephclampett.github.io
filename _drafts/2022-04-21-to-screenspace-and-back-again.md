---
title: 'To Screenspace and Back Again - Projections and Unprojections'
date: 2022-04-21
permalink: /posts/2022/04/21/to-screenspace-and-back-again/
tags:
  - programming
  - graphics
---
{% include katex_import.html %}

Plane Intersection
======
We will start with the easiest two coordinates to calculate, $$\hat{\textbf{q}}_x$$ and $$\hat{\textbf{q}}_y$$. It's easiest to work on one and use the similarities to calculate the other, so we will look at an $$xz$$ trace of the frustum.
----
----
We can fix our plane anywhere, so it's easiest to choose the bounds of the plane
$$\frac{a_x}{g} = \tan(\varphi_x)$$

$$\frac{a_y}{g} = \tan(\varphi_y)$$

$$\frac{\sqrt{a_y^2+a_x^2}}{g} = \tan(\varphi_d)$$

Thus we can choose to define $$g$$ in terms of one angle. Here we choose to follow photography convention and obtain $$g$$ from the *diagonal Field of View (FoV)*, $$\theta_d$$ (which will often be called the *angle of view* on lens specifications), but we can also calculate it from the vertical FoV, $$\theta_y$$, or the horizontal FoV, $$\theta_x$$.

$$g = \frac{\sqrt{a_y^2+a_x^2}}{\tan(\varphi_d)},\:\varphi_d = \frac{\theta_d}{2}$$

$$g = \frac{a_y}{\tan(\varphi_y)},\:\varphi_y = \frac{\theta_y}{2}$$

$$g = \frac{a_x}{\tan(\varphi_x)},\:\varphi_x = \frac{\theta_y}{2}$$

----
----
For this graph, we can calculate the intersection of the line with our $$z = g$$ value. Thus, we obtain
$$g = \frac{\hat{\textbf{p}}_z - 0}{\hat{\textbf{p}}_y - 0}y = \frac{\hat{\textbf{p}}_z}{\hat{\textbf{p}}_y}y$$

$$x = \frac{\hat{\textbf{p}}_x}{\hat{\textbf{p}}_z}g$$

$$y = \frac{\hat{\textbf{p}}_y}{\hat{\textbf{p}}_z}g$$