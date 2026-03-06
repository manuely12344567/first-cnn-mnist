# 🧠 First-CNN-MNIST

> A simple and educational implementation of a Convolutional Neural Network (CNN) for handwritten digit classification.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow&logoColor=white)
![Dataset](https://img.shields.io/badge/Dataset-MNIST-lightgrey)

---

## 📌 Overview

This project implements a CNN to classify handwritten digit images using the **MNIST dataset**.  
It is designed to be simple, readable, and educational — perfect for beginners exploring deep learning.

- 🏗️ **TensorFlow / Keras** — model building & training  
- 📊 **Matplotlib** — result visualization & error analysis

---

## 🗂️ Project Structure

```
First-CNN-MNIST/
├── model/
│   └── cnn_mnist.py        # Model definition and training
├── utils/
│   └── visualize.py        # Visualization utilities
├── notebooks/
│   └── exploration.ipynb   # Jupyter notebook for exploration
├── requirements.txt
└── README.md
```

---

## 🧱 Model Architecture

```
Input: 28×28 grayscale image
    │
    ▼
Reshape (28, 28, 1)         → Prepares image for CNN (1 channel)
    │
    ▼
Conv2D + ReLU               → Detects patterns and shapes
    │
    ▼
MaxPooling2D                → Reduces feature map size, keeps key info
    │
    ▼
Flatten                     → Converts matrix to 1D vector
    │
    ▼
Dense(128, ReLU)            → Deep analysis of extracted features
    │
    ▼
Dense(10, Softmax)          → Predicts digit (0 to 9)
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/First-CNN-MNIST.git
cd First-CNN-MNIST
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the model

```bash
python model/cnn_mnist.py
```

---

## 📦 Requirements

```
tensorflow>=2.0
matplotlib
numpy
```

> Install all dependencies with:
> ```bash
> pip install -r requirements.txt
> ```

---

## 📈 Results

| Metric       | Value     |
|--------------|-----------|
| Dataset      | MNIST     |
| Input shape  | 28×28×1   |
| Output classes | 10      |
| Optimizer    | Adam      |
| Loss         | Sparse Categorical Crossentropy |

---

## 📚 Dataset

The **MNIST** dataset contains 70,000 grayscale images of handwritten digits (0–9):
- 60,000 training images
- 10,000 test images

It is automatically downloaded via `tensorflow.keras.datasets.mnist`.

---



<p align="center">Made with ❤️ to learn Deep Learning</p>
