# Tiny Object Detection in SAR (Synthetic Aperture Radar)

This project aims to detect tiny objects in Synthetic Aperture Radar (SAR) images using advanced deep learning techniques. SAR images are typically used for applications like remote sensing, environmental monitoring, and surveillance. However, detecting small objects in SAR images is challenging due to noise, speckle, and low resolution.

## Overview

The goal of this repository is to provide an end-to-end solution for tiny object detection in SAR images. The project uses a deep learning-based approach, leveraging convolutional neural networks (CNNs) or transformer-based models, to identify and classify tiny objects in SAR imagery.

## Methodology

This research evaluates the performance of FPG (Feature Pyramid Generators), NAS-FPN (Neural Architecture Search-based FPN), and traditional FPN models across various architectures for SAR object detection. Our hypothesis focuses on improving the fused feature representations from the neck and backbone networks to enhance accuracy, particularly for tiny object detection.

## Dataset & Experimental Summary

Two SAR datasets were used:

- [**HRSID Dataset:**](https://github.com/chaozhong2010/HRSID) Testing showed nearly identical performance across all configurations, with no improvement when using NAS-FPN or FPG.
- [**SSDD-OPEN Dataset:**](https://github.com/TianwenZhang0825/Official-SSDD?tab=readme-ov-file) Custom combinations of FPG with ResNet-50 and ResNet-101 variants outperformed TOOD, achieving higher mAP scores (0.6800 and 0.6704).

![methodolgy_wtout_transparent](https://github.com/user-attachments/assets/78ab535a-94fc-4c9c-881a-44288d110f3a)

### Key Features of this Project:

- **Data Preprocessing:** Techniques for preparing and augmenting SAR images for deep learning models.
- **Model Architecture:** A choice of state-of-the-art object detection models tailored for SAR images.
- **Evaluation Metrics:** Methods for evaluating the performance of the model, including precision, recall, F1 score, and mAP (mean Average Precision).
- **Visualization:** Tools for visualizing detection results on SAR images.

## Key Findings:

- **Initial Evaluation:** TOOD emerged as the superior model for SAR object detection.
- **Custom Backbone and FPN Combinations:** Optimized combinations of backbones and FPN variants showed comparable or better performance, suggesting that further hyperparameter optimization can enhance detection accuracy.

This methodology provides insights into the impact of different architectures on tiny object detection in SAR imagery, offering a path to improved model performance through customized configurations.

## Training Notebook

For detailed training and testing procedures, you can explore the [Training Notebook](https://github.com/SK-Nemo/tiny-object-detection-in-SAR/blob/main/Using%20Mmdetection-3x-On-SARScope.ipynb).
