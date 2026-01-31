
---

# Brain Tumor Detection and Classification Using Deep Learning

## Project Overview

Brain tumors are abnormal growths of cells within the brain that can be either benign or malignant. Early detection and accurate classification of brain tumors are critical for effective treatment planning and improving patient survival rates.
This project presents a deep learning–based approach for automated brain tumor detection and multi-class classification using MRI images.

The system employs multiple models—**CNN, ResNet, GNN, and a hybrid CNN+GNN architecture**—to analyze brain MRI scans and classify them into four categories: **Glioma, Meningioma, Pituitary, and No Tumor**.

---

## Objectives

* To develop an automated system for brain tumor detection and classification using MRI images.
* To compare the performance of CNN, ResNet, GNN, and CNN+GNN models.
* To improve classification accuracy by combining spatial and structural feature learning.
* To assist clinicians with reliable diagnostic predictions.

---

## Dataset Description

The dataset used in this project is a combination of three publicly available datasets:

* **Figshare**
* **SARTAJ Dataset**
* **Br35H Dataset**

### Dataset Details:

* Total Images: **7023 brain MRI images**
* Classes:

  * Glioma
  * Meningioma
  * Pituitary
  * No Tumor
* The *No Tumor* images are sourced from the Br35H dataset.
* Glioma images from the SARTAJ dataset were replaced with Figshare images due to labeling inconsistencies.

### Dataset Structure:

```
dataset/
├── Training/
│   ├── glioma/
│   ├── meningioma/
│   ├── pituitary/
│   └── notumor/
└── Testing/
    ├── glioma/
    ├── meningioma/
    ├── pituitary/
    └── notumor/
```

---

## Methodology

1. **Data Collection:**
   MRI images are collected from multiple datasets covering four tumor classes.

2. **Data Preprocessing:**
   Images are resized, normalized, and denoised to ensure consistent input and improved model performance.

3. **Feature Extraction:**
   CNN and ResNet extract spatial features, while GNN captures relational and structural feature dependencies.

4. **Model Training:**
   CNN, ResNet, GNN, and CNN+GNN models are trained using labeled MRI images with the Adam optimizer.

5. **Model Evaluation:**
   Models are evaluated using accuracy, precision, recall, F1-score, and confusion matrices.

6. **Diagnosis Support:**
   The system outputs tumor class predictions and confidence scores to support clinical decision-making.

---

## Models Used

* Convolutional Neural Network (CNN)
* ResNet
* Graph Neural Network (GNN)
* Hybrid CNN + GNN Model

---

## Performance Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Tools and Technologies

* Python
* TensorFlow / PyTorch
* OpenCV
* NumPy, Pandas
* Matplotlib, Seaborn

---

## Results

The hybrid **CNN+GNN model** demonstrates improved classification performance compared to individual CNN, ResNet, and GNN models by effectively combining spatial and relational features.

---

## Conclusion

This project demonstrates that deep learning models, especially hybrid CNN+GNN architectures, can significantly enhance brain tumor detection and classification accuracy. The proposed system can serve as a supportive diagnostic tool for radiologists and healthcare professionals.

---

