# essential-oil-chemometrics
*   **Description:** Enterprise XAI dashboard and LIMS platform for GC-MS botanical fingerprinting, featuring PCA Biplots, automated PDF CoAs, and Explainable QC.

# 🌿 Executive AI Botanical Fingerprinter & LIMS Platform

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://essential-oil-chemometrics.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)

An executive-tier Explainable AI (XAI) and Laboratory Information Management System (LIMS) engineered for analytical phytochemistry and pharmaceutical QA/QC. Utilizing a schematic layout inspired by executive BI dashboards, this tool automates the multivariate analysis of GCxGC-MS datasets to authenticate botanical origins and automatically generate audit-ready PDF Certificates of Analysis (CoA).

## 💡 Advanced Executive Capabilities
*   **Automated CoA PDF Generation:** Integrates pure-Python PDF rendering (`fpdf2`) to allow QA managers to instantly export localized, formatted Certificates of Analysis detailing batch quality control status and complete terpene profiles for audit archives.
*   **Chemometric Biplot Projections:** Overlays PCA scores and feature loadings simultaneously in an interactive chemical space, allowing senior analysts to visually trace exactly which phytochemical vectors are pulling a given batch out of specification.
*   **Explainable AI (XAI) Root-Cause Analysis:** Resolves "black-box" rejection parameters by synthesizing an automated Waterfall Chart. It computes the exact deviation of a rejected batch against the authentic baseline, weighted by Random Forest feature importance.
*   **Zero-Shot Adulterant Flagging:** Utilizes unsupervised `IsolationForest` anomaly detection to identify structurally abnormal batches without requiring prior training on specific adulterants.
*   **Phytochemical Co-Occurrence Networks:** Employs `NetworkX` graph theory to map secondary metabolite correlations across geographic regions, visualizing natural co-elution clusters.

## 🚀 Deployment Operations

**1. Clone the Repository**
```bash
git clone https://github.com/Arashka-Ch/essential-oil-chemometrics.git
cd essential-oil-chemometrics
```

**2. Provision the Environment**
```bash
mamba create -n chemometrics_env python=3.10 -y
mamba activate chemometrics_env
pip install -r requirements.txt
```

**3. Launch the Application**
```bash
streamlit run app.py
```
