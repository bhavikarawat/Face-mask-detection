# AI-Based Face Mask Detection

## 📌 Project Overview

This project implements an AI-based face mask detection system using TensorFlow, OpenCV, and TFLite. The system is trained on images of people wearing and not wearing masks and can be deployed for real-time detection using a laptop webcam.  

## 📂 Project Structure  
│── maskData/ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; # Dataset (With Mask & Without Mask)  
│── README.md &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;            # Project documentation   
│── app.py &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;                        # VS Code real-time mask detection script 
│── mask_detection.ipynb &nbsp;&nbsp;&nbsp;&nbsp;            # Google Colab training notebook   
│── mask_detection.tflite&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;       # Saved TFLite model   

## 📥 Dataset
The dataset consists of two categories:  
1-With Mask (label: 1)  
2-Without Mask (label: 0)

## 🏗️ Model Training

The model is trained using TensorFlow and Google Colab. It consists of multiple convolutional layers for feature extraction and classification. The model is later converted into a TensorFlow Lite (TFLite) model for real-time deployment.  \
🔹 Steps to Train the Model:  
1-Run the mask_detection_training.ipynb notebook in Google Colab.  
2-The model is trained with data augmentation, batch normalization, and dropout.  
3-The trained model is converted to a TFLite model for edge deployment.  
4-Download the mask_detection.tflite model.  

## 🖥️ Technology Stack  
Google Colab (Training)  
TensorFlow & TFLite (Model Development)  
OpenCV (Webcam Processing)  
NumPy, Matplotlib, Seaborn (Data Processing & Visualization)  
Python (Programming Language)

## 📊 Model Performance

Training Accuracy: ~96%

Validation Accuracy: ~96%

Test Accuracy: ~96.5%

## ⚠️ Known Issues

Detection accuracy may drop under low-light conditions.

Works best for frontal face images.

## 🚀 Future Enhancements

Improve generalizability by using more data augmentation techniques or transfer learning.

Enhance face detection to work in dynamic environments.



