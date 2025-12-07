# Data Analysis in Excel: Bike Sales & Customer Insights

## Objective
End-to-end data analysis in Excel—from data cleaning and transforming raw customer data, to analyzing purchase trends, to building an interactive dashboard, in order to identify key factors influencing bike purchase decisions.

---

## Dataset Overview
The dataset contains customer records with attributes such as:

- **Demographics:** Age, Gender, Marital Status, Region  
- **Socioeconomic:** Income, Education, Occupation, Home Ownership  
- **Lifestyle:** Number of Children, Cars Owned, Commute Distance  
- **Target Variable:** Purchased Bike (Yes/No)  

---

## 1. Data Cleaning & Preparation

### Steps Taken
- **Age Brackets:** Categorized using:``` =IF(L2>54,"55+", IF(L2>=31,"31-54", IF(L2<31,"0-30","Invalid"))) ```
- **Column Standardization:** Corrected column names (e.g., `Martial Stal` → `Marital Status`, `Home Ownt` → `Home Own`)  
- **Categorical Value Standardization:**  
  - Marital Status: `M` → `Married`, `S` → `Single`  
  - Gender: `F` → `Female`, `M` → `Male`  
- **Education & Occupation:** Expanded abbreviations for clarity  
- **Numeric Formatting:** Standardized Income format (removed trailing `.00`)  
- **Target Variable:** Renamed to `Purchased Bike` for consistency  

### Few of the Excel Tools Used:
- Formulas: `IF`, `XLOOKUP`, `TRIM`  
- Find & Replace  
- Data Validation & Conditional Formatting  
- Text-to-Columns for splitting fields  

---

## 2. Pivot Table Analysis: Income, Gender, and Bike Purchase Trends


- Created Pivot Tables to analyze:  
  - **Average Income per Purchase**  
  - **Customer Commute Distance**  
  - **Customer Age Brackets**  

### Key Insights
- Male buyers had higher average income than female buyers  
- Non-buyers sometimes had slightly higher income than buyers  
- Income alone is **not the sole predictor** of bike purchase  

---

## 3. Interactive Dashboard in Excel

### Dashboard Components

**Filters (Slicers):**
- Marital Status  
- Region  
- Education Level  

**Visualizations (Charts):**
1. **Avg Income Per Purchase** – Clustered Column chart comparing income by gender and purchase decision  
2. **Customer Age Brackets** – Line chart showing purchase distribution across age groups  
3. **Customer Commute Distance** – analyzing how commute distance relates to bike purchases  

**Dashboard Features:**
- Interactive slicers for dynamic filtering  
- Pivot Charts update in real-time based on slicer selections  
- Clean layout using shapes, text boxes, and formatting  
- Named ranges and table references for maintainability  

---

## Summary: Excel Analysis Outcomes

- **Data Cleaning in Excel:** Standardized data using formulas and built-in tools  
- **Pivot Table Analysis:** Revealed trends across demographics and purchase behavior  
- **Interactive Dashboard:** Created a dynamic, filter-driven dashboard using Excel visualization tools  

### Business Implications
- Bike buyers tend to be in the **31–54 age bracket**  
- **Commute distance** and **region** significantly influence purchase likelihood  
- **Male customers** with moderate commutes represent a key target segment  

---

## Credits
- Dataset source and guidance: **Alex The Analyst**  
