# Deep Learning for Wildlife Trail Cam Classification

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/DeepLearning_Trailcam_classification/blob/main/YOUR_NOTEBOOK.ipynb)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-ee4c2c.svg)](https://pytorch.org/)

An interactive Google Colab teaching laboratory designed for **beginner ecology and biology students**. This hands-on module introduces computer vision and transfer learning for wildlife monitoring using deep neural networks, quantitative validation, and geospatial deployment.

By Joschka Wiegleb

---

## Overview

Camera traps and community science platforms generate millions of wildlife images every year. Manual classification creates a massive bottleneck for conservation research. 

This notebook guides students through training, evaluating, and deploying a pre-trained deep convolutional neural network (PyTorch) to automatically identify 5 target species:

* **White-tailed Deer** (*Odocoileus virginianus*)
* **Raccoon** (*Procyon lotor*)
* **Coyote** (*Canis latrans*)
* **Wild Turkey** (*Meleagris gallopavo*)
* **Eastern Gray Squirrel** (*Sciurus carolinensis*)

---

## 💡 Key Learning Objectives

1. **Transfer Learning Fundamentals:** Understand how pre-trained computer vision models (ImageNet backbone) adapt to ecological tasks with minimal training time.
2. **Learning Curve & Overfitting Analysis:** Recognize the 3 stages of model learning (underfitting, optimal performance, and background memorization) using dual-axis loss and accuracy plots.
3. **Model Performance Metrics:** Interpret confusion matrices, Precision, Recall, Accuracy, and F1-Scores beyond standard overall accuracy.
4. **Scaled Field Deployment:** Process 1,000 unseen field photos, export structured metadata to Excel, and generate interactive spatial maps.

---

## Dual Dataset Pathways

Students can choose between two dataset paths early in the notebook depending on their learning focus:

| Option | Dataset Source | Image Type | Downstream Focus |
| :--- | :--- | :--- | :--- |
| **Option A (Cell 2a)** | **iNaturalist** | Citizen science photos (smartphones/cameras) | **Cell 8:** Global species distribution & geospatial mapping across continents. |
| **Option B (Cell 2b)** | **AMMonitor** *(LILA BC)* | Motion-activated forest camera traps | **Cell 7:** Local camera trap evaluation (handling fixed backgrounds, night shots, and motion blur). |

---

## Notebook Structure

```text
├── Cell 1: Environment Setup & GPU Verification
├── Cell 2: Dataset Selection (Option 2a: iNaturalist OR Option 2b: AMMonitor)
├── Cell 3: Data Transformations & Augmentation
├── Cell 4: Model Architecture & Transfer Learning Setup
├── Cell 5: Training Loop & Overfitting Visualization (Loss/Accuracy Curves)
├── Cell 6: Quantitative Validation (Metrics Report & Confusion Matrix)
├── Cell 7: Local Camera Trap Field Deployment (AMMonitor Focus)
├── Cell 8: Global Deployment, Excel Export & Interactive World Maps (iNaturalist Focus)
└── Cell 9: References & Data Acknowledgments
```
