# 📈 BYOL (Bootstrap Your Own Latent) – From Scratch Implementation in Pytorch

<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python">
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white" alt="Jupyter Notebook">
</p>
<p align="center">
  
Welcome to the **BYOL (Bootstrap Your Own Latent)** repository! Dive into our comprehensive, from-scratch implementation of BYOL—a cutting-edge self-supervised learning algorithm that's transforming how we approach unsupervised feature learning.

## 🔧 Requirements

Before running the code, ensure you have the following dependencies:

- **Python 3**: The language used for implementation.
- **PyTorch**: The deep learning framework powering our model training and evaluation.

## 🧠 Model Overview

BYOL represents a breakthrough in self-supervised learning. Unlike traditional methods that rely on negative samples for contrastive learning, BYOL focuses solely on positive pairs—images of the same instance with different augmentations. This unique approach simplifies training and minimizes computational requirements, achieving remarkable results.

### Key Features:
- **No Negative Samples Required**: Efficient training by focusing exclusively on positive pairs.
- **State-of-the-Art Results**: Achieves impressive performance on various image classification benchmarks.

<h3 align="center">BYOL Model</h3>
<p align="center">
  <img src="https://raw.githubusercontent.com/deepmancer/byol-pytorch/main/images/Byol.jpg" width="600" alt="BYOL Model Overview">
</p>

## 📁 Dataset

### STL10 Dataset

We use the STL10 dataset to evaluate our BYOL implementation. This dataset is tailored for developing and testing unsupervised feature learning and self-supervised learning models.

- **Overview**: Contains 10 classes, each with 500 training images and 800 test images.
- **Source**: [STL10 Dataset](https://cs.stanford.edu/~acoates/stl10/)

<h3 align="center">STL10 Dataset Example</h3>
<p align="center">
  <img src="https://cs.stanford.edu/~acoates/stl10/images.png" width="600" alt="STL10 Dataset Sample">
</p>

## 📊 Results

Our experiments highlight the impact of BYOL pretraining on the STL10 dataset:

- **Without Pretraining**: Baseline accuracy of 84.58%.
- **With BYOL Pretraining**: Accuracy improved to 87.61% after 10 epochs, demonstrating BYOL’s effectiveness.

### Implementation Insights

This repository features a complete, from-scratch implementation of BYOL. For our experiments, we used a ResNet18 model pretrained on ImageNet as the encoder, showcasing how leveraging pretrained models can further enhance BYOL’s capabilities.
