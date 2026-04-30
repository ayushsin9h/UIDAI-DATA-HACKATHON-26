# 🇮🇳 Lifecycle-Aware Aadhaar Intelligence Framework (LAIF)

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Data: Kaggle](https://img.shields.io/badge/Data-Kaggle-blue)](https://www.kaggle.com/)

> **Developed for the UIDAI Data Hackathon 2026**, this project introduces a predictive, data-driven framework to transform Aadhaar from a static identity program into a dynamic, lifecycle-based service. **LAIF** enables the UIDAI to anticipate update demands, optimize center capacity, and proactively respond to societal shifts.

---

## 👥 Team Information: UIDAI_7380
* **Team Lead**: Ayush Singh
* **Institution**: Guru Nanak Institute of Technology (GNIT), Kolkata

---

## 📌 Problem Statement
The current Aadhaar update system is largely reactive, leading to predictable overcrowding at centers during specific months (e.g., March and July). Resources are often unevenly distributed across states, and enrollment/update cycles lack a planned, anticipatory approach.

---

## 📥 Data Setup (Kaggle)
Due to GitHub's file size constraints (100MB limit), the raw and processed Aadhaar datasets are hosted externally to maintain Git history integrity.

1. Download the dataset from Kaggle: **https://www.kaggle.com/datasets/ayushs1ngh/uidai-2026-data-hackathon/**
2. Extract the downloaded `.zip` file.
3. Place the extracted `raw/` and `processed/` folders directly into the `data/` directory of this repository.

---

## 💡 Proposed Solution: LAIF
Instead of merely tracking historical volumes, LAIF asks: **"WHO updated WHAT, WHY, and WHEN—and what will happen NEXT?"**

### Key Strategic Pillars
1. **Lifecycle Segmentation**: Categorizes behavior by age (0-5: Enrollment; 5 & 15: Mandatory Biometric Updates; 17+: Demographic corrections).
2. **Temporal Demand Forecasting**: Links update spikes to real-world triggers like fiscal deadlines in March and school admissions in September.
3. **Operational Efficiency Index**: Introduces *"Average Entries per Center per Day"* as a National KPI to identify and manage overloaded regional hotspots.

---

## 🛠️ Tech Stack & Methodology
* **Language**: Python (Pandas, NumPy, Pathlib)
* **Visualization**: Power BI, Matplotlib
* **Data Cleaning**: Standardized inconsistent date formats and rigorously validated 766+ districts against official government references.
* **Scope**: Analyzed massive-scale enrollment, biometric, and demographic datasets from March to December 2025.

---

## 📂 Repository Structure (MLOps Standard)
```text
UIDAI-DATA-HACKATHON-26/
├── dashboards/                  # Power BI dashboard for trend analysis
│   └── data_visualization.pbix
├── data/                        # Hosted externally on Kaggle (See Data Setup)
│   ├── processed/               # Cleaned & merged output CSVs
│   └── raw/                     # Immutable original datasets
├── docs/                        # Presentations and analytical reports
│   └── data_cleaning_insights_report.xlsx
├── notebooks/                   # Jupyter notebooks for EDA
│   └── biometric_demographic_analysis.ipynb
├── src/                         # Production Python scripts
│   ├── __init__.py
│   ├── biometric/
│   │   ├── cleaning_3_states_biometric.py
│   │   ├── cleaning_4_districts_biometric.py
│   │   └── implementation_5_biometric_merging.py
│   ├── demography/
│   │   ├── cleaning_5_states_demography.py
│   │   ├── cleaning_6_districts_demography.py
│   │   └── implementation_6_demography_merging.py
│   └── enrolment/
│       ├── cleaning_1_states_enrolment.py
│       ├── cleaning_2_districts_enrolment.py
│       └── implementation_4_enrolment_merging.py
├── .gitignore                   # Ignores large data files and system caches
├── LICENSE                      # MIT License
├── README.md                    # Project documentation
└── requirements.txt             # Python dependencies
