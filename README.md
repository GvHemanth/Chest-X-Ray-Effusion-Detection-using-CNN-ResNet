# X-Ray Image Classification Project

This project aims to build a deep learning model for classifying chest X-ray images into "normal" and "abnormal" classes. The model is trained to detect abnormalities in X-ray images, making it a valuable tool for medical professionals and researchers.

## Table of Contents
- Introduction
- Dataset
- Data Pre-processing
- Data Augmentation
- Model Building
- Weighted Cross-Entropy
- Training
- Evaluation
- Making Predictions


## Installation
To run this project locally, you need the following prerequisites:
- Python 3
- TensorFlow
- Scikit-learn
- Matplotlib
- OpenCV
- Numpy

You can install the required packages using the following command:
```bash
pip install tensorflow scikit-learn matplotlib opencv-python numpy
```

## Dataset
The dataset consists of grayscale chest X-ray images with two classes: "nofindings" and "effusion." We performed data augmentation to enrich the dataset and address class imbalance issues.

## Model Building
We used a ResNet-18 architecture for the image classification task. The model was trained using weighted cross-entropy to handle class imbalance effectively.

## Training
The model was trained on augmented data for a certain number of epochs. We monitored the AUC metric to evaluate model performance.

## Evaluation
The final model achieved satisfactory results on the validation set with improved AUC values, indicating its effectiveness in identifying abnormalities.

## Making Predictions
We provided a method to make predictions using the trained model on new chest X-ray images.

## Conclusion
This project demonstrates the application of deep learning in medical image classification, specifically for chest X-ray images. The weighted cross-entropy technique proved crucial in handling imbalanced data and improving model accuracy in identifying abnormalities.
