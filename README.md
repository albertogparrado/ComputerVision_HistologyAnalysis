# ComputerVision_HistologyAnalysis

This project performs an analysis of histological images using computer vision techniques in Python. The primary goal is to detect and characterize lumen structures in tissue samples, helping differentiate between healthy and cancerous tissue morphology.

## Overview

Two histological images are processed and compared:
- histo_1.jpg — expected to represent healthy tissue
![histo_1](https://github.com/user-attachments/assets/ffcabb4b-1bea-46a1-bcef-d711f8f370b5)


- histo_2.jpg — expected to represent cancerous tissue
![histo_2](https://github.com/user-attachments/assets/deaf2443-5df3-4be6-9532-04349e763823)



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
