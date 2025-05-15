# 🧬 Quantum Machine Learning Demo on Tox21 (Binary Task)

This notebook demonstrates a minimal QML pipeline using a subset of the Tox21 dataset.
We use a binary classification setup (toxic vs non-toxic for one task) and apply a quantum kernel method using `PennyLane`.

---

## What it does:
- Loads Tox21 and selects a single binary task (e.g., NR-AR)
- Reduces data size for quick training and simulation
- Uses a simple quantum feature map and kernel-based classifier

**Note:** Requires `pennylane`, `scikit-learn`, `matplotlib`, and `deepchem`.