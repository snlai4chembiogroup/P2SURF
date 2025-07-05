# 🧪 P2SURF: Machine Learning Framework for Predicting Critical Micelle Concentration (CMC)

**P2SURF** is a machine learning-based framework for predicting the **critical micelle concentration (CMC)** of both single and binary surfactant systems. It leverages **cheminformatics descriptors** and **artificial neural networks (ANNs)** to deliver robust prediction capabilities—including both **interpolation** across known compositions and **extrapolation** to novel mixtures.

---

## 🧠 Project Overview

Surfactants are key components in a wide range of applications, including:

- Pharmaceuticals  
- Personal care products  
- Enhanced oil recovery  
- Firefighting foams  
- Environmental remediation  

Their performance hinges on the **CMC**, a key physicochemical property. This project applies machine learning to predict CMC using molecular structure alone.

The framework covers:
- ✅ Prediction of **single-component surfactant** CMCs  
- ✅ Prediction of **binary surfactant mixture** CMCs, including:
  - **Interpolation** at untested mole fractions within known mixtures  
  - **Extrapolation** to entirely novel surfactant combinations  

The workflow integrates:
- Molecular descriptor generation (`RDKit`, `Mordred`, `PaDEL`)
- Feature selection using `BorutaPy`
- Model training and evaluation via ANNs

---

## 📦 Requirements

To set up the environment, run:

```bash
conda env create -f environment.yml
conda activate CMC_Prediction
```

---

## 📁 Repository Structure
```
P2SURF/
├── Single_Surfactant_CMC/
│
├── Mixture_surfactants/
│ ├── Case-1_Interpolating CMC at intermediate mole fraction/
│ │
│ └── Case-2_Predicting CMC for unseen surfactant mixtures/
│
├── environment.yml
└── README.md
```

---

## 📁 Datasets

All datasets used in this project are included in the `dataset` folders within each case directory. These datasets contain:

- SMILES strings
- Experimental CMC values

---

## 🚀 How to Run

Open and run each notebook step-by-step using **Jupyter Notebook** or **JupyterLab** in any of the following folders:

- `Single_Surfactant_CMC/`
- `Mixture_surfactants/Case-1_Interpolating CMC at intermediate mole fraction/`
- `Mixture_surfactants/Case-2_Predicting CMC for unseen surfactant mixtures/`
