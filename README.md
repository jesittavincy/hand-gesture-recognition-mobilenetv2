# Hand Gesture Recognition Using MobileNetV2 for Touchless Interaction

## Project Overview

This project presents a deep learning-based hand gesture recognition using MobileNetV2 transfer learning for touchless interaction.

A custom dataset containing 785 images across 20 predefined hand gesture classes was used to train and evaluate the model. The system classifies hand gestures from images and provides a foundation for touchless human-computer interaction applications.

## Objectives

- Develop a hand gesture recognition system using deep learning.
- Apply MobileNetV2 transfer learning for hand gesture classification.
- Build and evaluate a custom dataset containing 20 gesture classes.
- Explore hand gestures as an alternative input method for touchless interaction.

## Dataset

- Total images: **785**
- Number of gesture classes: **20**
- Training images: **638**
- Validation images: **147**
- Image size: **224 × 224 pixels**

The dataset contains images representing 20 predefined hand gestures.

## Methodology

The project follows these major stages:

1. Dataset collection and organization
2. Image preprocessing
3. Data augmentation
4. MobileNetV2 transfer learning
5. Model training
6. Model evaluation
7. Hand gesture classification

## Model Architecture

The model uses **MobileNetV2 pretrained on ImageNet** as the feature extraction backbone.

The MobileNetV2 base is kept frozen, with the following classification layers added:

- Global Average Pooling
- Dense layer with 64 neurons and ReLU activation
- Dropout with a rate of 0.6
- Softmax output layer for 20 gesture classes

## Training Configuration

| Parameter | Value |
|---|---|
| Model | MobileNetV2 |
| Pretrained Weights | ImageNet |
| Input Size | 224 × 224 |
| Optimizer | Adam |
| Learning Rate | 0.0001 |
| Epochs | 12 |
| Batch Size | 16 |
| Output Classes | 20 |

## Results

The trained model achieved the following validation performance:

| Metric | Result |
|---|---:|
| Validation Accuracy | **92.52%** |
| Precision | **95.44%** |
| Recall | **93.88%** |
| F1-Score | **93.35%** |

The MobileNetV2-based approach achieved higher classification accuracy than the basic CNN approach discussed in the project report.

## Technologies Used

- Python
- TensorFlow
- Keras
- MobileNetV2
- OpenCV
- NumPy
- Jupyter Notebook
- Google Colab

## Project Documentation

📄 [View Final Year Project Report](./Hand_Gesture_Recognition_MobileNetV2_Project_Report.pdf.pdf)

The project report contains the detailed methodology, dataset description, model architecture, training process, evaluation results, and conclusions.

## Future Enhancements

- Implement real-time gesture recognition using a camera.
- Expand the dataset with more images and gesture classes.
- Improve robustness under different lighting conditions and backgrounds.
- Integrate recognized gestures with practical touchless applications.

## Project Status

**Completed – Final Year Major Project**
