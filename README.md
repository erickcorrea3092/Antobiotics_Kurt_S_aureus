# Antobiotics_Kurt_S_aureus
This code is about a QSAR model development for the prediction of the antimicrobial activity against Staphyloccous aureus.

QSAR Modeling for Antibiotic Activity Against Staphylococcus aureus

📌 Description

This repository contains the dataset, computational scripts, and Machine Learning models developed to predict antibacterial activity ($\text{pIC}_{50}$ / $\text{MIC}$) against Staphylococcus aureus.Using quantitative structure-activity relationship (QSAR) methodologies and molecular descriptors calculated from chemical structures (SMILES), this project aims to support the rational design and virtual screening of novel therapeutic candidates to combat bacterial resistance.

The recopilation of the data is in the excel archive .xlsx type called data.xlsx and Actividad.xlsx, and in the first script 1_kurt_similitud.ipynb is posible to see wich molecules are avalaible for the construction of the model, were organized by Butina-Taylor Clustering, and a similarity matrix were constructed.


<img width="1500" height="700" alt="newplot (81)" src="https://github.com/user-attachments/assets/5b2ca648-457a-418d-bfa7-edd08f8d827c" />



<img width="2100" height="1050" alt="image" src="https://github.com/user-attachments/assets/a410074b-f03f-405e-b438-b80ba6db847f" />


<img width="1000" height="800" alt="newplot (82)" src="https://github.com/user-attachments/assets/889d2f96-d1b3-4832-b389-4f5f4ee1672c" />


With this information is posible the construction of a model QSAR. first, we calculate molcular descriptors using mordred library. we dont show the exctly script but we left a script where can ilustrate the code for the obtention of molecular descriptors. Anyway the excel type archive is ActividadV.xlsx and the archive with the endpoint pMIC realated is in ActividadV.xlsx.

the scripts 2 and 3 show the construction fo the model, the script 2 is a simple construction of the QSAR model, the main function is known how make the splittin of the train an test group, the construction of a pipeline, how many descriptors use, what regressor model use and its hyperparameters, etc, while the third script was created for understand how is the data bahaivor along the pipeline executation. 

In forth script is defined also the Aplication Domain by leverage method, and in this, we can make the predictions of our molecules that we want to investigate, that group is called xplor group, the chemical space is defined by the Lipinski criteria and three represenattions were made: Principal Component Analisis PCA, T-distributed Stochastic Neighbor Embedding (tSNE) and UMAP (Uniform Manifold Approximation and Projection).

An databased published by DIFAQUIM research group in UNAM were evaluated for the search of new estructures with antimicrobial activity, a molecules called Aristoloxacin A were predicted his activity with a vey little diference that aloow us to the percibe the predectivie power of our model.


The methodological WorkflowData of the model is below: 

Curation & Preprocessing:Curation of bioactive compounds tested against Staphylococcus aureus.
Standardization of chemical structures (removal of salts, neutralization, tautomer evaluation).

Feature Extraction:Calculation of 2D/3D molecular descriptors and Morgan Fingerprints (ECFP4/6) using RDKit/py3Dmol.

Model Building & Validation:Implementation of Machine Learning algorithms (e.g., Random Forest, XGBoost, Support Vector Machines).Evaluation through internal validation (Cross-Validation, $R^2$, $Q^2$, RMSE) and domain of applicability analysis.
