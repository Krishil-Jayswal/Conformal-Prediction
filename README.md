# 🧠 Conformal Prediction with Tube Loss

This repository contains our research on **Conformal Prediction** using a novel and computationally efficient scoring function called **TubeLoss**. The project compares **TubeLoss** with the widely used **Conformalized Quantile Regression (CQR)** and demonstrates that TubeLoss can **reduce training time by approximately 50%** while maintaining competitive performance.

We employ **Artificial Neural Networks (ANNs)** for regression tasks and evaluate both methods across multiple real-world datasets.

---

## 🚀 Overview

Conformal prediction is a framework for creating reliable prediction intervals with finite-sample guarantees. Our work focuses on improving its computational efficiency by introducing:

- **TubeLoss**: A custom loss function that produces well-calibrated prediction intervals with significantly faster training times.
- **CQR (Conformalized Quantile Regression)**: A strong baseline using quantile regression and pinball loss.

---

## 📊 Datasets

We tested our approach on the following benchmark datasets:

- Concrete Strength
- Bike Sharing
- Star (Stellar Properties)
- Communities and Crime
- Facebook Metrics
- Boston Housing
- Naval Propulsion
- Yacht Hydrodynamics
- Auto MPG

Each dataset varies in size and complexity, providing a broad base for comparing the performance of both methods.

---

## 📈 Results

We report the following evaluation metrics for both TubeLoss and CQR:

- **PICP**: Prediction Interval Coverage Probability
- **MPIW**: Mean Prediction Interval Width
- **Training Time**

Our results consistently show that **TubeLoss provides competitive PICP and MPIW scores while cutting down training time by almost half** in most cases.

---

## 🔍 Highlights

- ✅ Introduced **TubeLoss**, a simple yet effective loss function for conformal prediction.
- 🧠 Used **neural networks** for all experiments.
- ⚡ Achieved significant speedups over standard CQR.
- 📁 Results are saved for each dataset and ready for analysis.

---

## 🧪 Future Work

We plan to extend this work by:

- Integrating other model architectures (e.g., gradient boosting, transformers).
- Supporting heteroscedastic uncertainty modeling.
- Publishing a package for easy integration of TubeLoss into conformal pipelines.