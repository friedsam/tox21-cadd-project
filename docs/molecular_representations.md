
# 🧬 Molecular Representations in Drug Discovery

This reference summarizes common ways to represent molecules in machine learning and cheminformatics. Each representation type is suited to different modeling goals.

---

## 🔠 Categories of Molecular Representations

| Type                      | Examples                      | Used For                           |
|---------------------------|-------------------------------|-------------------------------------|
| **Fingerprints**          | ECFP (Morgan), MACCS, Avalon  | Classical ML, fast screening        |
| **SMILES strings**        | `"CC(=O)OC1=CC=CC=C1C(=O)O"`   | Text-based models, transformers     |
| **Graphs**                | Nodes = atoms, edges = bonds  | GNNs (graph-based deep learning)    |
| **3D Structures**         | XYZ coordinates, conformers   | Docking, quantum chemistry          |
| **Descriptors (numeric)** | logP, MW, TPSA, H-bond counts | QSAR, interpretable ML              |
| **SELFIES**               | String format alternative to SMILES | Safer for generative models     |
| **Coulomb matrices**      | Atomic charges + distance info | Quantum ML (e.g., energy prediction)|

---

## 🔍 Comparison of Common Representations

### 🧬 Fingerprints (e.g., ECFP)
- Binary vectors based on molecular substructures
- Pros: Fast, simple, well-supported
- Cons: Opaque, no spatial or global context

### 🔗 SMILES / SELFIES
- Text-based formats of chemical structure
- Pros: Compact, widely used, easy to generate
- Cons: Not structure-aware, fragile (SMILES), harder to model directly

### 🧠 Graphs
- Molecule as a graph: atoms = nodes, bonds = edges
- Pros: Preserves structural information, ideal for GNNs
- Cons: More complex to build and process

### ⚛️ 3D Coordinates
- Precise atom positions in space
- Pros: Required for docking, simulations, and QML
- Cons: Sensitive to conformers, not always available

### 📊 Descriptors
- Precomputed physical or chemical properties
- Pros: Interpretable, quick to compute
- Cons: May miss complex patterns

---

## 📦 Summary

Choose the representation based on:
- Available data (SMILES, structures, etc.)
- Modeling goals (screening, generation, simulation)
- ML methods in use (RF vs GNN vs QML)

It's often useful to try **multiple representations** and compare performance.

