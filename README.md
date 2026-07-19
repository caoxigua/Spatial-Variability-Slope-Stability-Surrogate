# Active-Learning-Surrogate-for-Slope-Stability
Surrogate modeling framework and benchmark datasets for efficient slope stability analysis considering spatial variability using deep learning and active learning.
# Surrogate Modeling for Slope Stability Analysis Considering Spatial Variability

This repository provides the datasets, trained models, and source codes associated with the surrogate modeling framework developed for efficient slope stability analysis considering spatial variability.

The proposed framework integrates high-fidelity numerical simulation-based datasets with deep learning surrogate models and active learning strategies to efficiently predict slope stability responses, including factor of safety (Fs), displacement fields, strain fields, and critical slip surfaces (CSS).

The repository is developed to support the reproducibility and further application of the research presented in:

> "Physics-driven surrogate modeling with active learning for slope stability analysis considering spatial variability"

---

## Overview

Spatial variability of soil properties introduces significant uncertainty into slope stability analysis. Traditional Monte Carlo simulations based on high-fidelity numerical methods are computationally expensive, making large-scale uncertainty analysis challenging.

This repository provides the implementation of a surrogate modeling framework that enables efficient prediction of slope stability responses using:

- CNN-based surrogate model for factor of safety prediction;
- U-Net-based surrogate model for displacement and strain field prediction;
- Active learning strategies for informative sample selection;
- Processed benchmark datasets for model training and evaluation.

---

## Repository Structure
