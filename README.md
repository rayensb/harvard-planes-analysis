# 🛫 Harvard Planes Dataset Analysis (Python, Pandas)

## Overview
This project explores the **Harvard Planes dataset** to uncover insights about flight delays and diverted flights.  
Using **Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)**, the analysis covers **data cleaning, exploratory analysis, feature engineering, and baseline modeling**.

## Objectives
- Inspect and clean flight delay data  
- Identify the best **day of the week** and **time of day** to minimize delays  
- Analyze the relationship between **aircraft age and delays**  
- Build a **logistic regression model** to understand flight diversion probability  
- Visualize the effect of key features over time  

## Tools
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)  
- Jupyter Notebook  

## Methodology
1. **Data Cleaning & Inspection**  
   - Removed missing values, standardized time formats  
   - Defined consistent delay metrics  

2. **Exploratory Data Analysis (EDA)**  
   - Delay distribution by **day of week** and **time of day**  
   - Relationship between **plane age and delays**  
   - Longitudinal analysis across years  

3. **Modeling (Logistic Regression)**  
   - Target: probability of a flight being **diverted**  
   - Features: `Taxi_dum`, `DepDelay`, `CRSElapsedTime`, `Distance`  
   - Coefficients compared across years  

---

## Key Insights

### Best Day to Fly
- **Sundays** consistently show the **lowest delay rates**.  
- Over multiple years, **Day 6** (Sunday) remained the best choice.  
<img width="751" height="452" alt="Best day over the years" src="https://github.com/user-attachments/assets/96cd2c6a-217a-44d9-816c-bafea59251eb" />

### Best Time to Fly
- Flights departing **early in the morning (5–6 AM)** are least likely to be delayed.  

<img width="751" height="452" alt="Count of best time" src="https://github.com/user-attachments/assets/9cb9ad38-6b5a-4197-be12-3a1b813b23f7" />

### Aircraft Age & Delays
- Surprisingly, **older planes had fewer delays**.  
- Newer planes may face more initial operational issues, while older ones are more stable after early adaptations.  
- The effect **diminishes over time** due to technological advancements.  
- Correlation analysis shows that **plane age explains ~30% of delays** in early years.  
![Correlation coefficient over time](https://github.com/user-attachments/assets/448b40ab-01b4-4976-9026-7849e8b38d70)


### Logistic Regression (Diverted Flights)
- Logistic regression tested diversion probability with four predictors:  
  - `Taxi_dum`, `DepDelay`, `CRSElapsedTime`, `Distance`  
- Results show **stable coefficient trends across years**, despite missing data in the earliest years.  
![Regression coefficients visualization](https://github.com/user-attachments/assets/d100e9bc-89d9-4747-95d5-99a4e46049ce)


---

## Deliverables
- Jupyter Notebook with code & analysis  
- Visualizations for delay patterns and logistic regression coefficients  
- Cleaned dataset (if shareable)  

## Conclusion
- **Best time to travel**: early morning, mid-week flights (especially Sundays).  
- **Plane age**: older planes tend to have fewer delays, though the effect is decreasing due to modern technology.  
- **Logistic regression** confirmed that delay-related and distance features consistently predict diversion probability.  

This project demonstrates how **systematic EDA and visualization can turn raw aviation data into actionable insights** for both passengers and airlines.
