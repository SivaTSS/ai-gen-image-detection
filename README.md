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

## Conclusion

Advanced architectures like ViT and EfficientNet demonstrate superior performance in accurately classifying real and fake images compared to traditional models. The trade-off between model performance and complexity emphasizes the importance of selecting the right architecture for specific tasks.

## Future Work

Future work will focus on optimizing models through hyperparameter tuning, expanding the dataset, deploying models in real-world scenarios, and enhancing interpretability. Collaboration with experts from various fields will drive innovation and address emerging challenges in image verification.
