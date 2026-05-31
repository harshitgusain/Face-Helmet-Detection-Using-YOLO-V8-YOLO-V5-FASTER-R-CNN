# Face & Helmet Detection using YOLOv8, YOLOv5 and Faster R-CNN

## Overview

This project implements a Computer Vision based Helmet Detection System using three state-of-the-art object detection models:

* YOLOv8
* YOLOv5
* Faster R-CNN

The system detects whether a person is wearing a helmet or not from images and compares the performance of different deep learning models based on accuracy, precision, recall, and mAP scores.

The project aims to identify the most suitable model for real-time helmet detection applications such as traffic monitoring, workplace safety, and industrial compliance.

---

## Objectives

* Detect helmets in images using deep learning.
* Compare YOLOv8, YOLOv5, and Faster R-CNN.
* Evaluate model performance using standard object detection metrics.
* Analyze strengths and limitations of each approach.
* Demonstrate why YOLO-based models are preferred for real-time detection.

---

## Dataset

Dataset used:

**Helmet Detection Dataset**
(Kaggle Dataset by Andrew MVD)
https://www.kaggle.com/datasets/andrewmvd/helmet-detection

The dataset contains:

* Images containing riders with helmets and without helmets.
* XML annotation files.
* Bounding box coordinates for object localization.

### Classes

1. With Helmet
2. Without Helmet

---

## Technologies Used

### Programming Language

* Python

### Deep Learning Frameworks

* PyTorch
* Ultralytics YOLO

### Libraries

* OpenCV
* NumPy
* Pandas
* Matplotlib
* Pillow
* TorchVision

### Development Environment

* Google Colab
* Kaggle Dataset API

---

## Project Workflow

### 1. Dataset Preparation

* Download dataset from Kaggle.
* Extract images and XML annotations.
* Convert annotations into model-compatible format.

### 2. YOLOv8 Training

* Train YOLOv8 on the helmet detection dataset.
* Evaluate performance using validation metrics.
* Generate predictions on test images.

### 3. YOLOv5 Training

* Train YOLOv5 using the same dataset.
* Compare training results with YOLOv8.
* Analyze mAP and fitness scores.

### 4. Faster R-CNN Training

* Build custom dataset loader using PyTorch.
* Train Faster R-CNN with annotated helmet images.
* Evaluate object detection performance.

### 5. Model Comparison

Compare:

* Precision
* Recall
* mAP@50
* mAP@50-95
* Fitness Score
* Inference Speed

---

## Model Architecture Comparison

### YOLOv8

* Anchor-Free Detection
* Improved feature extraction
* Better generalization
* Real-time performance

### YOLOv5

* Anchor-Based Detection
* Faster convergence
* Lightweight architecture
* Excellent for edge devices

### Faster R-CNN

* Two-stage detector
* High localization accuracy
* Slower inference speed
* Suitable when accuracy is prioritized over speed

---

## Evaluation Metrics

The following metrics were used:

* Precision
* Recall
* mAP@50
* mAP@50-95
* Fitness Score

These metrics help evaluate both detection accuracy and model robustness.

---

## Results

The trained models were evaluated and compared using:

* Validation Performance
* Prediction Accuracy
* Detection Quality
* Computational Efficiency

### Key Observation

YOLOv8 provides advanced feature learning and improved object localization.

YOLOv5 may achieve higher fitness scores in early training stages because of anchor-based detection, while YOLOv8 generally offers better scalability and modern architecture.

Faster R-CNN provides strong detection accuracy but is computationally more expensive compared to YOLO models.

---

## Applications

* Traffic Rule Enforcement
* Smart Surveillance Systems
* Construction Site Monitoring
* Industrial Safety Compliance
* Workplace Accident Prevention

---

## Project Structure

├── Dataset

├── XML Annotations

├── YOLOv8 Training

├── YOLOv5 Training

├── Faster R-CNN Training

├── Model Evaluation

├── Prediction Results

└── Face_Helmet_Detection.ipynb

---

## Future Improvements

* Real-time video detection
* Live CCTV integration
* Multi-class safety equipment detection
* Helmet color classification
* Deployment using Flask or Streamlit
* Edge deployment on Jetson Nano/Raspberry Pi

---

## Author

Harshit Singh Gusain

Computer Vision | Deep Learning | Machine Learning | Python
