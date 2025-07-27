# ComputerVision_HistologyAnalysis

This project performs an analysis of histological images using computer vision techniques in Python. The primary goal is to detect and characterize lumen structures in tissue samples, helping differentiate between healthy and cancerous tissue morphology.

## Overview

Two histological images are processed and compared:
- histo_1.jpg — expected to represent healthy tissue
- histo_2.jpg — expected to represent cancerous tissue

The process involves:
- Converting images to CMYK color space
- Extracting the magenta channel (which highlights tissue regions)
- Applying Gaussian blur and Otsu thresholding
- Cleaning small regions and segmenting lumens
- Filling holes and detecting contours
- Cropping the largest lumen
- Extracting 13 geometric features per image

## Technologies Used
- Python
- OpenCV
- scikit-image
- SciPy
- Matplotlib
