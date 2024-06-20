# Neural Style Transfer
This repository implements a neural style transfer model that allows you to transfer the artistic style of one image (style image) onto the content of another image (content image).

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Major functions](#major-functions)

## Introduction
This project lets you create artistic blends of your photos by applying the style of one image to another. Imagine your family portrait reimagined as a Van Gogh masterpiece or your landscape photos with a Monet-like impressionistic touch. Get creative and explore the possibilities of AI-powered art!

## Features
1. Content & Style Balance: Maintains content (objects/scene) while applying artistic style.
2. Pre-trained VGG19 Features: Leverages VGG19 for efficient feature extraction.
3. Loss-driven Optimization: Minimizes content & style loss for optimal results.
4. Iterative Refinement: Gradually improves the generated image.

## Requirements
### Software:
- Python 3.x (check version with python --version or python3 --version)
- TensorFlow (tested with version 2.x) - Install with pip install tensorflow
- NumPy - Install with pip install numpy
- Matplotlib (optional, for visualization) - Install with pip install matplotlib
### Hardware:
While not strictly required, a computer with a decent GPU will significantly speed up the style transfer process.

## Usage
1. Install the required libraries:
   ```bash
   !pip install tensorflow numpy PIL.image matplotlib
2. Upload your content and style images. Make sure they are named appropriately (e.g., content_image.jpg and style_image.jpg).
3. Run the provided Jupyter notebook.

## Major functions
Major concepts and functions are used to do the following tasks:
1. Load & Preprocess Images: Reads, decodes, resizes, and normalizes images.
2. Feature Extraction (VGG19): Extracts features from content and style images using a pre-trained VGG19 network.
3. Content Loss Calculation: Measures the difference between content and generated image features.
4. Style Loss Calculation: Analyzes correlations in style image features for replication in the generated image.
5. Total Loss & Optimization: Combines content and style loss, iteratively refining the generated image to minimize the total loss.
6. Saving the Result: Saves the final artistic image.
