# OpenCV Project - Image Contour Detection

## Overview
This project applies image processing techniques to detect and draw contours in images using the OpenCV library. It features the ability to distinguish between external and internal contours and draw them in different colors.

## Features
- Read and display images
- Convert images to grayscale
- Reduce noise using Gaussian Blur
- Detect edges using Canny edge detection algorithm
- Convert images to binary using Thresholding
- Detect contours using findContours with RETR_TREE mode
- Distinguish external contours (green) from internal contours (blue)
- Display results in a grid of 6 subplots
- Print statistics about detected contours
- Save the resulting image

## Requirements
- OpenCV
- NumPy
- Matplotlib

## Installation
pip install opencv-python numpy matplotlib

## How to Run
- Make sure the image file input1.jpg is in the same directory
- Run the code
- A window will display 6 images: original image, grayscale, binary image, contours, external contours only, internal contours only
- Statistics about contour counts will be printed
- The final image will be saved as output_all_contours.jpg

## Example Output
Number of detected contours: 64
Number of external contours: 15
Number of internal contours: 49

## Code Explanation
- Read image and convert from BGR to RGB
- Convert image to grayscale
- Apply Gaussian Blur to reduce noise
- Apply Thresholding using Otsu to get binary image
- Detect contours using RETR_TREE
- Draw external contours in green and internal contours in blue
- Display all results in an image grid
- Save the final image
