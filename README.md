# 🧬 Biomarker Identification for NSCLC using Multi-Omics and Explainable AI

## 🔍 Project Overview

A **biomarker** is a measurable indicator of a biological state or condition that provides vital insights into disease processes. Biomarkers play a critical role in clinical research, prognosis, diagnosis, and therapeutic development. With the advent of **multi-omics integration**, the discovery of biomarkers can be enhanced through a comprehensive view of complex biological systems and disease mechanisms.

This research project focuses on **Lung Cancer** and employs **multi-omics data** and **machine learning (ML)** with **Explainable Artificial Intelligence (XAI)** techniques to uncover target biomarkers responsible for **non-small cell lung cancer (NSCLC)**. The outcome of this analysis can potentially assist researchers in identifying drug targets for personalized treatment.

---

## 📊 Objectives

- Integrate and preprocess **multi-omics datasets** (RNA-Seq, methylation, CNA, protein arrays, and clinical data) from **TCGA-LUAD** and **TCGA-LUSC**.
- Develop ML models to classify NSCLC subtypes (LUAD and LUSC).
- Apply XAI methods (SHAP, LIME) to interpret model predictions and feature importance.
- Identify critical genes, hub proteins, and pathways through **PPI networks** and **KEGG pathway enrichment**.
- Build a survival prediction model using **Cox regression** and evaluate with Kaplan-Meier plots.

---

## 🧪 Methodology

### 1. **Data Collection & Preprocessing**
- Downloaded and assembled RNA-Seq, DNA-CNA, and protein array data from **TCGA**.
- Cleaned, normalized, and integrated the datasets for downstream analysis.

### 2. **Modeling and Classification**
- Trained **Multi-Layer Perceptron (MLP)** and **Logistic Regression** models on RNA-Seq and DNA+CNA data.
- Classified tumor samples into LUAD and LUSC subtypes.
- Evaluated performance using accuracy, precision, recall, and F1-score metrics.

### 3. **Model Explainability with XAI**
- Implemented **SHAP (SHapley Additive exPlanations)** and **LIME (Local Interpretable Model-Agnostic Explanations)** to understand key biomarkers influencing the predictions.
- Interpreted gene features related to:
  - Tumor microenvironment
  - Cell cycle regulation
  - Immune system modulation

### 4. **Biological Analysis**
- Conducted **Protein-Protein Interaction (PPI)** network analysis to identify **hub proteins**.
- Applied **KEGG pathway enrichment** to uncover significant biological pathways.
- Filtered top differentially expressed genes/proteins for potential therapeutic targets.

### 5. **Survival Prediction**
- Developed **Cox Proportional Hazards Regression** models for survival analysis.
- Used **Kaplan-Meier curves** and **Kernel Density Estimations (KDE)** to visualize survival probability by subtype.
- Assessed risk stratification of patients based on biomarker expression.

---

## 🛠️ Technologies Used

- **Languages**: Python
- **Libraries**: 
  - `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
  - `lifelines` (Cox Regression, Kaplan-Meier)
  - `shap`, `lime` (XAI)
  - `networkx`, `BioPython` (PPI analysis)
- **Datasets**: TCGA-LUAD, TCGA-LUSC (via GDC Portal)


---

## 📈 Results

- Achieved successful classification of LUAD and LUSC subtypes using RNA-Seq and CNA data.
- XAI techniques revealed interpretable and biologically relevant biomarkers.
- PPI and KEGG pathway analysis pinpointed actionable targets and key cancer-related mechanisms.
- Survival prediction models exhibited strong subtype-specific risk separation.
---

## 🧾 Citation
-[https://doi.org/10.1158/0008-5472.CAN-07-0003]
## Dataset 
-[https://www.cbioportal.org/study/summary?id=luad_tcga_pan_can_atlas_2018] <br/>
-[https://www.cbioportal.org/study/summary?id=lusc_tcga_pan_can_atlas_2018]



