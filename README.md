
# ECG→ASD Features  
**Robust Estimation of Inter-beat Interval Skewness for Autonomic Dysregulation Assessment in Noisy Neonates ECG**

Talithea Concepción · University of South Carolina  
Advisors: Dr. Christian O’Reilly & Dr. Jessica Bradshaw  

---

## 📘 Overview
This repository contains the full analysis pipeline for extracting **ECG-derived features** such as skewness and entropy from neonatal ECG recordings.  
The goal is to evaluate how **inter-beat interval (IBI) skewness** varies with window length and noise level, validating it as a potential biomarker for **autonomic dysregulation and early ASD detection**.

---

## 🧠 Research Context
Neonatal ECG signals are often **short and noisy**, limiting traditional long-segment analyses.  
By computing skewness and entropy over multiple smaller segments and applying bootstrapping, this project:
- Quantifies **stability vs. window size** (1–5 minutes)  
- Measures bias introduced by segment length  
- Produces reproducible KDE and variance plots  

---

## 🧩 Repository Structure

src/ecgasd/ # Core feature extraction and signal utilities
├─ notebooks/ # Analysis notebooks 
├─ configs/ # YAML configuration files
├─ docs/ # Figures, HTML exports, and TSV outputs
├─ scripts/ # Reproducibility and automation scripts
├─ tests/ # Unit tests
├─ data/ # (git-ignored) Raw / interim ECG data
└─ environment.yml # Reproducible environment definition
