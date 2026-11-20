# ARL 9900 XRF Predictive Maintenance & Anomaly Detection

**Program:** DeepTech_Ready x WESOnline Mentorship Program (Cohort 4)
**Author:** Muhammad Maccido Aminu
**Mentor:** Mr. Idris Aliyu
**Host Site:** Dangote Cement Plc, Obajana (Automation & QCX)

## Overview
This project is the final capstone submission for the DeepTech_Ready x WESOnline Mentorship Program. It builds a Machine Learning pipeline to detect instrument drift and mechanical degradation in the ARL 9900 XRF Workstations at Dangote Cement Plc (Obajana). 

## The Problem
The OXSAS software does not natively export historical alarm logs or sensor status to a clean CSV format. Maintenance is currently reactive, leading to unplanned downtime for the 4 ARL machines.

## The Solution
Using custom Python parsing, this project extracts chemical analysis data (Clinker CaO percentages) from raw OXSAS CSV exports. It then applies an **Isolation Forest** (Unsupervised Machine Learning) algorithm to detect anomalies in the chemical readings. By merging this with simulated sensor parameters (Vacuum Pump Time), the model successfully flags potential machine failures before they cause a "Fatal Error."

## View the Project
*   **Python Code:** Open `XRF_Drift_Analysi.ipynb` (requires Jupyter Notebook)
*   **Static Report:** Open `XRF_Drift_Analysi.html` (view directly in your browser)

## Technologies Used
*   **Language:** Python 3
*   **Libraries:** Pandas, Scikit-Learn, Matplotlib, Seaborn
*   **Tools:** Jupyter Notebook, Git
