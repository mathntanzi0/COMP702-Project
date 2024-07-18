# South Africa Bank Notebook Recognition System

Welcome to the South Africa Bank Notebook Recognition System! This repository contains a Python notebook designed to predict the values of provided banknotes using various image processing and computer vision techniques.

## Overview

Banknote recognition involves capturing and classifying images of paper-based currency. This process is crucial for counterfeit detection, automated cash handling, and improved efficiency in banking operations. Our system aims to accurately classify both old and new South African banknotes in denominations of R10, R20, R50, R100, and R200.

## Requirements

To run the code, follow these steps:

1. **Recommended Environment**: Use [Google Colab](https://colab.research.google.com/).
2. **Files to Download**: Ensure you download both JSON files from this repository and upload them to your Google Colab environment.

Once the files are uploaded, the code should run smoothly.

## How to Use

1. **Open Google Colab**: Go to [Google Colab](https://colab.research.google.com/).
2. **Upload Notebook**: Upload the Python notebook from this repository to your Colab environment.
3. **Upload JSON Files**: Download the JSON files from this repository and upload them to Colab.
4. **Run the Notebook**: Execute the cells in the notebook sequentially.

## Methods and Techniques

### Image Preprocessing

- **Gray-Scale Conversion**: Simplifies image data by reducing it to one channel.
- **Contrast Enhancement (Histogram Equalization)**: Enhances visibility of features.
- **Noise Reduction**: Smooths out imperfections in the images.
- **Image Thresholding**: Converts gray-scale images into binary images.
- **Edge Detection**: Identifies boundaries of objects within an image.

### Feature Extraction

The following features are extracted from the banknote images:

- **Hu Moments**: Capture shape invariants.
- **Edge Features**: Quantify edge density and patterns.
- **Color Moments**: Represent the color distribution in the image.

### Classification Models

Three classification models are implemented and evaluated:

1. **Support Vector Machine (SVM)**: Uses a linear kernel to classify banknotes.
2. **Feed-Forward Neural Network (FNN)**: Utilizes Keras with ReLU activation and dropout layers.
3. **Random Forest Classifier**: Aggregates results of multiple decision trees for stable predictions.

## Dataset

The dataset consists of images of South African banknotes in denominations of R10, R20, R50, R100, and R200. Each denomination includes images of both front and back sides, processed and encoded in JSON format.
