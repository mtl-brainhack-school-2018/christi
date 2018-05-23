
# Christina Tremblay #

# Montreal Brainhack school project 2018 #

## Is depression in Parkinson’s disease related to different atrophy and cognitive patterns? ##
### Aims ###

•	The main aim of this project is to investigate the cortical thickness changes after a few years in small subgroups of patients with Parkinson’s disease (PD) with and without depressive symptoms compared to aging healthy control 

•	The second aim is to verify if the cortical changes observed is related to different pattern of cognitive deterioration in PD with and without depression

### Database ### 

The neuroimaging data (structural MRI) come from patients’ subgroups belonging to the Parkinson's Progression Markers Initiative (PPMI), an open access longitudinal database continually updated, containing multiple kind of data (including neuroimaging, neuropsychological and demographical data) from up to 5 years around 35 centers in North America, Europe, Israel, and Australia (http://www.ppmi-info.org/about-ppmi/). The principal goal of the PPMI study is to assess the progression of clinical features, imaging and biologic markers in PD patients (de novo PD, Prodromal and subjects with specific genetic mutations) and healthy controls.

#### *Subgroups used for the brainhack project* ####

•	10 PD patients with depressive symptoms (GDS-Short >5) - PDDS

•	10 PD patients without depressive symptoms (GDS-Short <5) - PD

•	10 Healthy Aging (Control) - HC

### Data preprocessing ###

•	Structural MRI (T1w and/or T2w): from baseline to 4 years

•	For each subject: structural MRI in BIDS format

•	Preprocessed with ANTs longitudinal cortical thickness pipeline (https://github.com/rmarkello/antsct)

•	Cortical thickness and Jacobian map for each subject in each session

### Next steps: quality control and neuroimaging analysis ###

#### *Quality control* ####

•	Visual inspection using Brain Match guidelines to assess the quality of brain registration (https://www.zooniverse.org/projects/simexp/brain-match)

•	Used MRIQC software package for quantitative metrics (https://www.biorxiv.org/content/early/2017/02/24/111294)

#### *Neuroimaging analysis* ####

•	Compare changes (baseline vs 4 years) in cortical thickness (atrophy) between the 3 subgroups (PDD vs PD vs HC)

•	Create thresholded map showing areas of significant difference between PD and HC (and PDD and HC) over 4 years (similar to Fig.1 in https://www.nature.com/articles/s41467-017-02416-0)

	→ [(PD2-PD1)–(HC2-HC1)] and [(PDD2-PDD1)–(HC2-HC1)]

•	Verify the relationship between the atrophy in different regions at baseline (and between the atrophy changes after 4 years) and the behavioral data (cognitive measures) in both PD subgroups

### Specific learning objectives ###

•	Visualizing my data with NeuroVault (https://neurovault.org/)

•	Using environments in Jupiter Notebook

•	Learning more about tools/software useful to do structural MRI group analysis (particularly, statistical comparisons between groups and correlation analysis between MRI and clinical data)
