# 🔢 MNIST Handwritten Digit Classification using Deep Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?logo=keras)
![Accuracy](https://img.shields.io/badge/Test%20Accuracy-97.04%25-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow?logo=googlecolab)

> **AI/ML Project — **
> A complete end-to-end deep learning project that trains a Neural Network to classify handwritten digits (0-9) from images.

---

## 📌 Project Overview

This project uses the **MNIST dataset** to build a Deep Neural Network that can automatically recognize handwritten digits. The model is trained on 60,000 images and achieves **97.04% accuracy** on 10,000 unseen test images. The project also tests the model on a **custom real handwritten digit image**.

---

## 🎯 Objectives

- Load and explore the MNIST dataset
- Preprocess and normalize image data
- Build a multi-layer Neural Network using TensorFlow/Keras
- Train the model and achieve >95% accuracy
- Evaluate using accuracy metrics and confusion matrix
- Test on a real custom handwritten digit image

---

## 📁 Repository Structure

```
MNIST-Digit-Classification/
├── MNIST_Digit_Classification_Colab.ipynb   <- Main Google Colab notebook
├── MNIST_Project_Report.docx                <- Detailed project report
├── MNIST_Digit_Classification.pptx          <- 11-slide PowerPoint presentation
├── 3-digit.PNG                              <- Sample custom test image
└── README.md                               <- You are here
```

---

## 🗂️ Dataset

| Property | Details |
|----------|---------|
| Name | MNIST |
| Total Images | 70,000 grayscale images |
| Training Set | 60,000 images |
| Test Set | 10,000 images |
| Image Size | 28 x 28 pixels |
| Classes | 10 (digits 0 through 9) |
| Source | keras.datasets.mnist |

---

## 🧠 Model Architecture

```
Input (28x28 image) → Flatten → Dense(50, ReLU) → Dense(50, ReLU) → Dense(10, Sigmoid)
```

| Layer | Units | Activation |
|-------|-------|------------|
| Flatten | 784 | - |
| Dense (Hidden 1) | 50 | ReLU |
| Dense (Hidden 2) | 50 | ReLU |
| Dense (Output) | 10 | Sigmoid |

**Optimizer:** Adam | **Loss:** Sparse Categorical Crossentropy | **Epochs:** 10

---

## 📊 Results

| Metric | Value |
|--------|-------|
| Training Accuracy | 98.90% |
| **Test Accuracy** | **97.04%** |
| Test Loss | 0.1340 |
| Correctly Classified | 9,704 / 10,000 |

---

## 🚀 How to Run

### Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/)
2. Click File → Upload notebook
3. Upload `MNIST_Digit_Classification_Colab.ipynb`
4. Click Runtime → Run all

### Local Setup

```bash
git clone https://github.com/YOUR_USERNAME/MNIST-Digit-Classification.git
cd MNIST-Digit-Classification
pip install tensorflow numpy matplotlib seaborn pillow opencv-python
jupyter notebook MNIST_Digit_Classification_Colab.ipynb
```

---

## 🛠️ Tech Stack

- Python 3.x
- TensorFlow 2.x + Keras
- NumPy, Matplotlib, Seaborn
- OpenCV, PIL (Pillow)
- Google Colab

---

## 📝 Key Learnings

- A simple 3-layer neural network achieves 97%+ accuracy on MNIST
- Normalizing pixel values is critical for training stability
- The confusion matrix reveals which digit pairs are most commonly confused
- Adam optimizer converges efficiently for multi-class classification
- Proper image preprocessing is essential for real-world deployment

---

## 👤 Author

**AI/ML | Harshada Patil**
