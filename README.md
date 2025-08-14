# 📊 Cancer Survival Analysis

## 📝 Project Overview
This repository contains a complete survival analysis workflow implemented in **R**, **Python**, and **SAS**.  
All three implementations perform the same analytical steps for full reproducibility.

The workflow includes:
- Data import & cleaning
- Kaplan–Meier survival curves
- Cox proportional hazards regression (univariable & multivariable)
- Stratified analysis by Intervention × Gender and Age Groups
- Forest plots for hazard ratios
- Median survival estimation
- Baseline descriptive statistics & hypothesis tests

---

## 📂 Dataset
**Variables:**
- `time` — Survival time in days  
- `status` — Event indicator (1 = censored, 2 = death)  
- `sex` — 1 = Male, 2 = Female  
- `intervention` — Treatment group (e.g., `Standard_Care`, `DrugA`, `DrugB`)  
- `age` — Patient age at baseline  

---

## 📈 Analysis Workflow
1. Load & format data  
2. Compute Kaplan–Meier curves by groups  
3. Fit Cox proportional hazards models  
4. Stratify by gender and age groups  
5. Generate forest plots  
6. Produce baseline characteristics tables & statistical tests  

---

## 📷 Example Outputs

<img width="45%" height="491" alt="Vis 2" src="https://github.com/user-attachments/assets/f3f7c621-d318-4415-bc61-c8af8e2ec4af" />
<img width="45%" height="488" alt="Vis 1" src="https://github.com/user-attachments/assets/8eb304a4-87cd-46cf-a433-6df61c7be1a2" />

---

## 🖥️ Code Availability
- **R** — Using `survival` and `survminer` packages  
- **Python** — Using `lifelines` and `scipy`  
- **SAS** — Using `PROC LIFETEST` and `PROC PHREG`

---

## 🚀 How to Run
**R:**
```r
install.packages(c("survival", "survminer", "dplyr", "ggplot2", "readr"))
source("analysis_R.R")

