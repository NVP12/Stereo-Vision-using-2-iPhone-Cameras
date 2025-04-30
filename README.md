Stereo Vision Depth Estimation using Dual iPhone 15 Cameras





📌 Overview

This project implements a stereo vision system using two iPhone 15 cameras to estimate depth from images. By calibrating the cameras and rectifying the image pairs, we generate disparity maps and estimate real-world depth. It’s designed as a low-cost DIY alternative to commercial stereo rigs, useful for robotics, AR, and computer vision education.

📷 Built during my MS in Robotics @ UMN and jointly developed with a teammate.⚙️ Tools used: OpenCV, Python, NumPy, and MATLAB (for calibration validation).

🚀 Features

Dual iPhone 15 camera setup for stereo image capture

OpenCV-based stereo camera calibration

Image rectification and epipolar alignment

Disparity map generation using block matching algorithms

Depth map computation and visualization

Optional K-means post-processing for refinement

🛠️ Project Structure

Stereo-Vision-using-2-iPhone-Cameras/
│
├── calibration/               # Camera calibration scripts and images
├── stereo_capture/           # Code to sync and align stereo images
├── disparity_map/            # Disparity and depth estimation logic
├── results/                  # Sample outputs and visualizations
├── utils/                    # Helper functions (e.g., undistort, resize)
├── README.md                 # You’re reading it!
└── requirements.txt          # Python dependencies

🧠 Methodology

Camera CalibrationUsed chessboard patterns to calibrate both cameras using OpenCV’s cv2.calibrateCamera() and saved intrinsic/extrinsic parameters.

Stereo RectificationAligned both camera images to make corresponding points lie on the same horizontal line.

Disparity CalculationApplied block matching using StereoBM and StereoSGBM to compute disparity maps.

Depth EstimationTranslated disparity to depth using the formula:



where f is focal length and B is baseline distance.

Post-processingUsed K-means clustering for enhancing segmentation of depth layers.

🧪 Sample Results

Left Image

Right Image

Disparity Map

Depth Visualization

📸

📸

🌈

🔍

Full examples in /results/.

🖥️ Requirements

Install dependencies:

pip install -r requirements.txt

Recommended:

Python 3.8+

OpenCV ≥ 4.5

NumPy, Matplotlib

🤝 Collaboration

This project was jointly developed by:

Nitish Poojari – Robotics @ UMN

Teammate Name – [Institution Name]

🧭 Future Work

Integrate point cloud generation using Open3D

Real-time stereo matching with mobile streaming

Comparison with LiDAR-based depth for benchmarking

📜 License

This project is licensed under the MIT License.

📫 Contact

Feel free to reach out:

📧 nitishpoojari10@gmail.com

🌐 LinkedIn

