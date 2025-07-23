#  Shade Removal from Images

<p align="center">
  <img width="602" height="467" alt="Screenshot 2025-07-24 at 00 03 58" src="https://github.com/user-attachments/assets/72fd6099-6037-449b-8b2d-099eefbd146c" />
</p>

### 📌 Project Overview

This project focuses on removing unwanted shade artifacts from digital images using classical image processing techniques. The objective is to recover the true appearance of scenes affected by non-uniform illumination, using a combination of low-pass filtering, downsampling, normalization, and image enhancement methods.

### 🎯 Goals


The main objectives of this project are to accurately extract shading patterns from RGB images and normalize them to correct non-uniform illumination artifacts. By estimating and removing the shading component, the project aims to recover the true visual appearance of the scenes. It also includes a comparison between the extracted shade and ground truth images to evaluate the accuracy of the method. The entire shade-removal pipeline is visualized step-by-step, providing clear insight into each processing stage. Finally, the corrected images are stitched together to offer a more comprehensive and seamless visual inspection.


### 🛠️ Methodology

The implemented approach follows a multi-step process:

* Load and organize original and ground-truth (shade-free) images
* Downsample and apply Gaussian filtering to estimate low-frequency shading
* Normalize and divide the shaded images by the estimated shade
* Convert RGB shade estimates to grayscale for simplicity
* Visualize comparisons between extracted and real shades
* Experiment with frequency domain analysis (FFT-based comparison)
* Stitch final corrected images to form a continuous scene
