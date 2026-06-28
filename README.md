## Leukocyte Classification using AlexNet Transfer Learning

## Project Overview

This project implements a deep learning-based leukocyte (white blood cell) classification system using **AlexNet with Transfer Learning**. The objective is to classify microscopic blood cell images into three different leukocyte classes: **LYT (Lymphocytes), MON (Monocytes), and NGS (Neutrophils)**. Instead of training the network from scratch, a pretrained AlexNet model trained on the ImageNet dataset was fine-tuned on the leukocyte dataset to improve classification performance and reduce training time.

## My Contribution

My primary responsibility was the implementation of the **AlexNet transfer learning pipeline** using PyTorch. This included:

* Loading and preprocessing the leukocyte dataset.
* Applying data augmentation and image normalization.
* Loading a pretrained AlexNet model with ImageNet weights.
* Replacing the original classifier with a custom 3-class output layer.
* Freezing the feature extraction layers and training the classifier.
* Fine-tuning the final convolutional layers for improved performance.
* Evaluating the model using accuracy, confusion matrix, precision, recall, and F1-score.
* Visualizing training/validation accuracy and loss curves.

## Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab (GPU)

## Dataset

The dataset consists of resized microscopic images of three leukocyte classes:

* LYT (Lymphocytes)
* MON (Monocytes)
* NGS (Neutrophils)

## Results

The pretrained AlexNet model successfully learned discriminative features from leukocyte images using transfer learning and fine-tuning, achieving strong classification performance while significantly reducing training time compared to training a model from scratch.
