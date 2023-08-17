# BYOL

This repository contains implementations of BYOL(Bootstrap Your Own Latent) model.

## Requirements

To run the scripts in this repository, you will need to have the following dependencies installed:

- Python 3
- PyTorch

## Model
BYOL is a self-supervised learning algorithm that does not explicitly use negative samples. Instead, it directly minimizes the similarity of representations of the same image under a different augmented view (positive pair). This makes BYOL more efficient to train than contrastive learning methods, which require a larger batch size to learn from negative samples. BYOL has been shown to achieve state-of-the-art results on a variety of image classification tasks.


<h3 align="center">Fashion MNIST</h3>
<p align="center">
  <img src="images/BYOL.png" width="600">
</p>

## Results

This project aims to evaluate the impact of pretraining the model with BYOL on the STL10 dataset for a classification task. We compare the performance results before and after incorporating BYOL pretraining.

The initial accuracy achieved without pretraining the model was 84.58%. However, after applying BYOL pretraining with 10 epochs, the accuracy significantly improved to 87.61%. This demonstrates the effectiveness of utilizing BYOL in enhancing the model's performance for the classification task.

To implement BYOL pretraining, we utilized a Resnet18 model pretrained on the ImageNet dataset as the encoder model for BYOL. Leveraging the knowledge learned from the ImageNet dataset proved beneficial in further enhancing the model's capabilities during the pretraining phase.

The improved accuracy resulting from the application of BYOL pretraining highlights its potential as a valuable technique for boosting performance in classification tasks.
