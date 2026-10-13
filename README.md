# 🔢 MNIST Digit Recognition Project

## 📌 Overview
This project implements a deep learning model to classify handwritten digits (0–9) from the **MNIST dataset**.  
The MNIST dataset is a benchmark in computer vision and machine learning, containing 70,000 grayscale images of digits.  
Our goal is to build, train, and evaluate models that can accurately recognize digits, demonstrating the power of neural networks.

---

## 📂 Dataset
- **Source:** MNIST dataset (available via TensorFlow/Keras).  
- **Format:** Grayscale images of size 28×28 pixels.  
- **Classes:** 10 categories (digits 0–9).  
- **Samples:**  
  - Training set: 60,000 images  
  - Test set: 10,000 images  

---

## ⚙️ Preprocessing
- Normalized pixel values to range [0,1].  
- Reshaped images to 28×28×1 for CNN input.  
- One-hot encoded labels for multi-class classification.  

---

## 🏗️ Methodology
We implemented and compared multiple models:

1. **Dense Neural Network (Baseline)** – fully connected layers.  
2. **Convolutional Neural Network (CNN)** – convolution + pooling layers for feature extraction.  
3. **Improved CNN** – deeper architecture with dropout for regularization.  

**Architecture Highlights:**
- Convolutional layers with ReLU activation.  
- MaxPooling layers for dimensionality reduction.  
- Dense layers for classification.  
- Softmax output layer for 10-class prediction.  

---

- Accuracy/Loss curves plotted for training and validation.  
- Confusion Matrix used to analyze misclassified digits.  
- Sample predictions visualized for demonstration.  

---

## 🔑 Insights
- Dense NN performs well but struggles with complex visual features.  
- CNN significantly improves accuracy by learning spatial patterns.  
- Improved CNN with dropout achieves near state-of-the-art performance.  

---

## 🚀 Enhancements
Future improvements could include:
- Data augmentation (rotation, shifting, scaling).  
- Transfer learning with pre-trained vision models.  
- Deployment as a web app for real-time digit recognition.  

---

## 📝 Summary
This project demonstrates the effectiveness of deep learning for handwritten digit recognition.  
By preprocessing data, experimenting with different architectures, and evaluating results, we achieved **~99% accuracy** on the MNIST dataset.  

**Key Takeaway:**  
Convolutional Neural Networks (CNNs) are highly effective for digit recognition and can be extended to other handwriting recognition tasks such as postal code reading or bank check processing.

---

## 📌 Requirements
- Python 3.x  
- TensorFlow / Keras  
- NumPy, Matplotlib, Seaborn  

Install dependencies:
```bash
pip install tensorflow numpy matplotlib seaborn
