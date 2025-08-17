# 🏥 Forecasting Aged Care Facility Demand in Australia

This repository contains the full code, datasets, and outputs for the project:  
**“Forecasting Aged Care Facility Demand in Australia Using Population Projections and Service Availability Data”**  
(COMP SCI 7319OL: Big Data Analytics, 2025).

---

## 📖 Project Overview

Australia’s population is ageing rapidly, raising urgent questions about whether aged care services can keep pace with demand.  

This project integrates **population projections** from the **Australian Bureau of Statistics (ABS)** with **aged care capacity data** from the **Australian Institute of Health and Welfare (AIHW)**. Using **big data analytics, clustering, and regression modelling**, we forecast where service shortfalls are most likely to occur by 2032.  

Key insights include:
- A **near-perfect linear relationship** between elderly population (70+) and aged care demand (R² = 1.000).  
- **Remoteness** plays a critical role, with rural and remote regions showing disproportionately lower service coverage.  
- By 2032, **~50,000 new aged care places** may be required nationwide, with the sharpest increases in coastal retirement hubs and regional towns.  

---

## 📂 Repository Structure

```plaintext
├── data/
│   ├── cleaned_CURF_file.xlsx
│   ├── Aged-Care-Data-Snapshot-2023.xlsx
│   ├── Projected-population-Australia.xlsx
│
├── notebooks/
│   ├── Assignment_1_Part_B.ipynb   # Clustering and exploratory analysis
│   ├── Assignment_1_Part_C.ipynb   # Regression modelling and forecasting
│
├── figures/
│   ├── R2_Score_by_Model.png
│   ├── Residuals_Linear.png
│   ├── Actual_vs_Predicted.png
│   ├── Distribution_Capacity_SA3.png
│   └── Aged_Care_Capacity_Remoteness.png
│
├── report/
│   ├── Assignment_1_Part_D_Final_Report.pdf
│   └── latex_source/ (if applicable)
│
└── README.md
```

---

## ⚙️ Requirements

This project was developed in **Python 3.9+** using the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Optional (for mapping and geospatial analysis):
```bash
pip install geopandas folium
```

---

## 🚀 How to Run

1. **Clone this repository**
   ```bash
   git clone https://github.com/Hazimshaikh/Assignment-1--Big-Data-Analysis-.git
   cd Assignment-1--Big-Data-Analysis-
   ```

2. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

3. **Run the analysis**
   - `notebooks/Assignment_1_Part_B.ipynb` → Exploratory analysis and clustering  
   - `notebooks/Assignment_1_Part_C.ipynb` → Regression models and forecasting  

4. **View results**  
   Outputs are saved automatically in the `figures/` folder.

---

## 📊 Key Results

- **Model Performance**
  - Linear Regression: R² = **1.000**, MAE ≈ 0, RMSE ≈ 0  
  - Ridge Regression: R² ≈ **0.999997**, MAE ≈ 4, RMSE ≈ 5  
  - Random Forest: R² ≈ **0.999994**, MAE ≈ 7, RMSE ≈ 9  

- **Forecast to 2032**
  - Demand will outpace capacity by ~50,000 places nationally.  
  - Coastal retirement regions and rural/remote towns will experience the largest shortages.  

---

## 📌 References

- Austin, A. et al. (2021). *Actual and projected gaps in the provision of residential aged care in NSW*.  
- Lewis, R.L. et al. (2025). *Set up to fail: systemic problems in in-home aged care*.  
- Australian Institute of Health and Welfare (2023). *Aged Care Data Snapshot*.  
- Australian Bureau of Statistics (2023). *Population Projections, Australia (2022–2071)*.  

---

## 📧 Contact

**Author:** Hazim Shaikh  

---

✨ *To reproduce the full study, start with the notebooks in `notebooks/` and follow the workflow step by step.*  
