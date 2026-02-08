# 🏥 Hospital Food Waste Analytics – Power BI Case Study
![Power BI](https://img.shields.io/badge/PowerBI-Analytics-F2C811?logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Dataset](https://img.shields.io/badge/Dataset-Synthetic-blue)

This project addresses the operational mismatch between patient occupancy and meal procurement in a 12-bed hospital ward.  
By transitioning from a **static ordering system** to a **dynamic, data-driven procurement model**, the analysis demonstrates a potential **20% reduction in food waste** and notable yearly cost savings.

---

## 📌 Table of Contents
- [Business Problem](#-business-problem)
- [Dataset (Synthetic but Realistic)](#-dataset-synthetic-but-realistic)
- [Key Metrics (DAX)](#-key-metrics-dax)
- [Dashboard Highlights](#-dashboard-highlights)
  - [Executive Summary View](#1️⃣-executive-summary-view)
  - [Operational Analysis View](#2️⃣-operational-analysis-view)
- [Strategic Insights](#-strategic-insights)
- [Tools Used](#-tools-used)
- [Repository Structure](#-repository-structure)
- [Resume-Ready Description](#-resume-ready-description)

---

## 🔍 Business Problem

The ward previously operated on **fixed daily meal orders**, regardless of real patient volume.

Daily fluctuations in:
- Admissions  
- Discharges  
- NPO status (“Nothing by Mouth”)  
- Diet / clinical changes  

…were **not** reflected in kitchen orders.

This led to:

### ❌ Financial Leakage  
Significant annual waste cost in DKK (≈18,000 DKK avoidable).

### ❌ Operational Rigidity  
No ability to scale meals according to demand.

### ❌ Sustainability Gaps  
High volume of avoidable organic waste (meals + dairy).

---
## 📁 Dataset (Synthetic but Realistic)

The dataset simulates the ward’s daily operations:

- `Patients_Current` (0–12 beds)  
- `Meals_Ordered`, `Meals_Consumed`, `Meals_Wasted`  
- `Dairy_Ordered`, `Dairy_Consumed`, `Dairy_Wasted`  
- `Main_Waste_Driver`  
- `Cost_of_Waste_DKK`  

All data files are included in the `/data` folder.

---

## 📊 Key Metrics (DAX)

| Metric | Logic | Purpose |
|--------|--------|---------|
| **Waste %** | `DIVIDE([Total Wasted], [Total Ordered])` | Tracks procurement efficiency |
| **Optimization Gap** | `[Current Cost] - [Dynamic Model Cost]` | Measures potential savings |
| **Patient Density** | `AVERAGE(Patients_Current)` | Identifies patterns of demand |

---

## 📈 Dashboard Highlights

### **1️⃣ Executive Summary View**
High-level KPIs showing **Current State vs Optimized State**, focused on ROI and savings potential.

<p align="center">
  <img src="https://github.com/user-attachments/assets/f20ced3d-9eaf-4adb-a399-d34c7af29a93" width="750" alt="Summary View">
</p>

---

### **2️⃣ Operational Analysis View**
A deep dive into daily waste trends, cost drivers, and monthly patterns.  
Provides actionable insights for ward managers and kitchen operations.

<p align="center">
  <img src="https://github.com/user-attachments/assets/f07b18cc-0fd2-4451-a76e-f4ba3b5e4a99" width="750" alt="Analysis View">
</p>

---

## 🎯 Strategic Insights

### 🔺 The “Fixed Order” Trap
- **85%** of waste comes from **overproduction**  
- Annual avoidable cost: **~18,000 DKK**

### 📉 Consistency of Waste
- Monthly waste ≈ **7,000 DKK**  
- Problem is **systemic**, not seasonal

### 🚀 Optimization Impact
Implementing a dynamic ordering model:  
`Adjusted Orders = Current Patients + 10% Buffer`

Results in:
- **13–20% reduction in waste**  
- Clear operational and financial gains  

---

## 🛠 Tools Used

- Power BI  
- DAX  
- Excel  
- GitHub  

---

## 📁 Repository Structure

```
Hospital-Food-Waste-Analytics/
├── data/       # CSV / Excel datasets
├── pbix/       # Power BI report file (.pbix / .pbit)
├── visuals/    # Dashboard screenshots
└── README.md   # Project documentation
```



---

## 🚀 Resume-Ready Description

Designed and delivered a Power BI analytics model for hospital food-waste optimization.  
Built a dynamic ordering system that identifies **20% waste reduction**, saving **~18,000 DKK annually**, using DAX modeling, scenario analysis, and cost-driver exploration.

---

