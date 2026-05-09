# 🚀 6CS012 Deep Learning Portfolio

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow%20/%20Keras-orange.svg)](https://www.tensorflow.org/)
[![Status](https://img.shields.io/badge/Status-Complete-green.svg)]()

This repository contains the comprehensive research and implementation for my Deep Learning portfolio, focusing on two primary domains: **Computer Vision** and **Natural Language Processing (NLP)**.

---

## 🖼️ Task 2: Intra-class Variation in Image Classification
### **Objective**
The goal was to build a robust model capable of distinguishing between plant species (e.g., Apple vs. Grape) while handling high intra-class variation (differences in lighting, angle, and health within the same species).

### **Technical Implementation**
* **Architecture:** Comparative analysis between a **Baseline CNN** and **MobileNetV2 Transfer Learning**.
* **Techniques:** Global Average Pooling, Dropout (0.2), and Data Augmentation (Rotation, Zoom, Horizontal Flip).
* **Results:** Transfer learning significantly reduced training time and improved validation accuracy by leveraging pre-trained ImageNet weights.



---

## 📰 Task 3: Sarcasm Detection in News Headlines
### **Objective**
Implementing a binary classification pipeline to identify sarcasm in a dataset of 28,619 news headlines. This task focuses on solving the long-term dependency problem in sequential text.

### **Technical Implementation**
* **Data Preprocessing:** Custom regex-based cleaning, NLTK-based lemmatization, and stopword removal.
* **Model Comparison:** Benchmarked **SimpleRNN** against **LSTM** architectures.
* **Optimization:** Integrated **Word2Vec** pre-trained embeddings to provide semantic context.

### **Performance Metrics**
| Model Variant | Accuracy | Observation |
| :--- | :--- | :--- |
| **SimpleRNN** | ~78.5% | High training accuracy (96%) with significant overfitting. |
| **LSTM (Baseline)** | ~80.4% | Improved stability via gating mechanisms. |
| **LSTM + Word2Vec** | **85%** | Peak performance with best generalization. |



---

## 🛠️ Tech Stack
* **Language:** Python 3.12
* **Frameworks:** TensorFlow, Keras
* **Libraries:** NLTK, NumPy, Pandas, Matplotlib, Scikit-learn
* **Environment:** Google Colab / Linux (KDE Plasma)

---

## 📂 Project Structure
```bash
.
├── Task2_Image_Classification.ipynb   # Computer Vision implementation
├── Task3_Sarcasm_Detection.ipynb      # NLP implementation
├── datasets/                          # Local data storage
├── models/                            # Saved .keras weights
└── README.md                          # Documentation
