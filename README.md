# P2SURF
Machine learning framework for predicting the critical micelle concentration (CMC) of single and binary surfactant systems using cheminformatics descriptors and artificial neural networks. Includes interpolation and extrapolation capabilities for surfactant mixtures.

🧠 Project Overview
Surfactants are widely used in pharmaceuticals, personal care, oil recovery, and more. Their performance is governed by critical micelle concentration (CMC)—a key physicochemical property. This project leverages artificial neural networks (ANN) and cheminformatics descriptors to predict CMC for:
Single-component surfactants
Binary surfactant mixtures, including:
  Interpolation across mole fractions in known mixtures
  Extrapolation to completely new surfactant combinations
  
This machine learning framework uses descriptor generation (RDKit, Mordred, PaDEL), feature selection (BorutaPy), and model training/evaluation steps.

📦 Requirements
Install the dependencies using:

  conda env create -f environment.yml
  conda activate cmc-prediction

📁 Datasets
All datasets used in this project are included in the dataset folders of each case. These datasets contain:
> SMILES strings
> Experimental CMC values

🚀 How to Run
You can open and run each notebook step-by-step inside any of the following folders:
> Single_Surfactant_CMC
> Mixture_surfactants_CMC/Case-1_Interpolating CMC at intermediate mole fraction
> Mixture_surfactants_CMC/Case-2_Predicting CMC for unseen surfactant mixtures
