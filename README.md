# 🐱🐶 Cat vs Dog Classification using Transfer Learning

This project leverages **Transfer Learning** with a pre-trained **ResNet50** model to classify images of cats and dogs. It was developed as part of the [Dogs vs. Cats Redux: Kernels Edition](https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/overview) Kaggle competition.

---

## 📚 Project Overview

- **Objective**: Build a binary image classifier to distinguish between cats and dogs.
- **Approach**:
  - Utilize a pre-trained **ResNet50** model (excluding top layers) for feature extraction.
  - Add custom classification layers tailored for the binary classification task.
  - Implement data augmentation to enhance model generalization.
  - Apply early stopping and learning rate reduction callbacks during training.

---

## 🛠️ Tech Stack

- **Python**
- **TensorFlow** / **Keras**
- **NumPy**
- **Matplotlib**
- **Pandas**

---

## 📊 Model Architecture

- **Base Model**: ResNet50 (pre-trained on ImageNet, `include_top=False`)
- **Custom Layers**:
  - Global Average Pooling
  - Dense layer with ReLU activation
  - Output layer with sigmoid activation for binary classification

- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Evaluation Metric**: Accuracy

---

## 🎯 Results

- Achieved high accuracy on both training and validation datasets.
- The model demonstrates strong generalization capabilities, attributed to transfer learning and data augmentation techniques.
