# 3D Environment Localization via Sensor Fusion

This project implements sensor fusion for 3D environment localization using reverse projection of sensor data. It aims to combine information from multiple sensors (e.g., LiDAR, camera) to create a more accurate and robust understanding of the robot's position and surroundings.

## Description

Traditional robot localization methods often rely on a single sensor, which can be susceptible to limitations or errors in specific environments. For instance, LiDAR sensors struggle in low-light conditions, while cameras can have difficulties with depth perception. Sensor fusion combines data from multiple sensors to overcome these limitations. This project focuses on utilizing LiDAR and camera data for localization.

Reverse projection is a technique used to project data from an image plane (camera) back into 3D space. In this context, it's used to find the corresponding 3D world points for detected features in the camera image, leveraging the LiDAR's depth information. By fusing the LiDAR's precise distance measurements with the camera's rich visual data (textures, edges), we aim to achieve a more accurate and reliable localization estimate.

A good reference for sensor fusion in SLAM (Simultaneous Localization and Mapping) systems is [A Review of Multi-Sensor Fusion SLAM Systems Based on 3D LIDAR](https://www.mdpi.com/2072-4292/12/18/7318). This article discusses various sensor fusion approaches and highlights the benefits of combining LiDAR and camera data for robust environment perception in robots.

## Getting Started

This project requires Python 3 and several libraries for sensor fusion and data processing. Here are the dependencies to install:

```bash
pip install numpy opencv-python
