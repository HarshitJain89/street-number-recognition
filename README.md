# 🔢 Street Number Recognition using CNN

## Overview
A Convolutional Neural Network (CNN) that reads multi-digit numbers from real-world street-level photographs. Trained and evaluated on the Street View House Numbers (SVHN) dataset, the model achieves **80% accuracy on unseen test data**.

## Problem Statement
Street-level imagery contains house numbers useful for address verification, mapping, and navigation. Can a deep learning model automatically read these numbers from photos taken in varying lighting and angles?

## Approach

| Step | Detail |
|------|--------|
| Dataset | Street View House Numbers (SVHN) |
| Preprocessing | Pixel normalisation (0-1), reshape for channel dimension, one-hot encoding |
| Model Architecture | Convolutional Feedforward Neural Network |
| Layers Used | Dense, Conv2D, Dropout, Flatten, Batch Normalisation |
| Loss Function | Categorical Crossentropy |
| Optimiser | Adam |
| Training | 50 epochs, 20% validation split |

## Key Concepts
- **Convolutional layers** extract spatial features from raw image pixels
- **Batch Normalisation** stabilises and accelerates training
- **Dropout** prevents overfitting by randomly deactivating neurons during training
- **Flatten + Dense** layers perform the final classification

## Results

| Dataset | Accuracy |
|---------|----------|
| Training | ~77% |
| Validation | ~80% |
| **Test Set** | **80.7%** |

## Tech Stack
```
Python | TensorFlow | Keras | NumPy | h5py | Matplotlib
```

## How to Run
1. Clone the repo
2. Install dependencies: `pip install tensorflow numpy h5py matplotlib`
3. Download the SVHN dataset (h5 format) and update the file path in the notebook
4. Open in Jupyter or Google Colab and run all cells

---
*Completed as part of the Post-Graduate Program in AI & Machine Learning - University of Texas at Austin (2021)*
