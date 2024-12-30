# Document-Page-Detection-with-OpenCV

This project focuses on detecting the boundary of a document page within an image using OpenCV. The process involves preprocessing the image, detecting edges, extracting contours, and then performing perspective transformation to achieve a clean and well-aligned document image.

## Overview

This repository uses OpenCV to detect the boundaries of a document page in an image, performing a series of image processing steps:
1. **Edge Detection** using the Canny edge detector.
2. **Image Preprocessing** including scaling, converting to grayscale, thresholding, and morphological operations like closing and erosion.
3. **Contour Detection** to find the largest contour, which corresponds to the document page.
4. **Perspective Transformation** to correct the perspective of the document, making the page appear as if viewed from the front.

## Features
- Detect document boundaries in images.
- Preprocess images using thresholding, erosion, and closing.
- Use perspective transformation to align the document.
- Visualize the document page with matplotlib.

## Technologies Used
- **Python 3.x**
- **OpenCV** for image processing.
- **NumPy** for numerical operations.
- **Matplotlib** for visualizing results.

## Setup

### 1. Clone the Repository
To get started with the project, clone the repository:


### 2. Install Dependencies
Ensure that you have Python 3.x installed on your system.


### 3. Running the Code

Once the dependencies are installed, you can run the image processing script to detect the document boundaries and transform the perspective.

You can run the script in Jupyter Notebook or as a standalone Python script. Below is a step-by-step breakdown of the process:

1. **Image Preprocessing**: The input image is read, and preprocessing steps like converting to grayscale, applying thresholding, and performing morphological operations are applied.
   
2. **Edge Detection**: Using the Canny edge detector, we highlight the edges of the document.

3. **Contour Detection**: We find contours in the image and select the largest contour, assuming it corresponds to the document's boundary.

4. **Perspective Transformation**: Using the largest contour's corner points, we apply a perspective transformation to straighten the document.


### Files in the Repository

- **document_page_detection.py**: Main script that performs the image processing steps (edge detection, contour finding, and perspective transformation).
- **README.md**: This file that provides an overview and setup instructions.

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. If you find any bugs or have any feature requests, please open an issue.

