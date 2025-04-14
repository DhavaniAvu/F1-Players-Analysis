# 🏁 F1 Racing Data Analysis & Driver Performance Modeling
## 📌 Overview
This project explores a comprehensive dataset of Formula 1 racing results, merging data from multiple sources such as lap times, pit stops, driver standings, and constructor information. The goal is to clean and process the data, engineer useful features, and build insightful visualizations and models to understand performance patterns and predict outcomes.

## 🎯 Objectives
Merge and enrich F1 race results with driver, constructor, lap time, and pit stop data

Clean, preprocess, and engineer features from noisy or inconsistent race data

Identify key factors that influence race outcomes and driver success

Visualize performance metrics and correlations among variables

Build predictive models to classify race winners and analyze feature importances

## 📁 Project Structure

- F1-Racing-Analysis/
  - **Code/**
    - ML Modeling.ipynb  — Preprocessing and model building
    - drivers.ipynb — Driver analysis and EDA
  - **CSV files/**
    - circuits.csv  
    - constructor_results.csv  
    - constructor_standings.csv  
    - constructors.csv  
    - driver.csv  
    - driver_standings_org.csv  
    - drivers_org.csv  
    - drivers_standingss.csv  
    - final_data.csv  
    - final_drivers.csv  
    - lap_times.csv  
    - lap_times_org.csv  
    - pit_stops.csv  
    - pit_stops_org.csv  
    - qualifying.csv  
    - races.csv  
    - results.csv  
    - results_with_names.csv  
    - seasons.csv  
    - sprint_results.csv  
    - status.csv  
  - **Visualisations/**
    - Visualization1.html — EDA output in HTML  
    - Visualization1.ipynb  
    - Visualizations.html  
    - Visualizations.ipynb  
    - Visualizations2.ipynb  
    - Visulaizations.twb — Tableau workbook
  - README.md — Project documentation



## 🧼 Data Cleaning & Feature Engineering
- Dropped redundant columns like `duration`, `positionText`, and `time` from race logs  
- Renamed key columns for clarity (e.g., `lap` → `lap_laptimes`, `milliseconds` → `lap_duration`)  
- Converted `fastestLapTime` from string (`mm:ss`) to milliseconds  
- Replaced all missing values represented as `\N` with `NaN` and handled them  
- Converted categorical race outcomes into binary classification labels  

**Merged race results with:**
- Driver names (`driverRef`)  
- Team names (`constructors`)  
- Pit stop and lap time durations  
- Status logs  

---

## 📊 Exploratory Data Analysis (EDA)
- Merged driver standings and personal data for deep-dive analysis  

**Analyzed:**
- Win count distribution by race position  
- Points scored per driver across seasons  
- Driver consistency and average performance  

**Visualized:**
- Wins vs Position (line chart)  
- Correlation heatmaps  
- Missing data & anomalies  

---

## 🤖 Machine Learning Workflow
Performed binary classification:

- **Target**: Whether the driver **won the race (1)** or **not (0)**

**Techniques used:**
- Label encoding  
- Handling missing values  
- Train/test split  
- Model training (`RandomForestClassifier`)  
- Feature importance analysis  

---

## 📈 Visualizations
- Interactive dashboards in **Tableau** (`Visulaizations.twb`)  
- HTML & Notebook-based plots using:
  - `Matplotlib`  
  - `Seaborn`  

**KPIs visualized include:**
- Driver race count  
- Win % by constructor  
- Lap & pit stop patterns  

---

## 🧪 Tools & Technologies
- **Languages**: Python (Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn)  
- **Visualization**: Tableau, HTML, Power BI (if applicable)  
- **Data Storage**: CSVs  
- **ML Libraries**: Scikit-learn (for classification modeling)  

---

## 📌 Key Takeaways
- Integrated raw, messy data from multiple CSVs into a clean, unified dataset  
- Uncovered key performance indicators for F1 drivers and constructors  
- Modeled winning prediction with engineered race features  
- Delivered interactive dashboards and insightful statistical graphics  
