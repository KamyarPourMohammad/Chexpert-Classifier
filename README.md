# Multi-Label Chest X-ray Classification with XAI
### Automated Pathology Detection using DenseNet121

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-green?style=for-the-badge)

---

## Project Overview
This repository implements a deep learning pipeline for detecting 10 distinct pathologies from chest radiograph images. By leveraging the **DenseNet121** architecture and **Explainable AI (XAI)** techniques, the model provides both high-accuracy predictions and visual justifications for its decisions.

## Key Technical Features
* **Architecture:** DenseNet121 (Pre-trained on ImageNet)
* **Dataset:** CheXpert (Large-scale chest X-ray dataset)
* **Learning Paradigm:** Multi-label Classification
* **Interpretability:** Integrated Grad-CAM support for clinical verification
* **Optimization:** Adam optimizer with Cosine Annealing learning rate scheduling

---

## Visual Interpretability (XAI)
To ensure clinical trust, this project utilizes **Grad-CAM** (Gradient-weighted Class Activation Mapping). This allows the model to produce heatmaps that highlight the specific anatomical regions contributing to a particular diagnosis.

> **Note:** A sample heatmap visualization of the lung regions can be placed here to demonstrate model transparency.

---

## Model Performance
The model is evaluated based on the Area Under the Curve (AUC) for each clinical label.

| Pathology | AUC Score | Performance Level |
| :--- | :---: | :--- |
| **Pneumothorax** | 0.85 | Excellent |
| **Edema** | 0.82 | High |
| **Cardiomegaly** | 0.79 | Good |
| **Consolidation** | 0.76 | Stable |
| **Macro Average** | **0.83** | **Optimal** |

---

## Installation and Usage

### Prerequisites
Ensure you have Python 3.8+ installed. You can install the dependencies using:

```bash
pip install torch torchvision torchxrayvision matplotlib pandas numpy
