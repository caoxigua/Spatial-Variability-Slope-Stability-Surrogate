# Spatial-Variability-Slope-Stability-Surrogate
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

# Dataset

The dataset contains processed input-output pairs used for training and evaluating surrogate models.

## Input

The input consists of spatially variable soil parameter fields:

- Cohesion fields
- Internal friction angle fields

## Output labels

The corresponding outputs include:

- Factor of safety (Fs)
- Displacement fields
- Strain fields
- Critical slip surface (CSS) information

The dataset is provided in a format directly usable for deep learning model training.

---

# Surrogate Models

## CNN model

The CNN-based surrogate model is developed for predicting scalar factor of safety:

\[
Input\ random\ fields \rightarrow F_s
\]

The model provides efficient prediction of Fs without additional high-fidelity numerical calculations.

---

## U-Net model

The U-Net architecture is employed for high-dimensional field prediction:

\[
Input\ random\ fields
\rightarrow
Displacement/strain\ fields
\]

The predicted displacement and strain fields are further used for critical slip surface identification.

---

# Active Learning

The repository includes different active learning strategies:

- Least Confidence Sampling (LCUS)
- Margin Sampling
- Entropy Sampling

These methods are used to identify informative samples and improve surrogate model performance with fewer training samples.

---

# Trained Models

Pre-trained models are provided for reproducing the prediction results reported in the paper.

The provided models include:

- CNN model for Fs prediction;
- U-Net model for displacement and strain field prediction.

---

# Reproducibility

To reproduce the reported results:

1. Download the dataset.
2. Install the required Python packages.
3. Train or load the provided surrogate models.
4. Run prediction scripts.
5. Compare the predicted results with the provided benchmark results.

---

# Requirements

The codes are developed using:

- Python >= 3.8
- PyTorch
- NumPy
- Scikit-learn
- Matplotlib

---

# Note

The high-fidelity numerical solver used to generate the training datasets is not included in this repository.

This repository provides the processed datasets, surrogate modeling framework, trained models, and prediction procedures required to reproduce the machine learning-based analyses presented in the paper.

---






