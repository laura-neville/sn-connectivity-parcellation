# Substantia Nigra Connectivity Parcellation
This project used diffusion MRI connectivity patterns to characterize the internal organization of the substantia nigra, a midbrain structure critically involved in Parkinson’s disease. Data-driven clustering of connectivity profiles was used to identify distinct connectivity-defined subregions and evaluate their relationship with disease-related network changes.

## Objectives:
- Can diffusion MRI connectivity reveal internal structure of the substantia nigra?
- Do connectivity patterns differ between Parkinson's disease patients and healthy controls?

## Datasets
- Human Connectome Project (7T diffusion MRI)
- Parkinson’s Progression Markers Initiative

## Methods overview

<img width="1362" height="1602" alt="fig1_methods" src="https://github.com/user-attachments/assets/cbbce08d-8718-4c7b-83d2-23d5c2aba865" />

## Results
### Key Results:
- A 6-cluster parcellation of the SN showed the highest reproducibility and stability across hemispheres
- The most distinguishing features driving SN cluster assignments were revealed with SHAP analysis
- Clinical motor severity scores were predicted using subject-level connectivity from each previously defined cluster

### Fig.1:
<img width="759" height="640" alt="fig3_results" src="https://github.com/user-attachments/assets/26a8bc8b-c732-4cb7-a936-342d867296ab" />

Identification of 6-cluster SN parcellation, validated by split-half reproducibility and hemispheric stability.

### Fig.2:
<img width="931" height="398" alt="Screenshot 2026-03-10 at 12 22 09" src="https://github.com/user-attachments/assets/0d7f8611-eeb2-47d7-856a-3fab83706646" />


- **B1:** t-SNE dimensionality reduction showed clear separation between connectivity-defined clusters.  
- **B2:** A Random Forest classifier predicted SN cluster identity with high accuracy, indicating strong separability based on connectivity features.  
- **B3:** The most influential cortical and subcortical regions contributing to each cluster are summarized.

### Fig. 3:
<img width="496" height="249" alt="Screenshot 2026-03-10 at 12 36 21" src="https://github.com/user-attachments/assets/83489ed6-a8cd-4c0c-ba05-3c9d5b3ebee6" />

An XGBoost machine learning model was trained to predict clinical motor severity scores (MDS-UPDRS-III). SHAP analysis was used to interpret the features most predictive of motor symptom expression. Red ROIs indicate hypoconnectivity in PD patients compared to healthy controls; blue ROIs indicate hyperconnectivity. 

## Key Takeaway
Connectivity-based analysis revealed a reproducible six-region organization within the substantia nigra and demonstrated how specific connectivity patterns relate to motor symptom severity in Parkinson’s disease.

## Tools and Methods
Analysis was performed using:
- Python
- MATLAB
- FSL

Processing pipeline of this study is available at: 
https://github.com/neuromti/ATPP_CLI_V2
