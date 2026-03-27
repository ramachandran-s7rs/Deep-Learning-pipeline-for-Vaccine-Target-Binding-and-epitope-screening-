# Deep-Learning-pipeline-for-Vaccine-Target-Binding-and-epitope-screening-
Deep Learning pipeline (DeepPurpose) for vaccine development. Quantify binding affinity (pKd), thermodynamic stability (ΔG), and potency (IC50) for protein-protein interactions. Features automated epitope screening via sliding-window analysis to identify high-affinity binding regions.


# In Silico Evaluation of Vaccine Constructs using Deep Learning

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python: 3.12+](https://img.shields.io/badge/Python-3.12%2B-blue)
![Framework: DeepPurpose](https://img.shields.io/badge/Framework-DeepPurpose-green)

## 📌 Project Overview
This repository contains a specialized Deep Learning pipeline designed to evaluate the binding affinity of **large  vaccine constructs**  against specific therapeutic targets.

The pipeline utilizes the **DeepPurpose** framework to perform Protein-Protein Interaction (PPI) predictions. By calculating biochemical metrics like **pKd**, **Gibbs Free Energy ($\Delta G$)**, and **IC50**, this project provides a computational "proof-of-concept" for vaccine efficacy, safety, and specificity before moving to *in vitro* laboratory testing.

## 🧪 Key Functionalities
* **Global Affinity Prediction:** Evaluates the structural fit of the full-length vaccine sequence.
* **Epitope Mapping (Sliding Window):** Scans the sequence for "hotspots" to identify the most active 30-AA binding regions.
* **Thermodynamic Modeling:** Automates the calculation of $\Delta G$ (kcal/mol) and molar dissociation constants ($K_d$).
* **Specificity & Control Testing:** Framework for benchmarking candidates against negative controls (e.g., Human Serum Albumin) to ensure low off-target binding.

## 🚀 Getting Started

### 1. Environment Setup (Google Colab Recommended)
DeepPurpose requires specific library versions to maintain compatibility with chemical informatics tools. Run the following in your terminal or a notebook cell:

```bash
# Install core bioinformatics tools
pip install rdkit PyTDC subword-nmt lifelines pandas-flavor wget
pip install git+[https://github.com/bp-kelley/descriptastorus](https://github.com/bp-kelley/descriptastorus)
pip install scikit-learn==1.2.2



DeepPurpose: Huang, K., Fu, T., Glass, L. M., Zitnik, M., & Sun, J. (2020). DeepPurpose: a deep learning library for drug-target interaction prediction. Bioinformatics, 36(17), 4606-4614.

BindingDB: Gilson, M. K., et al. (2016). BindingDB in 2015: A public database for protein-ligand binding affinities, predictive modeling and drug design. Nucleic Acids Research, 44(D1), D1045-D1053.
# Install DeepPurpose Framework
pip install git+[https://github.com/kexinhuang12345/DeepPurpose.git](https://github.com/kexinhuang12345/DeepPurpose.git) --no-deps
