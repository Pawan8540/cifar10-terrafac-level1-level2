# cifar10-terrafac-level1-level2
CIFAR-10 image classification – Level 1 &amp; Level 2 submission
CIFAR-10 Image Classification (Level 1 & Level 2)
 Problem Understanding

The objective of this project is to perform image classification on the CIFAR-10 dataset, which consists of 60,000 RGB images (32×32) across 10 object categories such as airplanes, cars, animals, and everyday objects.

The challenge is to:

Build a baseline deep learning model using transfer learning.

Apply systematic improvements such as data augmentation and regularization.

Analyze performance across multiple levels in a structured manner.

This project follows a level-wise experimental approach to demonstrate understanding of deep learning workflows rather than only maximizing accuracy.

📦 Dataset Details

Dataset: CIFAR-10

Number of classes: 10

Image size: 32×32 RGB

Total images: 60,000

 Data Split Strategy

80% Training

10% Validation

10% Test

The official CIFAR-10 test set is used for final evaluation.
Validation data is carved out from the training set to ensure a fair comparison across levels.

 Approach Overview

The project is implemented in two levels:

Level 1 — Baseline Model

Used ResNet-18 pretrained on ImageNet

Replaced the final classification layer to match 10 CIFAR-10 classes

No data augmentation or regularization applied

Purpose: establish a reference performance baseline

 Level 2 — Improved Model

Introduced data augmentation (random cropping and horizontal flipping)

Added regularization using weight decay

Kept architecture and dataset split unchanged for fair comparison

Purpose: improve robustness and reduce overfitting

 Experimental Setup

Framework: PyTorch

Platform: Google Colab (GPU enabled)

Optimizer: Adam

Loss Function: Cross-Entropy Loss

Learning Rate: 1e-4

Epochs: 20–25

All experiments were executed on Colab with visible outputs to ensure reproducibility
