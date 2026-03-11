# Connectivity-Based Organization of the Substantia Nigra
This project reveals a previously unresolved connectivity-based organization of the substantia nigra and shows how distinct subregions contribute differently to motor network dysfunction in Parkinson’s disease.

## Objectives:
- Can diffusion MRI connectivity reveal internal structure of the substantia nigra?
- Do connectivity patterns from SN subregions differ between Parkinson’s disease patients and healthy controls?
- Can connectivity patterns predict clinical motor symptom severity?
- 
## Datasets
- Human Connectome Project (7T diffusion MRI)
- Parkinson’s Progression Markers Initiative

## Methods overview

<img width="1362" height="1602" alt="fig1_methods" src="https://github.com/user-attachments/assets/cbbce08d-8718-4c7b-83d2-23d5c2aba865" />

## Results
### Key Results:
- A **six-cluster connectivity-defined parcellation** of the substantia nigra showed the highest reproducibility and hemispheric stability.
- Connectivity patterns distinguishing clusters were identified using **machine learning and SHAP feature interpretation**.
- Cluster-level connectivity features predicted **clinical motor severity (MDS-UPDRS-III)** in Parkinson’s disease patients.

### Fig.1:
<img width="759" height="640" alt="fig3_results" src="https://github.com/user-attachments/assets/26a8bc8b-c732-4cb7-a936-342d867296ab" />

**Fig. 1:** Identification of a six-cluster substantia nigra parcellation validated using split-half reproducibility and hemispheric stability.

### Fig.2:
<img width="931" height="398" alt="Screenshot 2026-03-10 at 12 22 09" src="https://github.com/user-attachments/assets/0d7f8611-eeb2-47d7-856a-3fab83706646" />

- **B1:** t-SNE dimensionality reduction showed clear separation between connectivity-defined clusters.  
- **B2:** A Random Forest classifier predicted SN cluster identity with high accuracy, indicating strong separability based on connectivity features.  
- **B3:** The most influential cortical and subcortical regions contributing to each cluster are summarized.

### Fig. 3:
<img width="496" height="249" alt="Screenshot 2026-03-10 at 12 36 21" src="https://github.com/user-attachments/assets/83489ed6-a8cd-4c0c-ba05-3c9d5b3ebee6" />

**Fig. 3:** An XGBoost model predicted clinical motor severity (MDS-UPDRS-III) from SN connectivity features. SHAP analysis identified the most influential regions contributing to motor symptom expression. Red ROIs indicate reduced connectivity in PD relative to healthy controls, while blue ROIs indicate increased connectivity.

## Key Takeaway
Connectivity-based diffusion MRI revealed a **reproducible six-region organization of the substantia nigra** and demonstrated how specific connectivity patterns from these subregions relate to motor symptom severity in Parkinson’s disease.

## Clinical Relevance
- Reveals previously unresolved internal organization of the substantia nigra based on whole-brain connectivity.
- Demonstrates that connectivity patterns from specific SN subregions relate to motor symptom severity.
- Suggests that connectivity-based parcellation may support **network-level biomarkers of Parkinson’s disease progression and heterogeneity**.

## Tools 
Analysis and visualisationwas performed using:
- Python
- MATLAB
- FSL
- Inkscape

Processing pipeline of this study is available at: 
https://github.com/neuromti/ATPP_CLI_V2
