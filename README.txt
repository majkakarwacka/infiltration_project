Project name: Identification of Immunological Factors Determining the Classification of Melanoma Patients at Increased Risk of Death

Author: Marianna Śmiełowska

Project description:
Using machine learning to analyze immunological factors affecting survival in patients with melanoma.
To support early identification of high-risk melanoma patients through immune profiling, potentially guiding more personalized treatment strategies.

Contents:
Project_MS.ipynb
Data analysis and machine learning pipeline implemented in a Jupyter Notebook to identify key immunological features associated with poor prognosis in melanoma patients.

TCGA_SKCM.csv
Clinical data about melanoma patients.
Data sources: cBioPortal: Cerami et al., 2012 & Gao et al., 2013
Column names:
- Patient ID: Unique identifier for the patient.
- Sample ID: Unique identifier for the tumor sample taken from the patient.
- Diagnosis Age: Age of the patient at the time of cancer diagnosis.
- Neoplasm Disease Stage American Joint Committee on Cancer Code: Overall stage of cancer based on AJCC criteria.
- Aneuploidy Score: Measure of chromosomal abnormalities.
- Buffa Hypoxia Score: Score indicating tumor hypoxia (low oxygen), based on gene expression (Buffa method).
- Fraction Genome Altered: Proportion of the genome with copy number alterations.
- Mutation Count: Total number of somatic mutations detected in the tumor sample.
- Overall Survival (Months): Time (in months) the patient lived after diagnosis or treatment.
- Overall Survival Status: Whether the patient is alive or deceased at last follow-up.
- Other Patient ID: Secondary ID used in related datasets or studies.
- American Joint Committee on Cancer Metastasis Stage Code: Code indicating if the cancer has metastasized.
- American Joint Committee on Cancer Tumor Stage Code: Code indicating the size/extent of the primary tumor.
- Person Neoplasm Cancer Status: Whether the patient currently has evidence of cancer or is in remission.
- Progress Free Survival (Months): Time (in months) the patient lived without disease progression after treatment.
- Progression Free Status: Indicates whether the disease has progressed
- Sex: Biological sex of the patient
- Patient Weight: Weight of the patient at time of sample collection.

TIP_SKCM.csv
Immunological data about infiltration of melanoma tumors.
Data sources: TIP: A Web Server for Resolving Tumor Immunophenotype Profiling. Cancer Research. 2018.
Column names:
- Mixture: Identifier for the sample
- B cells: Abundance of B lymphocytes at tumor site. Involved in antibody production.
- CD4 Naive: Abundance of Naive CD4+ T cells at tumor site. Not yet exposed to antigen; important in initiating immune responses.
- CD4 Memory: Abundance of Memory CD4+ T cells at tumor site. They respond quickly to previously encountered antigens.
- CD8 Naive: Abundance of Naive CD8+ T cells at tumor sites. Cytotoxic precursors not yet activated by antigens.
- CD8 Memory: Abundance of Memory CD8+ T cells at tumor site. Long-lived and ready to attack previously encountered pathogens or tumor cells.
- CD8 Effector: Abundance of Effector CD8+ T cells at tumor site. Actively involved in killing cancer cells.
- Treg cell: Abundance of Regulatory T cells at tumor site. They suppress immune responses — often upregulated in tumors to evade immunity.
- Th cell: Abundance of Helper T cells (CD4+) at tumor site. They coordinate immune responses by activating other immune cells.
- Monocytes CD16: Abundance of monocytes expressing CD16 at tumor site. Involved in inflammation and tissue repair.
- Monocytes CD14: Abundance of monocytes with CD14 expression at tumor site. Typically involved in pathogen detection and immune activation.
- DC (Dendritic Cells): Abundance of DC at tumor site. Antigen-presenting cells that activate T cells and initiate immune responses.
- NK (Natural Killer) cells: Abundance of NK at tumor site. Cytotoxic lymphocytes that can kill tumor cells without prior sensitization.