# 🏥 Hospital Food Waste Analytics – Power BI Case Study

A complete analytics project exploring food & dairy waste in a 12-bed hospital ward.  
The goal is to identify waste patterns, understand operational drivers, and demonstrate how dynamic meal ordering can reduce waste by approximately **20%**.


## 🔍 Business Problem

The ward operates with a maximum capacity of 12 beds.  
Patient count changes daily (admissions, discharges, NPO status, diet changes),  
but **meal and dairy orders were fixed and not adjusted**.

This mismatch created:

- Overproduction of meals  
- Avoidable food waste  
- Unnecessary cost in DKK  
- Operational inefficiency  



## 📁 Dataset (Synthetic but Realistic)

The dataset simulates the ward’s daily operations:

- `Patients_Current` (0–12 beds)  
- `Meals_Ordered`, `Meals_Consumed`, `Meals_Wasted`  
- `Dairy_Ordered`, `Dairy_Consumed`, `Dairy_Wasted`  
- `Main_Waste_Driver`  
- `Cost_of_Waste_DKK`  

All data files are included in the `/data` folder.



## 📊 Key Metrics (DAX)

### Waste Percentage Measures
- **FoodWastePct** = Meals_Wasted / Meals_Ordered  
- **DairyWastePct** = Dairy_Wasted / Dairy_Ordered  

### Recommended Ordering Model  
A dynamic ordering model based on patient count to reduce waste.



## 📈 Power BI Dashboards

### **1️⃣ Summary View**
- Avg Food Waste  
- Avg Optimized Food Waste  
- Waste Reduction %  
- Executive Summary Text  

### **2️⃣ Analysis View**
- Daily food & dairy waste trend  
- Waste cost over time  
- Waste by main driver  
- Monthly waste cost  
- Business insights  



## 🎯 Insights

- Overproduction is the main waste driver (~18K DKK).  
- Monthly waste cost is stable (~7K DKK/month).  
- Optimized ordering reduces waste by **13–20%**.  
- Clear opportunity for operational improvement.  



## 🛠 Tools Used

- Power BI  
- DAX  
- Excel  
- GitHub  



## 📂 Repository Structure

