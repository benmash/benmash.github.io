---
title: "Numpy Path Tracer"
categories:
    - projects
---

I've started working on a pathtracer written in Python with NumPy. My machine learning class this semester expects good Python experience so I decided to start a project involving linear algebra to give me some practice. It's a pretty interesting to me since I've done a few things with pathtracers in the past, but since they were computed on the GPU using shaders my code only had to compute the color of one pixel at a time. Using NumPy, I'm manipulating the entire matrix of pixels and their corresponding rays at the same time, which is more or less the opposite approach. It's definitely less efficient, given GPUs are literally built to do this sort of thing, but this approach does allow for some techniques that don't work as well in parallel. Code is [here](https://github.com/benmash/numpy-pathtracer).

  
    
![Depth Image](/assets/images/purple.png)
*Example Image of some spheres*