# Hospital Efficiency & Clinical Outcomes: Analysis of Heart Failure Lethality in Brazil (2024)
## 🩺 Clinical Context
In Brazil, Heart Failure (HF) is a leading cause of hospitalization and a major public health burden. While treatment protocols are well-established, in-hospital lethality remains a proxy for healthcare quality and system efficiency. This project evaluates the Hospital Lethality Rate—the ratio between hospital deaths and total admissions—across all Brazilian states in 2024, identifying where the system fails to save patients once they are admitted.

## 📊 Key Analytical Insights
 The Lethality Leaders: A critical efficiency gap was identified in Alagoas (3.26%) and Rio de Janeiro (3.01%), which recorded the highest mean lethality rates in the country. This indicates a severe disparity in clinical outcomes compared to the national average.
The RJ vs. SP Paradox: Despite similar urban complexities, Rio de Janeiro consistently underperformed São Paulo every month of 2024. Since lethality is a percentage-based metric, this suggests that RJ's higher mortality is driven by system inefficiency (e.g., late-stage admissions or resource management) rather than mere population volume.
Data Integrity & Underreporting: Significant outliers were detected in states like Espírito Santo, where near-zero lethality in specific months suggests potential underreporting or delays in the SIH/SUS database, highlighting a challenge for real-time epidemiological surveillance.

## 🛠️ Technologies & Methodology
Language: Python 3.x
Data Libraries: * Pandas: Cleaning and processing administrative datasets, handling Brazilian-specific numerical formatting (thousands separators), and feature engineering (Lethality Coefficient calculation).
Matplotlib: Time-series visualization and comparative analysis of state-level performance.
Methodology: Calculation of monthly lethality coefficients
(Deaths/Admissions)∗100
and weighted annual means to identify geographic "hotspots" of hospital mortality.

## 📁 Data Source
The raw data was extracted from TABNET/DATASUS (Brazilian Ministry of Health), specifically from the Hospital Information System (SIH/SUS). The analysis includes:
Total hospital admissions for Heart Failure (IC) per state.
Total in-hospital deaths for Heart Failure (IC) per state.
Monthly data coverage from January to December 2024.
