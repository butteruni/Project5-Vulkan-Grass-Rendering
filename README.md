Vulkan Grass Rendering
==================================

**University of Pennsylvania, CIS 565: GPU Programming and Architecture, Project 5**

* MingLi Gu
* Tested on: Windows 11 23H2
  - AMD Ryzen 7 8845HS w 3.80 GHz
  - 32 RAM
  - NVIDIA GeForce RTX 4070 Laptop 8GB

### Introduction

​	This project is a Vulkan implementation of paper [Responsive Real-Time Grass Rendering for General 3D Scenes](https://www.cg.tuwien.ac.at/research/publications/2017/JAHRMANN-2017-RRTG/JAHRMANN-2017-RRTG-draft.pdf). The paper use Bezier curves to present individual grass blades, which is achieved by using compute shader in this project.

![](https://github.com/butteruni/Project5-Vulkan-Grass-Rendering/blob/main/img/example.gif?raw=true)

​	

| Num of Blades | FPS  |
| :------------ | ---- |
| 2^20          | 200  |

### Feature

- vulkan pipeline
- compute shader for physic calculation
- culling optimization

### Culling Optimization

| *Orientation Culling*                                        | *Frustum Culling*                                            | *Distance Culling*                                           |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](https://github.com/butteruni/Project5-Vulkan-Grass-Rendering/blob/main/img/orientation.gif?raw=true) | ![](https://github.com/butteruni/Project5-Vulkan-Grass-Rendering/blob/main/img/frustum.gif?raw=true) | ![](https://github.com/butteruni/Project5-Vulkan-Grass-Rendering/blob/main/img/distance.gif?raw=true) |



### Performance Analysis

![](https://github.com/butteruni/Project5-Vulkan-Grass-Rendering/blob/main/img/performance.png?raw=true)
