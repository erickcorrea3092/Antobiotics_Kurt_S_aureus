# Antobiotics_Kurt_S_aureus
This code is about a QSAR model development for the prediction of the antimicrobial activity against Staphyloccous aureus.

QSAR Modeling for Antibiotic Activity Against Staphylococcus aureus

this work was a merit for a thesis and the obtention of B. Sc. degree in UNAM in Mexico City.
📝 Citation & Credits
Research Group / Supervised by: Dr. Erick Correa Padilla

Thesis / Contributor: Cristopher Carlos Verde Pérez

📌 Description

This repository contains the dataset, computational scripts, and Machine Learning models developed to predict antibacterial activity ($\text{pIC}_{50}$ / $\text{MIC}$) against Staphylococcus aureus.Using quantitative structure-activity relationship (QSAR) methodologies and molecular descriptors calculated from chemical structures (SMILES), this project aims to support the rational design and virtual screening of novel therapeutic candidates to combat bacterial resistance.

The recopilation of the data is in the excel archive .xlsx type called data.xlsx and Actividad.xlsx, and in the first script 1_kurt_similitud.ipynb is posible to see wich molecules are avalaible for the construction of the model, were organized by Butina-Taylor Clustering, and a similarity matrix were constructed.


<img width="1500" height="700" alt="newplot (81)" src="https://github.com/user-attachments/assets/5b2ca648-457a-418d-bfa7-edd08f8d827c" />



<img width="2100" height="1050" alt="image" src="https://github.com/user-attachments/assets/a410074b-f03f-405e-b438-b80ba6db847f" />


<img width="1000" height="800" alt="newplot (82)" src="https://github.com/user-attachments/assets/889d2f96-d1b3-4832-b389-4f5f4ee1672c" />


With this information is posible the construction of a model QSAR. first, we calculate molcular descriptors using mordred library. we dont show the exctly script but we left a script where can ilustrate the code for the obtention of molecular descriptors. Anyway the excel type archive is ActividadV.xlsx and the archive with the endpoint pMIC realated is in ActividadV.xlsx.

The scripts 2_kurt_búsqueda.ipynb and 3_Resumen_Kurt.ipynb show the construction fo the model, the script 2_kurt_búsqueda.ipynb is a simple construction of the QSAR model, the main function is known how make the splittin of the train an test group, the construction of a pipeline, how many descriptors use, what regressor model use and its hyperparameters, etc, while the third script was created for understand how is the data bahaivor along the pipeline executation. 

In forth script 4_Kurt__final.ipynb is defined also the Aplication Domain by leverage method, and in this, we can make the predictions of our new molecules that we want to investigate, that group is called 'xplor' group, add, the chemical space is defined by the Lipinski criteria and three represenattions of chemical space were made: Principal Component Analisis PCA, T-distributed Stochastic Neighbor Embedding (tSNE) and UMAP (Uniform Manifold Approximation and Projection).


<img width="1280" height="720" alt="Platica_Andrés_1 pptx (2)" src="https://github.com/user-attachments/assets/773e4118-9d9c-446d-9361-3daf55ef2c07" />


<img width="1280" height="720" alt="Platica_Andrés_1 pptx (3)" src="https://github.com/user-attachments/assets/7fae3891-616c-43f3-a21f-9555f7a02e35" />




An databased published by DIFAQUIM research group in UNAM were evaluated for the search of new estructures with antimicrobial activity, a molecules called Aristoloxacin A were predicted his activity with a vey little diference that aloow us to the percibe the predectivie power of our model.

<img width="1280" height="720" alt="Platica_Andrés_1 pptx (4)" src="https://github.com/user-attachments/assets/8afb1e09-b225-4279-9b6f-ef63bf928d23" />


<img width="1280" height="720" alt="Platica_Andrés_1 pptx" src="https://github.com/user-attachments/assets/249e5ff1-1eef-42b3-bf08-cb0f196cfcc9" />


<img width="1280" height="720" alt="Platica_Andrés_1 pptx (1)" src="https://github.com/user-attachments/assets/eca3b97d-1ac5-435e-83eb-1e305e37e1ac" />


