# 🌊 Flood Area Segmentation with U-Net (Keras)
This project focuses on segmenting flooded areas from satellite images using a **U-Net** deep learning model implemented with **Keras** and **TensorFlow**. The goal is to perform pixel-wise classification (semantic segmentation) to automatically identify flooded zones, which can be useful for disaster management and response.


## 📌 Project Overview
- **Task**: Binary Semantic Segmentation (Flood vs. No Flood)
- **Model**: U-Net (Convolutional Neural Network)
- **Framework**: TensorFlow + Keras
- **Dataset**: Satellite images and corresponding binary masks (flood annotations)
- **Metrics**: Accuracy, Loss, IoU (Intersection over Union)
- **Visuals**: Training history, segmented image results, and IoU evaluation


## 📂 Dataset
We use the [Flood Area Segmentation - Dataset](https://www.kaggle.com/datasets/faizalkarim/flood-area-segmentation/data). The dataset contains images of flood hit areas and corresponding mask images showing the water region. There are 290 images and self annoted masks. The dataset is automatically downloaded using `kagglehub`.


## Download the dataset using kagglehub
```
import kagglehub

# Download latest version
path = kagglehub.dataset_download("faizalkarim/flood-area-segmentation")

print("Path to dataset files:", path)
```


## 🧠 Model Used: U-Net Architecture

**U-Net** is a convolutional neural network architecture specifically designed for semantic segmentation. It was introduced in the paper: [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597) by Ronneberger et al.


## 📊 Features
- ✅ U-Net architecture with customizable input size
- 📁 Data pipeline using ImageDataGenerator
- 📈 Real-time training visualization (Accuracy / Loss)
- 📸 Segmented image visualization
- 📐 IoU (Intersection over Union) score computation


## 📈 Metrics and Evaluation
- Loss Function: Binary Cross-Entropy
- Accuracy: Pixel-wise accuracy
- IoU (Jaccard Index): Measures overlap between prediction and ground truth


## 📘 Language
- Python
