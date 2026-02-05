# 🏥 Hospital Food Waste Analytics – Power BI Case Study

A complete analytics project exploring food & dairy waste in a 12-bed hospital ward.  
The goal is to identify waste patterns, understand operational drivers, and demonstrate how dynamic meal ordering can reduce waste by ~20%.

---

## 📌 Business Problem

The ward has a maximum capacity of 12 beds.  
Patient count changes daily (admissions, discharges, NPO status, diet changes),  
but **meal and dairy orders were fixed and not adjusted**.

This mismatch led to:

- Overproduction of meals
- avoidable food waste
- unnecessary cost in DKK  
- operational inefficiency  

---

## 📊 Dataset (Synthetic but Realistic)

The dataset simulates the ward’s daily operations:

- `Patients_Current` (0–12 beds)
- `Meals_Ordered`, `Meals_Consumed`, `Meals_Wasted`
- `Dairy_Ordered`, `Dairy_Consumed`, `Dairy_Wasted`
- `Main_Waste_Driver`
- `Cost_of_Waste_DKK`

Data files will be placed in `/data`.

---

## 🧠 Key Metrics (DAX)

### Waste Percentage Measures
- **FoodWastePct** = Meals_Wasted / Meals_Ordered  
- **DairyWastePct** = Dairy_Wasted / Dairy_Ordered

### Recommended Ordering Model
A dynamic ordering model based on patient count:

