# Liver Tumor Segmentation and Detection using ResUNET

This repository contains the implementation of the **Liver Tumor Segmentation and Detection** model using the **ResUNET** architecture. The goal of this project is to develop a deep learning model that can accurately segment liver tumors from medical images, aiding in diagnosis and treatment planning.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Architecture](#architecture)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Liver cancer is among the most fatal cancers globally, and early detection is vital for improving patient outcomes. This project utilizes the ResUNET architecture to perform segmentation of liver tumors from CT scan images, providing essential tools for clinicians in the early diagnosis of liver cancer.

## Features

- **ResUNET Architecture:** A hybrid model combining ResNet's deep feature extraction capabilities with UNET's effective segmentation.
- **Data Augmentation:** Implements various augmentation techniques to enhance the model's generalization.
- **Comprehensive Evaluation Metrics:** Includes Dice Coefficient, IoU, Precision, and Recall to evaluate model performance.

## Architecture

The ResUNET architecture combines the strengths of residual learning (ResNet) and the UNET model, specifically designed for image segmentation tasks. This combination helps in retaining spatial information through skip connections while ensuring deep feature extraction.

### Key Components:

- **Encoder:** Based on ResNet, it extracts hierarchical features from the input images.
- **Decoder:** Reconstructs the image to the original size, outputting the segmentation mask.
- **Skip Connections:** Maintain high-resolution spatial features by connecting the encoder and decoder at each level.

## Dataset
)
The model is trained on the [Liver Tumor Segmentation Challenge (LiTS)](https://competitions.codalab.org/competitions/17094 dataset, which includes annotated CT scans with labeled liver tumors.

### Preprocessing Steps:

- **Normalization:** Standardizes pixel values across images.
- **Resizing:** Ensures a consistent input size for the network.
- **Augmentation:** Applies transformations like rotation, flipping, and scaling to improve model robustness.

## Installation

Follow these steps to set up the project:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Liver-Tumor-Segmentation-Detection-by-ResUNET.git
   cd Liver-Tumor-Segmentation-Detection-by-ResUNET
