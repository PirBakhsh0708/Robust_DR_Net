# RobustDRNet – Diabetic Retinopathy Classification & Explainability

This repository provides a modular pipeline for training, evaluating, and explaining deep‑learning models for Diabetic Retinopathy (DR) classification.

## Notebooks Included

### 1. Base Models.ipynb
Contains:
- Dataset loading and augmentation
- Focal loss implementation
- Base CNN model training (ResNet, ConvNeXt)
- Wrapper utilities

### 2. RobustDRNet_Original.ipynb
Implements:
- Preprocessing and loaders
- Feature-level fusion (concatenation)
- Hybrid ensemble (soft, hard, weighted, stacking)
- RobustDRNet classifier pipeline

### 3. Explainability Suite-Original.ipynb
Includes:
- LogitWrapper utility
- Loading explainability-ready models
- Explainability methods such as Grad-CAM, IG, occlusion, etc.

## Workflow

1. Train base models → `Base Models.ipynb`
2. Build RobustDRNet fusion/ensemble → `RobustDRNet_Original.ipynb`
3. Generate explainability outputs → `Explainability Suite-Original.ipynb`

## Requirements

Install dependencies:

```
pip install -r requirements.txt
```

## Project Structure

```
project/
│── Base Models.ipynb
│── RobustDRNet_Original.ipynb
│── Explainability Suite-Original.ipynb
│── models/
│── data/
│── results/
│── README.md
│── requirements.txt
│── .gitignore
```

## License
MIT License (or your preferred license).
