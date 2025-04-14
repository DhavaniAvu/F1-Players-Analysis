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

F1-Racing-Analysis

├── Code
│   ── ML Modeling.ipynb           # Preprocessing and binary classification modeling
│   ── drivers.ipynb              # EDA and driver-level analysis
│
├── CSV files
│   ── final_data.csv             # Merged and processed data
│   ── results.csv                # Raw F1 race results
│   ── drivers_org.csv            # Original drivers information
│   ── constructors.csv           # Constructor (team) information
│   ── lap_times.csv              # Lap time logs per driver per lap
│   ── pit_stops.csv              # Pit stop records
│   ── status.csv                 # Final status of drivers
│   ── ...                        # Additional supporting files
│
├── Visualisations
│   ── Visualization1.html        # EDA HTML output
│   ── Visualizations.ipynb       # Visualization notebooks (matplotlib, seaborn)
│   ── Visulaizations.twb         # Tableau workbook
│
└── README.md                      # Project documentation


---

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
