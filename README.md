# Intelligent Systems — Coursework & Project

Coursework and final project developed for the Intelligent Systems course 
at Instituto Superior Técnico (IST), Master's in Mechanical Engineering 
— Specialization in Systems, Robotics and AI.

## Contents

### Assignments
- **A1 (Exercise 1 & 2)** — Core intelligent systems concepts and implementations
- **A2** — Advanced assignment covering machine learning techniques

### Final Project — Markerless Pose Estimation of Drosophila Locomotion
Trained and evaluated deep learning models for automated pose estimation 
of freely walking Drosophila using [SLEAP](https://sleap.ai/) 
(Social LEAP Estimates Animal Poses) — a state-of-the-art multi-animal 
pose tracking framework based on deep neural networks.

**Approach:**
- Labelled keypoints on Drosophila leg positions across multiple video recordings
- Trained U-Net based models on Google Colab using high-speed imaging data
- Compared baseline model vs data-augmented model performance
- Evaluated using OKS mAP (Object Keypoint Similarity mean Average Precision)

**Results:**

| Model | Val OKS mAP | Val p50 Distance (px) |
|---|---|---|
| Baseline U-Net | 0.906 | 1.36 |
| Augmented U-Net | 0.895 | 1.46 |

**Key finding:** Baseline model achieved strong performance (OKS mAP 0.906). 
Data augmentation did not improve results in this case, 
suggesting the baseline architecture generalised well to the validation set.

## Tech Stack
Python · SLEAP · Google Colab · Jupyter Notebook · U-Net

## Context
This project directly informed the methodology of my Master's thesis: 
[DL-Locomotion-Tracking](https://github.com/Vasquez-505/DL-Locomotion-Tracking) 
— developing a production-grade deep learning pipeline for markerless 
locomotion tracking in collaboration with NOVA Medical School.
