# Classification of Real vs. AI-Generated Images

## Table of Contents

- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Methodology](#methodology)
  - [Dataset Description](#dataset-description)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Data Pre-processing](#data-pre-processing)
  - [Model Building and Training](#model-building-and-training)
- [Results and Evaluation](#results-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)


## Introduction

In today's digital landscape, distinguishing between authentic and artificially generated images is crucial due to the rise of sophisticated digital manipulation techniques. This project aims to develop a robust classification model capable of accurately identifying real and AI-generated images. The ability to differentiate between the two holds significant implications across various domains, including journalism, cybersecurity, and content moderation.

## Problem Statement

The proliferation of fake images presents challenges in maintaining the integrity of visual data. This project seeks to address this issue by developing a powerful classification model that can effectively discern between real and AI-generated images. By leveraging machine learning techniques and comprehensive data analysis, we aim to create a reliable solution for combating misinformation and ensuring the authenticity of visual content.

## Methodology

### Dataset Description

The dataset consists of 120,000 images divided into two classes: "REAL" and "FAKE." The "REAL" images are sourced from the CIFAR-10 dataset, while the "FAKE" images are generated using the stable diffusion model version 1.4. The dataset is further divided into training and testing sets, with detailed subclass information provided.

### Exploratory Data Analysis

Exploratory Data Analysis (EDA) is conducted to understand the characteristics and distributions of the dataset. Analysis includes color distribution, texture analysis, and entropy distribution, providing insights into the visual properties of real and fake images.

### Data Pre-processing

Data pre-processing involves resizing images to a uniform size, normalizing pixel values, and other techniques to prepare the dataset for model training.

### Model Building and Training

Multiple classification models are explored, including Vanilla CNN, MobileNet, ResNet, VGG16, EfficientNet, and Vision Transformer (ViT). Each model's architecture, performance, and complexity are evaluated to identify the most effective solution.

## Results and Evaluation

The performance of each model is evaluated based on metrics such as accuracy, precision, recall, and F1-score. Observations and insights regarding model performance and complexity are provided, highlighting the strengths and limitations of each architecture.

| Model       | Accuracy | Precision | Recall | F1-score | Parameters (in Millions) |
|-------------|----------|-----------|--------|----------|--------------------------|
| Vanilla CNN | 0.911    | 0.964     | 0.851  | 0.904    | 0.37                     |
| MobileNet   | 0.950    | 0.944     | 0.958  | 0.947    | 1.1                      |
| ResNet      | 0.960    | 0.952     | 0.970  | 0.961    | 6.26                     |
| VGG16       | 0.960    | 0.971     | 0.948  | 0.959    | 14.86                    |
| EfficientNet| 0.972    | 0.975     | 0.960  | 0.967    | 24.13                    |
| ViT         | **0.984**    | **0.988**     | **0.980**  | **0.984**    | **86.56**                    |


## Conclusion

Advanced architectures like ViT and EfficientNet demonstrate superior performance in accurately classifying real and fake images compared to traditional models. The trade-off between model performance and complexity emphasizes the importance of selecting the right architecture for specific tasks.

## Future Work

Future work will focus on optimizing models through hyperparameter tuning, expanding the dataset, deploying models in real-world scenarios, and enhancing interpretability. Collaboration with experts from various fields will drive innovation and address emerging challenges in image verification.
