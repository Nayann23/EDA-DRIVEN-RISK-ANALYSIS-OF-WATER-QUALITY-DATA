# ⚠️ Risk Analysis of Water Quality Data – EDA-Driven Insights

This project focuses on **assessing the potential health risks** associated with water quality using an Exploratory Data Analysis (EDA) approach. Rather than building a machine learning model, we concentrated on analyzing how each water attribute aligns with real-world safety standards — and identified serious concerns in the dataset.

---

## 📁 Project Structure

```
📦RISK-ANALYSIS-OF-WATER-QUALITY-DATA
├── 📁 data
│   └── water_potability.csv         # Raw dataset file
│
├── 📁 notebook
│   └── EDA-Driven-Risk-Analysis-Of-Water-Quality-Data.ipynb  # Main visual risk analysis notebook
│
├── column_info.md                   # Contains domain-based explanation of each column
└── README.md                        # Project overview
```

---

## ⚙️ What This Project Covers

- **Data Cleaning**: Identified missing values and verified the integrity of data types.
- **Risk-Focused Feature Profiling**: Explained each column using WHO/EPA-based safe ranges.
- **Univariate Risk Analysis**: Plotted each feature with safety thresholds marked clearly.
- **Commentary Per Feature**: Added markdown summaries under each plot that compare the data to safe limits.
- **Correlation Heatmap**: Included a visual to check feature-to-feature relationships.
- **Outcome**: Found the data **too unreliable** for model training, and halted development at the EDA stage.

---

## ⚠️ Why ML Modeling Was Abandoned

- Several key features like `Solids`, `Sulfate`, `Organic_carbon`, and `Turbidity` were **drastically outside safe drinking limits**.
- Only a handful (`Conductivity`, `Trihalomethanes`, `Hardness`) aligned with realistic values — not enough for modeling.
- The target column `Potability` was **imbalanced** (64% "Not Potable"), making the outcome unreliable.
- **Conclusion**: Proceeding with ML would introduce misleading results and false confidence.

---

## 💡 Final Insight

> **Risk analysis is about responsibility — if the data isn't realistic, it's better to stop.**  
> A truthful, safety-aware EDA tells a stronger story than a forced prediction model.

---

## 📌 Dataset Source

Sourced from public repositories. The dataset is labeled for potability (0 = unsafe, 1 = safe) based on nine physical-chemical water attributes.

---

## 📄 License

Open for academic, portfolio, and demonstration purposes.
