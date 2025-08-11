# QML-HEP: Quantum and Classical Machine Learning Methods for High-Energy Physics

## Overview
This repository contains implementations of **quantum** and **classical** machine learning methods applied to **high-energy physics (HEP)** problems.  
It includes work on **graph neural networks (GNNs)**, **equivariant quantum neural networks (QNNs)**, **Kolmogorov–Arnold Networks (KANs)**, and **quantum representation learning**.

## Motivation
Modern HEP experiments generate massive, complex datasets.  
Machine learning via both classical and quantum can help:
- Identify particle signatures (e.g., quark vs. gluon jets)
- Leverage symmetries in detector data via equivariant architectures
- Explore compact function approximations with KANs

These approaches are relevant for **particle physics** and **dark matter searches**, where signal extraction from noisy backgrounds is critical.

## Implementations

### Classical GNN for Quark/Gluon Jet Classification
- Dataset: ParticleNet data (Pythia/Herwig)
- Input: `(pt, rapidity, azimuthal angle, pid)` features per particle
- Evaluation: ROC-AUC, accuracy

### Equivariant Quantum Neural Networks (QNNs)
- Z₂ × Z₂ equivariant models
- Implemented in Qiskit and PennyLane
- Explores symmetry-preserving parameterizations

### Kolmogorov–Arnold Network (KAN)
- Quantum-inspired and classical implementations
- Function approximation in HEP contexts

### Quantum Representation Learning
- Variational quantum circuits for HEP feature extraction

## Repository Structure
.
├── classical-gnn/                     # Classical graph neural network for quark/gluon jet classification
│   ├── gnn_quark_gluon_classification.ipynb
│   └── utils_data_processing.ipynb
│
├── eqv-qnn/                            # Equivariant quantum neural network notebooks
│   └── equivariant_qnn_z2x2.ipynb
│
├── kan/                                # Kolmogorov–Arnold network implementations
│   └── kolmogorov_arnold_network_hep.ipynb
│
├── quantum-repr/                       # Quantum representation learning notebooks
│   └── quantum_representation_learning_hep.ipynb
│
├── requirements.txt                    # Python dependencies
└── README.md                           # Project documentation
