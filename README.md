# Hand Sign Classification using ResNet50

This project implements a Deep Residual Network (ResNet50) from scratch to classify images of hand signs representing digits 0 through 5. The goal was to build a robust computer vision pipeline that handles data loading, preprocessing, model training, and inference.

## Project Overview

- **Model:** Custom implementation of ResNet50 (50-layer Residual Network) using TensorFlow/Keras.
    
- **Input:** 64x64 RGB images of hand gestures.
    
- **Output:** Classification of the image into one of 6 classes (digits 0-5).
    
- **Key Techniques:** skip-connections to solve vanishing gradient problems.
    

## Dataset

The dataset used for this project is the **Hand Sign Language Digit Dataset**, sourced from Kaggle. It consists of folders labeled 0-5, containing images of hand signs for the respective numbers.

- **Source:** [Kaggle - Hand Sign Language Digit Dataset](https://www.kaggle.com/datasets/shivam1711/hand-sign-language-digit-dataset-for-0-5/data?select=0)


## Results

The model was trained using an Adam optimizer with a learning rate of 0.00015.

- **Training Accuracy:** ~98%
    
- **Validation Accuracy:** ~86%
    
![Accuracy And Loss Graph](Accuaracy_losss_ graph.png)

The model was able to correctly classify a custom image of my hand as the digit 5
The implementation of residual blocks allowed the network to converge effectively despite its depth, avoiding the degradation problem common in deep neural networks.
