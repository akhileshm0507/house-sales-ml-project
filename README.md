# 🏠 House Sales in King County, USA

A complete data science project analyzing residential home sales in King County, Washington. This project covers the full ML pipeline — from data wrangling and EDA through to polynomial regression and Ridge regularization.

---

## 📋 Project Overview

This project was completed as the **final capstone** for the IBM Data Science / Machine Learning course. It walks through:

- Loading and cleaning real-world housing data
- Exploratory data analysis (EDA) with visualizations
- Building progressively more complex regression models
- Evaluating and comparing model performance using R²

---

## 📁 Project Structure

```
king-county-house-sales/
│
├── king_county_house_sales.ipynb   # Main Jupyter notebook (all 10 questions)
├── requirements.txt                 # Python dependencies
├── .gitignore                       # Files to exclude from version control
└── README.md                        # This file
```

---

## 📊 Dataset

**Source:** IBM Skills Network / Coursera  
**URL:** [kc_house_data_NaN.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0101EN-SkillsNetwork/labs/FinalModule_Coursera/data/kc_house_data_NaN.csv)

The dataset contains house sale prices for King County, Washington (May 2014 – May 2015), with features including:

| Feature | Description |
|---------|-------------|
| `price` | Sale price (target variable) |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `sqft_living` | Interior living space (sq ft) |
| `sqft_lot` | Lot size (sq ft) |
| `floors` | Number of floors |
| `waterfront` | Waterfront property (0/1) |
| `view` | View quality rating |
| `grade` | Overall grade of the home |
| `sqft_above` | Square footage above ground |
| `sqft_basement` | Square footage of basement |
| `lat` / `long` | Geographic coordinates |
| `sqft_living15` | Living space of nearest 15 neighbors |

---

## 🧪 Questions Covered

| # | Task | Method |
|---|------|--------|
| Q1 | Drop irrelevant columns | `df.drop()` |
| Q2 | Handle missing values | Replace NaN with column mean |
| Q3 | Analyze floor distribution | `value_counts()` |
| Q4 | Waterfront vs price analysis | Boxplot |
| Q5 | `sqft_above` vs price correlation | Regression plot |
| Q6 | Simple linear regression | `LinearRegression` on `sqft_living` |
| Q7 | Multiple linear regression | `LinearRegression` on 11 features |
| Q8 | Polynomial pipeline | `StandardScaler` → `PolynomialFeatures` → `LinearRegression` |
| Q9 | Ridge regression | `Ridge(alpha=0.1)` with train/test split |
| Q10 | Polynomial + Ridge | `PolynomialFeatures(degree=2)` + `Ridge(alpha=0.1)` |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/king-county-house-sales.git
cd king-county-house-sales

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook king_county_house_sales.ipynb
```

---

## 📦 Requirements

See [`requirements.txt`](requirements.txt) for the full list. Key libraries:

- `pandas` — data manipulation
- `numpy` — numerical computing
- `matplotlib` / `seaborn` — visualization
- `scikit-learn` — machine learning models and pipelines

---

## 📈 Results Summary

Run the notebook to generate all R² scores. The final cell prints a complete performance summary table comparing all five models.

---

## 🛠 Technologies Used

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).
