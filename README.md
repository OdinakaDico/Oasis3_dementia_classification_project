# Oasis3_dementia_classification_project
Medical image classification project using OASIS-3 MRI data and PyTorch to classify cognitively normal vs dementia cases.
# OASIS3 MRI Classification

## Project Overview

This project focuses on binary classification of cognitive status from T1-weighted brain MRI using deep learning and PyTorch.

The objective is to classify MRI scans into:
- Cognitively normal
- Dementia

using MRI data from the OASIS-3 dataset.

This project is part of the course:

**Data Analytic – Medical Image Analysis and Machine Learning**

---

## Dataset

We use the **OASIS-3** dataset, which contains:
- T1-weighted MRI brain scans
- Clinical metadata such as age and diagnosis
- Clinical Dementia Rating (CDR)

### Labels
- `CDR = 0` → Normal
- `CDR ≥ 1` → Dementia
- `CDR = 0.5` cases are excluded

### Age Range
Subjects between:
- 60–85 years

---

## Project Goal

The goal is to build a deep learning model that can classify brain MRI scans into:
- normal
- dementia

using supervised learning.

---

## Planned Pipeline

### Data Preprocessing
- Remove missing metadata values
- Select one scan session per subject
- Match MRI scans with clinical labels
- Filter subjects by age

### MRI Processing
- Use `T1w_norm_noskull.nii.gz`
- Convert 3D MRI volumes into 2D slices
- Select homogeneous middle slices

### Model
- PyTorch
- Pretrained ResNet18

---

## Expected Challenges
- Class imbalance
- Noisy or empty MRI slices
- Multiple sessions per subject
- Metadata cleaning

### Planned Solutions
- Data filtering and cleaning
- Slice selection
- Data augmentation
- Proper train/validation splitting

---

## Repository Structure

```text
data/
  metadata/
  splits/

notebooks/
reports/
results/
src/
```

---

## Team
Bachelor student group project.
