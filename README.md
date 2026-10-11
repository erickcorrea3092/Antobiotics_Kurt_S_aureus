# Antobiotics_Kurt_S_aureus
This code is about a QSAR model development for the prediction of the antimicrobial activity against Staphyloccous aureus.

QSAR Modeling for Antibiotic Activity Against Staphylococcus aureus

📌 DescriptionThis repository contains the dataset, computational scripts, and Machine Learning models developed to predict antibacterial activity ($\text{pIC}_{50}$ / $\text{MIC}$) against Staphylococcus aureus.Using quantitative structure-activity relationship (QSAR) methodologies and molecular descriptors calculated from chemical structures (SMILES), this project aims to support the rational design and virtual screening of novel therapeutic candidates to combat bacterial resistance.
The recopilation of the data is in the excel archive .xlsx type called 





<img width="2100" height="1050" alt="image" src="https://github.com/user-attachments/assets/a410074b-f03f-405e-b438-b80ba6db847f" />







Methodological WorkflowData 

Curation & Preprocessing:Curation of bioactive compounds tested against Staphylococcus aureus.
Standardization of chemical structures (removal of salts, neutralization, tautomer evaluation).

Feature Extraction:Calculation of 2D/3D molecular descriptors and Morgan Fingerprints (ECFP4/6) using RDKit/py3Dmol.

Model Building & Validation:Implementation of Machine Learning algorithms (e.g., Random Forest, XGBoost, Support Vector Machines).Evaluation through internal validation (Cross-Validation, $R^2$, $Q^2$, RMSE) and domain of applicability analysis.
