# Lifecycle-Aware Aadhaar Intelligence Framework (LAIF)

Developed for the **UIDAI Data Hackathon 2026**, this project introduces a predictive, data-driven framework to transform Aadhaar from a static identity program into a dynamic, lifecycle-based service. **LAIF** enables the UIDAI to anticipate update demands, optimize center capacity, and proactively respond to societal shifts.

---

## 👥 Team Information: UIDAI_7380
* **Team Lead**: Ayush Singh
* **Institution**: Guru Nanak Institute of Technology (GNIT), Kolkata

---

## 📌 Problem Statement
The current system is largely reactive, leading to predictable overcrowding at centers during specific months like March and July. Resources are often unevenly distributed across states, and enrollment/update cycles lack a planned approach.

---

## 💡 Proposed Solution: LAIF
Instead of tracking historical volumes, LAIF asks: **"WHO updated WHAT, WHY, and WHEN—and what will happen NEXT?"**

### Key Strategic Pillars
1.  **Lifecycle Segmentation**: Categorizes behavior by age (0-5: Enrollment; 5 & 15: Mandatory Biometric Updates; 17+: Demographic corrections).
2.  **Temporal Demand Forecasting**: Links update spikes to real-world triggers like fiscal deadlines in March and school admissions in September.
3.  **Operational Efficiency Index**: Introduces "Average Entries per Center per Day" as a National KPI to identify and manage overloaded hotspots.

---

## 🛠️ Tech Stack & Methodology
* **Language**: Python (Pandas, NumPy)
* **Visualization**: Power BI, Matplotlib
* **Data Cleaning**: Standardized inconsistent date formats and validated 766+ districts against official government references.
* **Datasets**: Analyzed enrollment, biometric, and demographic datasets from March-December 2025.

---

## 📂 Repository Structure
```text
UIDAI-DATATHON-2026/
├── Biometric/                      # Raw and processed biometric datasets
├── Demography/                     # Raw and processed demographic datasets
├── Enrolment/                      # Raw and processed enrolment datasets
├── DATA VISUALIZATION.pbix          # Power BI dashboard for trend analysis
├── Data Cleaning Insights Report.xlsx # Metrics on data preprocessing results
└── biometric_demographic_analysis.ipynb # Main Python script for data analysis
