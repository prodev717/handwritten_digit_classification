# Handwritten Digit Classification using CNN

A deep learning project that classifies handwritten digits (0–9) using a Convolutional Neural Network (CNN) trained on the MNIST dataset. This project demonstrates the power of CNNs in solving image classification problems and forms a foundation for Optical Character Recognition (OCR) systems.

## Project Overview

This project aims to build a high-accuracy digit recognizer that can identify handwritten numbers regardless of variations in writing style. It applies Convolutional Neural Networks for feature extraction and classification.

## Author

* Ganesh M 
* April 5, 2025

---

## Dataset

* **Source**: MNIST Dataset (CSV Format)
* **Samples**: 70,000 grayscale images (28x28 pixels)

  * Training: 56,000
  * Testing: 14,000
* **Classes**: 10 (Digits 0 through 9)

Each image is a 784-dimensional flattened vector with an associated label.

---

## Model Architecture

The CNN model consists of the following layers:

1. **Conv2D** (32 filters, 3×3) → ReLU
2. **MaxPooling2D** (2×2)
3. **Conv2D** (64 filters, 3×3) → ReLU
4. **MaxPooling2D** (2×2)
5. **Flatten**
6. **Dense** (128 units) → ReLU
7. **Output Dense** (10 units - Softmax)

---

## Training Details

* **Optimizer**: Adam
* **Loss Function**: Categorical Crossentropy
* **Metrics**: Accuracy
* **Epochs**: 5 (adjustable)
* **Batch Size**: 64 (adjustable)

---

## Evaluation

The model was evaluated on various metrics:

* **Accuracy**: \~99.7%
* **Loss**: Monitored during training to ensure convergence
* **Confusion Matrix**: Used for understanding class-wise performance

---

## Visualizations

* Training & Validation Loss vs. Epoch
* Training & Validation Accuracy vs. Epoch
* Confusion Matrix (Test Set)
* Sample Predictions (Correct & Incorrect)

