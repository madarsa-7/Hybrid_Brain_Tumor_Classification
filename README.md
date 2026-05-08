# Brain Tumor Classification using Hybrid VGG19–ResNet50

A deep learning-based brain tumor classification system that combines the strengths of **VGG19** and **ResNet50** using **feature fusion** and **imbalance-aware learning** techniques for robust MRI image classification.

The model is designed to classify brain MRI scans into four categories:

* No Tumor
* Glioma
* Meningioma
* Pituitary Tumor

---

# Features

* Hybrid CNN architecture using **VGG19 + ResNet50**
* Feature-level fusion for enhanced representation learning
* Imbalance-aware learning using **Focal Loss**
* Data augmentation using **SMOTE** and **GAN-based techniques**
* Transfer learning with ImageNet pretrained weights
* MRI preprocessing and normalization pipeline
* Multi-class classification with high accuracy
* Grad-CAM visualization support for explainability

---

# Dataset

Dataset used: **BraTS2020**

The dataset contains MRI brain scans categorized into:

* No Tumor
* Glioma
* Meningioma
* Pituitary Tumor

Preprocessing steps:

* Slice extraction from MRI volumes
* Image resizing to `224x224`
* Intensity normalization
* Data augmentation

---

# Model Architecture

The framework uses two parallel CNN backbones:

## VGG19

* Captures fine-grained spatial features
* Effective for texture and edge learning

## ResNet50

* Uses residual learning
* Captures deep semantic representations

## Feature Fusion

Outputs from both networks are:

1. Flattened
2. Concatenated
3. Passed through dense layers
4. Classified using Softmax activation

---

# Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* OpenCV
* Scikit-learn
* Matplotlib

---

# Performance

| Metric         | Score |
| -------------- | ----- |
| Accuracy       | 88%   |
| Macro F1-Score | 85.5% |
| Average AUC    | 0.92  |

---


# Results

The hybrid architecture outperformed standalone CNN models such as:

* VGG19
* ResNet50
* Simple CNN

The feature fusion strategy significantly improved classification robustness and minority-class prediction.

---

# Future Improvements

* 3D MRI volume classification
* Attention mechanisms
* Vision Transformers (ViTs)
* Federated learning integration
* Clinical deployment pipeline

---

# Research Paper

This repository is based on the research work:

**“A Hybrid VGG19–ResNet50 Feature Fusion Framework with Imbalance-Aware Learning for Robust Brain Tumor Classification”**

---

# Authors

* D P Madarsa
* Team Members & Research Collaborators

---

# License

This project is intended for educational and research purposes.
