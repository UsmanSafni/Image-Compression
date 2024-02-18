# Image Compression using K-means Algorithm

## Introduction

This project focuses on image compression using the K-means algorithm. The primary goal is to reduce the number of colors in a given image, efficiently representing it in a compressed form. The significance lies in the ability to maintain image quality while significantly decreasing the required storage space, making it applicable to scenarios with limited storage resources.

## Data Overview

- **Dataset:** The dataset used is an image in a 24-bit color representation, where each pixel is represented by three 8-bit values for red, green, and blue intensities.
- **Size:** The image is 128x128 pixels, resulting in 16384 data points.
- **Preprocessing:** The image is loaded using matplotlib, and preprocessing involves reshaping the matrix to a 2D matrix of pixel colors.

## Problem Definition

The machine learning problem involves applying K-means clustering to find the 16 most representative colors in the image. Success is measured by the ability to reconstruct the image using these 16 colors, achieving a significant reduction in storage requirements while retaining image quality.

## Methodology

- **Algorithm:** The chosen methodology involves applying the K-means algorithm to the pre-processed image data.
- **Hyperparameter Tuning:** Different values of K (number of clusters) and maximum iterations are experimented with.
- **Initialization:** K-means initialization is done using a function that selects initial centroids.
- **Compression:** The final step involves assigning each pixel to its closest centroid, effectively compressing the image.

## Results

The results showcase the selected centroids and the compressed image. Key performance metrics include the reduction in bits required for image representation. Visualizations illustrate the effects of compression, revealing the trade-off between reduced storage and potential compression artifacts.

## Conclusion

In conclusion, the project successfully demonstrates the application of K-means for image compression. The compressed representation significantly reduces storage requirements while maintaining essential image characteristics. The project contributes to the field of image processing and storage optimization. Future improvements could involve exploring advanced clustering algorithms or refining the compression process to mitigate artifacts further.

