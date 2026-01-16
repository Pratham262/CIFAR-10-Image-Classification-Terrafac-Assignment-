# 🚀 CIFAR-10 Image Classification using Deep Learning

## 📌 Problem Understanding

Image classification is a core problem in computer vision where the task is to assign a correct label to an input image from a predefined set of classes. In real-world scenarios, image classification is used in applications such as self-driving cars, medical imaging, surveillance, and e-commerce product recognition.

The CIFAR-10 dataset is a standard benchmark dataset consisting of low-resolution (32×32) color images belonging to 10 different object categories. Due to small image size, background clutter, and visual similarity between some classes (e.g., cat vs dog, truck vs automobile), accurate classification is challenging and requires robust feature extraction methods.

The objective of this project is to design and train a deep learning model that can automatically learn visual features from images and correctly classify them into one of the 10 CIFAR-10 categories using Convolutional Neural Networks (CNNs) and transfer learning techniques.

---

## 📘 Project Overview

This project implements an end-to-end deep learning pipeline for CIFAR-10 image classification using transfer learning with ResNet50. The model is trained in multiple stages:

- Baseline model using pre-trained ResNet50
- Performance improvement using data augmentation and regularization
- Detailed evaluation using confusion matrix, classification report, and class-wise accuracy
- Visualization of training curves and misclassified samples

The project demonstrates how modern deep learning techniques can be applied to small-scale image datasets with strong generalization performance.

---

## 📊 Dataset

- **Name:** CIFAR-10  
- **Total Images:** 60,000  
- **Image Size:** 32 × 32 (RGB)  
- **Classes (10):**  
  Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck  
- **Split:**  
  - Training: 50,000 images  
  - Testing: 10,000 images  

The dataset is directly loaded using TensorFlow/Keras utilities.

---

## 🧠 Model Architecture

- Pre-trained **ResNet50** as feature extractor
- Input resizing to match ResNet requirements
- Custom fully connected layers
- Batch Normalization and Dropout for regularization
- Softmax output layer for multi-class classification

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Deep Learning:** TensorFlow / Keras  
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn  
- **Environment:** Google Colab / Jupyter Notebook / VS Code  

---

## ⚙️ Setup Instructions

### ✅ Option 1: Run on Google Colab (Recommended)

1. Open Google Colab: https://colab.research.google.com/
2. Upload the notebook file:
   - `CIFAR-10.ipynb`
3. Set runtime:
   - Runtime → Change runtime type → GPU
4. Run all cells sequentially

TensorFlow and all required libraries are pre-installed on Colab.

---

### ✅ Option 2: Run Locally (VS Code / Jupyter)

# ================================
# STEP 1: CLONE REPOSITORY
# ================================
git clone https://github.com/Pratham262/CIFAR-10-Image-Classification-Terrafac-Assignment-


# ================================
# STEP 2: CREATE VIRTUAL ENV (OPTIONAL)
# ================================
python -m venv venv
venv\Scripts\activate        # Windows
# source venv/bin/activate   # Linux/Mac


# ================================
# STEP 3: INSTALL LIBRARIES
# ================================
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn


# ================================
# STEP 4: RUN JUPYTER NOTEBOOK
# ================================
jupyter notebook
# Open: cifar10_resnet_classification.ipynb




