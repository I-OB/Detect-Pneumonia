# Pneumonia detecion in chest X-Ray images using Convolutional Neural Networks

## Overview
This repository houses the code and documentation for a deep learning model designed to address the challenge of multiclass X-ray classification for pneumonia detection. The project focused on exploring various models and architectures to achieve accurate and robust classification results. The development of this model was part of a Kaggle competition within our university class. The competition aimed to foster collaboration and innovation among students, providing an opportunity to apply deep learning techniques to real-world healthcare challenges.
To learn more about the Kaggle competition, visit the [competition webpage.](https://www.kaggle.com/competitions/detect-pneumonia-spring-2023)

### Keywords
CNN, Transfer learning, Ensemble methods, Pneumonia, Classification

## Table of Contents
1. [Dataset](#Dataset)
2. [Models explored](#Models-explored)
3. [Challenges and Solutions Explored](#Challenges-and-Solutions-Explored)
4. [Conclusion](#Conclusion)

## 1. Dataset <a name="Dataset"></a>
The dataset used for training and evaluation presented a slight class imbalance, with 1227 normal cases (class 0), 2239 bacterial pneumonia cases (class 1), and 1207 viral pneumonia cases (class 2). Various techniques were employed to address the imbalance.

## 2. Models Explored <a name="Models-explored"></a>
The project involved experimentation with a variety of models, with a particular emphasis on VGG19 and ResNet50. The notebook showcases these models, but extensive exploration beyond those presented here was conducted in the quest for optimal performance.

## 3. Challenges and Solutions Explored <a name="Challenges-and-Solutions-Explored"></a>
### 3.1 Data Imbalance
Equalizing the number of images for each class did not improve accuracy due to the subtle differences between bacterial and viral pneumonia.

### 3.2 Data Augmentation
Class-specific augmentations and combinations across classes were explored but did not significantly improve classification.

### 3.3 Ensemble Methods
Ensemble methods like majority voting, averaging, and maximum voting were employed using different VGG19 architectures. Positive outcomes were observed.

### 3.4 Stacked Ensemble Model
Combining multiple architectures into a stacked ensemble did not surpass the performance of individual models.

### 3.5 Feature Extraction
Random forest feature extraction using pre-trained VGG19 features did not achieve satisfactory results.

### 3.6 Cross-Validation
Implementing k-fold cross-validation did not significantly improve performance in distinguishing between bacterial and viral pneumonia.

## 4. Conclusion <a name="Conclusion"></a>
Distinguishing between bacterial and viral pneumonia proved challenging due to their similarities. While VGG19 served as a beneficial starting point, further exploration is needed to enhance accuracy and robustness. The project signals the necessity for ongoing research and development in this domain.

