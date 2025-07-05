🧪 P2SURF: Machine Learning Framework for Predicting Critical Micelle Concentration (CMC)
P2SURF is a machine learning framework for predicting the critical micelle concentration (CMC) of both single and binary surfactant systems. It leverages cheminformatics descriptors and artificial neural networks (ANNs) to deliver robust prediction capabilities, including both interpolation across known compositions and extrapolation to novel mixtures.

🧠 Project Overview
Surfactants are essential in a wide range of applications, such as:

Pharmaceuticals

Personal care products

Enhanced oil recovery

Firefighting foams

Environmental remediation

Their performance depends on the CMC, a key physicochemical property. This project applies machine learning to predict CMC directly from molecular structure.

Framework features:

Single-component surfactant CMC prediction

Binary surfactant mixture CMC prediction, including:

Interpolation at untested mole fractions within known mixtures

Extrapolation to entirely novel surfactant combinations

Workflow includes:

Molecular descriptor generation (RDKit, Mordred, PaDEL)

Feature selection with BorutaPy

Model training and evaluation using ANNs

📦 Requirements
To set up the environment, run:

bash
conda env create -f environment.yml
conda activate CMC_Prediction
📁 Repository Structure
text
├── Single_Surfactant_CMC/
│
├── Mixture_surfactants/
│   ├── Case-1_Interpolating CMC at intermediate mole fraction/
│   │
│   └── Case-2_Predicting CMC for unseen surfactant mixtures/
│
├── environment.yml
└── README.md
📁 Datasets
All datasets used in this project are included in the dataset folders for each case. These datasets contain:

SMILES strings

Experimental CMC values

🚀 How to Run
Open and run each notebook step-by-step in Jupyter Notebook or JupyterLab within any of the folders listed above.
