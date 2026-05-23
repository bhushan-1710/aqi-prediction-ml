<div align="center">

# 🌫️ Air Quality Index (AQI) Prediction
### Machine Learning | Random Forest | Python

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0-orange?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19VPLykkaoSFSyeARgS2Q9xa9_KXwj8_c)

*Predicting Air Quality Index of Indian cities using real-world pollutant data*

</div>

---

## 🔍 Overview

Air pollution is one of the most serious environmental challenges facing India today. This project builds a **Random Forest Regression** model trained on **29,000+ daily air quality records** across Indian cities to predict the AQI from key pollutant concentrations — PM2.5, PM10, NO2, and CO.

---

## 📊 Results at a Glance

| 🔢 Metric | 📈 Value |
|-----------|---------|
| Model | Random Forest Regressor |
| Dataset Size | 29,000+ records |
| Train / Test Split | 80% / 20% |
| Mean Absolute Error | **23.67** |
| Top Predictor | PM2.5 — 50.8% importance |

---

## 🧠 Feature Importance

| Feature | Importance | Bar |
|---------|-----------|-----|
| 🟥 PM2.5 | 50.8% | ████████████░░░░░░░░░ |
| 🟧 CO | 41.3% | ██████████░░░░░░░░░░░ |
| 🟨 PM10 | 4.3% | █░░░░░░░░░░░░░░░░░░░░ |
| 🟦 NO2 | 3.6% | █░░░░░░░░░░░░░░░░░░░░ |

> 💡 **PM2.5 and CO together account for 92% of the model's predictive power** — highlighting them as the dominant drivers of poor air quality in Indian cities.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 Python | Core language |
| 🐼 Pandas | Data loading and wrangling |
| 🔢 NumPy | Numerical operations |
| 🤖 Scikit-learn | ML model, imputation, evaluation |
| 📊 Matplotlib | Plotting actual vs predicted |
| 🎨 Seaborn | AQI distribution visualisation |
| ☁️ Google Colab | Development environment |

---

## 📁 Project Structure

```
aqi-prediction-ml/
│
├── 📓 aqi_prediction.ipynb     # Main notebook — full code + visualisations
├── 📄 city_day.csv             # Dataset (download from Kaggle link below)
└── 📝 README.md
```

---

## 🚀 How to Run

**1. Clone the repo**
```bash
git clone https://github.com/bhushan-1710/aqi-prediction-ml.git
cd aqi-prediction-ml
```

**2. Install dependencies**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

**3. Download the dataset**

Get `city_day.csv` from [Kaggle — Air Quality Data in India](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india) and place it in the project folder.

**4. Run the notebook**
```bash
jupyter notebook aqi_prediction.ipynb
```
Or open directly in [Google Colab ☁️](https://colab.research.google.com/)

---

## 📓 What the Notebook Covers

- ✅ Loading and exploring the dataset
- ✅ Handling missing values — null target removal + mean imputation on features
- ✅ 80/20 train-test split
- ✅ Training a Random Forest Regressor (100 estimators)
- ✅ Model evaluation using MAE
- ✅ Actual vs Predicted AQI scatter plot
- ✅ Feature importance analysis and bar chart
- ✅ AQI distribution visualisation with KDE curve
- ✅ Predicting AQI for custom pollutant inputs

---

## 🔮 Sample Prediction

```python
new_data = {
    'PM2.5': 120,
    'PM10':  180,
    'NO2':    60,
    'CO':    1.2
}

# ➜ Predicted AQI: 288.25  →  Category: 🟠 Very Poor
```

---

## 🌈 AQI Categories (CPCB Standard)

| AQI Range | Category | Health Impact |
|-----------|----------|--------------|
| 0 – 50 | 🟢 Good | Minimal impact |
| 51 – 100 | 🟡 Satisfactory | Minor discomfort for sensitive people |
| 101 – 200 | 🟠 Moderate | Breathing discomfort on prolonged exposure |
| 201 – 300 | 🔴 Poor | Breathing discomfort for most people |
| 301 – 400 | 🟣 Very Poor | Respiratory illness on prolonged exposure |
| 401 – 500 | ⚫ Severe | Serious health hazard |

---

## 🔭 Future Improvements

- [ ] Add more pollutant features (SO2, O3, Benzene, Toluene)
- [ ] Try XGBoost and compare performance
- [ ] Build a Streamlit web app for live AQI prediction
- [ ] Add city-wise and season-wise analysis
- [ ] Hyperparameter tuning with GridSearchCV

---

## 👤 Author

<div align="center">

**Bhushan Sapkal**
B.Tech — Artificial Intelligence & Data Science
RH Sapat College of Engineering, Nashik

[![GitHub](https://img.shields.io/badge/GitHub-bhushan--1710-181717?style=flat-square&logo=github)](https://github.com/bhushan-1710)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Bhushan_Sapkal-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/bhushan-sapkal-754a34376/)
[![Email](https://img.shields.io/badge/Email-bhushansapkal207@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:bhushansapkal207@gmail.com)

</div>

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
⭐ If you found this useful, consider starring the repo!
</div>
