
# 🧪 tox21-env: Environment Package Summary

This document summarizes the key Python packages used in the Tox21 project and what each one does. It serves as both a reproducibility guide and a personal learning reference.

---

## 🔍 Core Scientific & ML Libraries

| Package         | Purpose |
|-----------------|---------|
| `numpy`         | Fast numerical arrays and linear algebra operations |
| `pandas`        | Tabular data manipulation and CSV/Excel I/O |
| `scikit-learn`  | Classical ML models, metrics (e.g. Random Forest, ROC-AUC) |
| `matplotlib`    | Plotting and data visualization |
| `seaborn`       | Statistical data visualization (optional) |

---

## 🧬 Cheminformatics

| Package         | Purpose |
|-----------------|---------|
| `rdkit`         | Parses SMILES, computes molecular fingerprints (ECFP), draws structures |
| `deepchem`      | Provides datasets (like Tox21), models, and featurizers for ML in chemistry |

---

## 🔥 Machine Learning / Deep Learning

| Package             | Purpose |
|---------------------|---------|
| `torch`             | PyTorch – general-purpose deep learning framework |
| `torch-geometric`   | Graph neural networks (GNNs) for molecular graphs |
| `tensorflow`        | Deep learning backend used by some DeepChem models |
| `lightning`         | Lightweight wrapper around PyTorch for easier training loops |
| `transformers`      | Pre-trained transformer models (e.g., ChemBERTa, SMILES-BERT) |

---

## ⚛️ Optional: Quantum ML & Differentiable Computing

| Package     | Purpose |
|-------------|---------|
| `jax`       | NumPy-compatible library for high-performance computing and auto-differentiation |
| `jaxlib`    | Backend for JAX (needed for execution on CPU or GPU) |

---

Feel free to add new entries here as you expand the environment!
