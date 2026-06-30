# ML_Task03_Deepfake-Detection\
# 🛡️ Simple Deepfake Image Detector (Task 3)

## 📌 Project Overview
This project applies machine learning to digital forensics by using an optimized K-Nearest Neighbors (KNN) classifier to detect deepfake images. 

Instead of processing heavy convolutional neural networks, this tool extracts structural metrics from an uploaded image—such as visual artifacts, lighting variations, and compression traits—and classifies them against a forensic dataset to determine authenticity.

---

## 📊 How It Works & Optimization
The app runs a **K-Nearest Neighbors (KNN)** classifier optimized for precision.

* **The Interface:** Upload any face image file to the dashboard. The application handles feature mapping dynamically and outputs a clear **REAL** or **FAKE** verdict along with a confidence percentage.
* **Optimization Layer:** Standard baseline KNN models are easily thrown off by outlier data noise. For this project, hyperparameter tuning was applied to determine the optimal neighborhood window ($K=7$) using distance-based weights to maximize classification boundaries.

---

## ⚙️ How to Run It Locally

If you want to run this code on your machine or inside Google Colab, follow these simple steps:

1. **Install the required libraries:**
   ```bash
   pip install gradio pandas scikit-learn numpy kagglehub opencv-python
