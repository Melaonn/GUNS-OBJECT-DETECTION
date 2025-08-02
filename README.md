# 🔫 Custom Gun Object Detection - End-to-End MLOps Project

This project demonstrates an end-to-end deep learning pipeline for detecting guns in images using a custom object detection model. It includes data ingestion, model training, versioning, experiment tracking, and an API for real-time predictions.

---

## 🚀 Overview

The workflow includes:

- Dataset loading directly from Kaggle  
- Data preprocessing and augmentation  
- Model architecture design and training  
- Experiment tracking using TensorBoard  
- Pipeline creation and versioning with DVC  
- Real-time inference via FastAPI with Swagger UI & Postman api.

---

## 🧰 Tech Stack & Workflow

### 📥 Data Ingestion
- **Kaggle API**: Used to fetch custom gun detection dataset directly.
- **Jupyter Notebooks**: For exploration, visualization, and initial preprocessing.

### 🧹 Data Processing
- Data cleaning, annotation parsing (e.g., COCO or Pascal VOC formats).
- Augmentations using libraries like Albumentations or OpenCV.

### 🧠 Model Development
- **Model Architecture**: Custom CNN or YOLO-based object detector.
- Built using **TensorFlow**, **Keras**, or **PyTorch**.

### 🏋️ Model Training & Tracking
- Training handled via scripts with configurable hyperparameters.
- **TensorBoard**: For visualizing training metrics like loss, mAP, precision, and recall.

### 📦 Training Pipeline & Versioning
- **DVC (Data Version Control)**: For managing datasets, models, and pipeline stages.
- Reproducible training with stage-wise execution (`dvc.yaml`).

### 🧪 Experiment Tracking
- TensorBoard logs stored and versioned with DVC.
- Easily compare model runs and performance.

### 🌐 API for Prediction
- **FastAPI** backend with:
  - `/predict` endpoint to upload an image and get predictions.
  - Auto-generated docs via **Swagger UI**.
- **Postman** used for external testing and validation.
