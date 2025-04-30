# Stereo-Vision-using-2-iPhone-Cameras

# Stereo Vision Depth Estimation using Dual iPhone 15 Cameras

![Depth Estimation](https://img.shields.io/badge/Computer%20Vision-Stereo%20Vision-blue)
![Platform](https://img.shields.io/badge/Platform-iOS%20%26%20Python-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Overview

This project implements a **stereo vision system** using two iPhone 15 cameras to estimate depth from images. By calibrating the cameras and rectifying the image pairs, we generate disparity maps and estimate real-world depth. It’s designed as a low-cost DIY alternative to commercial stereo rigs, useful for robotics, AR, and computer vision education.

> 📷 Built during my MS in Robotics @ UMN and jointly developed with a teammate.  
> ⚙️ Tools used: OpenCV, Python, NumPy, and MATLAB (for calibration validation).

---

## 🚀 Features

- Dual iPhone 15 camera setup for stereo image capture
- OpenCV-based stereo camera calibration
- Image rectification and epipolar alignment
- Disparity map generation using block matching algorithms
- Depth map computation and visualization
- Optional K-means post-processing for refinement

---

## 🛠️ Project Structure

