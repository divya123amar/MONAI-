# 🧠 Brain Tumor Segmentation Using MONAI

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue.svg">
  <img src="https://img.shields.io/badge/PyTorch-Deep%20Learning-red.svg">
  <img src="https://img.shields.io/badge/MONAI-Medical%20AI-green.svg">
  <img src="https://img.shields.io/badge/Medical-Imaging-orange.svg">
</p>

---

# Overview

This repository demonstrates the implementation of **Brain Tumor Segmentation** using the **Medical Open Network for AI (MONAI)** framework.

MONAI is an open-source deep learning framework built on PyTorch and designed specifically for healthcare imaging applications. It provides optimized tools for medical image preprocessing, augmentation, training, inference, and evaluation.

The objective of this project is to build an end-to-end medical image segmentation pipeline for multi-modal MRI brain tumor images.

---

# Features

✔ Medical image preprocessing using MONAI transforms

✔ MRI data loading from NIfTI files

✔ Multi-modal MRI support

✔ Data augmentation pipeline

✔ Patch-based training

✔ Sliding Window Inference

✔ Dice Metric Evaluation

✔ PyTorch-based implementation

✔ Research-oriented workflow

---

# Dataset

This project uses the **Brain Tumor Segmentation (BraTS)** dataset.

MRI Modalities

- T1
- T1ce
- T2
- FLAIR

Segmentation Labels

- Background
- Enhancing Tumor (ET)
- Tumor Core (TC)
- Whole Tumor (WT)

> **Note:** The BraTS dataset is not included in this repository because it requires registration and acceptance of the Data Use Agreement.

---

# Why MONAI?

MONAI simplifies medical imaging research by providing:

- Optimized medical image transforms
- GPU-accelerated workflows
- Built-in loss functions
- Medical segmentation metrics
- Sliding Window Inference
- Smart caching datasets
- Support for 2D and 3D medical imaging

---

# Repository Structure

```
MONAI-Brain-Tumor-Segmentation/

│
├── dataset/
│
├── notebooks/
│
├── preprocessing/
│
├── models/
│
├── training/
│
├── inference/
│
├── evaluation/
│
├── utils/
│
├── train.py
├── predict.py
├── requirements.txt
└── README.md
```

---

# Workflow

```
BraTS Dataset

↓

Load MRI Images

↓

MONAI Transforms

↓

Data Augmentation

↓

Dataset & DataLoader

↓

Model Training

↓

Validation

↓

Sliding Window Inference

↓

Performance Evaluation
```

---

# MONAI Components Used

## Data Loading

- LoadImaged
- EnsureChannelFirstd
- Orientationd
- Spacingd

---

## Preprocessing

- ScaleIntensityRanged
- NormalizeIntensityd
- CropForegroundd

---

## Data Augmentation

- RandFlipd
- RandRotate90d
- RandShiftIntensityd
- RandScaleIntensityd

---

## Training

- CacheDataset
- DataLoader
- DiceLoss
- Adam Optimizer

---

## Validation

- DiceMetric
- Sliding Window Inference

---

## Visualization

- Matplotlib
- MONAI Visualization Utilities

---

# Model

This repository supports medical image segmentation models developed using MONAI.

Example architectures include:

- 3D U-Net
- UNETR
- SwinUNETR
- SegResNet

(Modify according to the model used in your implementation.)

---

# Installation

Clone the repository

```bash
[git clone https://github.com/yourusername/MONAI-Brain-Tumor-Segmentation.git](https://github.com/divya123amar/MONAI-.git)
```

Move into the project directory

```bash
cd MONAI-Brain-Tumor-Segmentation
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# Requirements

- Python 3.10+
- PyTorch
- MONAI
- NumPy
- Matplotlib
- NiBabel
- SimpleITK
- Scikit-Learn

---

# Training

Run

```bash
python train.py
```

---

# Inference

```bash
python predict.py
```

---

# Evaluation Metrics

The following metrics are used to evaluate segmentation performance:

- Dice Similarity Coefficient
- Intersection over Union (IoU)
- Precision
- Recall
- Accuracy
- Hausdorff Distance (optional)

---

# Sample Pipeline

```
MRI Images

↓

MONAI Preprocessing

↓

Data Augmentation

↓

Deep Learning Model

↓

Predicted Segmentation

↓

Evaluation Metrics
```

---

# Future Improvements

- Federated Learning with MONAI
- Differential Privacy
- Vision Transformers
- MONAI Label Integration
- Interactive Annotation
- Explainable AI
- 3D Visualization
- Multi-site Medical AI

---

# Research Applications

This repository can be used for:

- Brain Tumor Segmentation
- Medical Image Analysis
- Healthcare AI Research
- Deep Learning Education
- Biomedical Image Computing
- Computer Vision Research

---

# Author

**Divyashree A**

PhD Research Scholar

Research Interests

- Artificial Intelligence
- Deep Learning
- Computer Vision
- Medical Image Analysis
- Federated Learning
- Healthcare AI

---

# Citation

If you use this repository in your research, please cite:

- The MONAI framework
- The BraTS Challenge dataset
- Any associated publications related to this implementation

---

# License

This project is intended for research and educational purposes.
