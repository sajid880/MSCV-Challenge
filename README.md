# MSCV-Challenge
SNR Computation and Analysis

This project demonstrates the computation of Signal-to-Noise Ratio (SNR) and related image processing tasks using Python. The workflow includes preprocessing, histogram analysis, noise generation, filtering, and analyzing the effect of different filter sizes on SNR.

Table of Contents

Introduction

Requirements

Workflow

How to Use

Tasks Overview

Results and Outputs

Introduction

This repository provides a Python-based implementation for performing various image processing tasks on a sample image. Key operations include:

Converting RGB images to grayscale using different methods.

Adding Gaussian noise to an image.

Computing and visualizing histograms.

Analyzing Signal-to-Noise Ratio (SNR) and Peak Signal-to-Noise Ratio (PSNR).

Applying smoothing filters and studying their impact on SNR.

Requirements

Ensure you have the following Python libraries installed:

numpy

opencv-python

matplotlib

scipy

Install the required libraries using pip:

pip install numpy opencv-python matplotlib scipy

Workflow

The code executes the following steps:

Load and preprocess the image: Resize the input image to 256x256 pixels.

Analyze RGB histograms: Display the histograms for the Red, Green, and Blue channels.

Convert to grayscale: Perform grayscale conversion using two methods and compare results.

Histogram of grayscale image: Compute and display the histogram and range of grayscale values.

Generate Gaussian noise: Create and visualize Gaussian white noise with specified parameters.

Analyze noise statistics: Compute the mean, standard deviation, and histogram of the noise.

Autocorrelation of noise: Compute and visualize the autocorrelation of the noise.

Add noise to the grayscale image: Add the Gaussian noise to the grayscale image and analyze the resulting histogram.

Compute SNR and PSNR: Calculate the SNR and PSNR for the noisy image.

Apply smoothing filter: Apply a 2D Gaussian filter to the noisy image and compute the new SNR.

Study SNR evolution: Analyze the evolution of SNR with varying filter sizes.

How to Use

Clone the repository:

git clone <repository-url>

Place your input image in the same directory as the script and rename it to input_image.jpg.

Run the script:

python script_name.py

Observe the outputs displayed in the terminal and the plots for each task.

Tasks Overview

Task 1: Data Type of Image

Displays the data type of the loaded image.

Task 2: RGB Channel Histograms

Plots the histograms for the Red, Green, and Blue channels.

Task 3: Grayscale Conversion

Converts the image to grayscale using two methods:

Method 1: Average of RGB channels.

Method 2: Weighted sum of RGB channels.
Compares the outputs of both methods.

Task 4: Grayscale Histogram and Range

Displays the histogram of the grayscale image and computes the range of pixel values.

Task 5: Gaussian Noise Generation

Generates Gaussian white noise with specified parameters and visualizes it.

Task 6: Noise Histogram and Statistics

Computes the mean and standard deviation of the noise and plots its histogram.

Task 7: Noise Autocorrelation

Calculates and visualizes the autocorrelation of the noise.

Task 8: Noisy Image

Adds the generated noise to the grayscale image and analyzes the resulting histogram.

Task 9: Compute SNR and PSNR

Calculates the Signal-to-Noise Ratio (SNR) and Peak Signal-to-Noise Ratio (PSNR) for the noisy image.

Task 10: Apply Smoothing Filter

Applies a 2D Gaussian filter to the noisy image and computes the new SNR.

Task 11: SNR Evolution with Filter Size

Analyzes the impact of varying filter sizes on SNR and plots the results.

Results and Outputs

Data Type: Displays the type of the loaded image (e.g., uint8).

Histograms: Visualizes histograms for RGB channels, grayscale image, noise, and noisy image.

Noise Statistics: Outputs mean and standard deviation of the noise.

SNR and PSNR: Displays calculated SNR and PSNR values in both linear and logarithmic (dB) scales.

Filtered Image: Shows the smoothed noisy image and the effect of different filter sizes on SNR.
