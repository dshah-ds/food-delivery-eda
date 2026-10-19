# 🍽️ Food Delivery EDA — India Restaurant Dataset

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green?logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> An end-to-end **Exploratory Data Analysis (EDA)** project on a large-scale food delivery dataset from India — covering data cleaning, feature engineering, correlation analysis, and actionable business insights.

---

## 📌 Project Overview

This project analyzes restaurant data across **98 cities in India** with over **211,000 rows** to understand what drives ratings, customer engagement, and delivery adoption. The analysis is structured to help both **existing restaurant owners** and **new business entrants** make data-informed decisions.

---

## 📊 Dataset

| Attribute | Details |
|---|---|
| **Source** | Food Delivery Dataset (`food_dely.csv`) |
| **Original Size** | 211,944 rows × 26 columns |
| **After Cleaning** | 60,011 rows × 16 columns |
| **Coverage** | 98 cities across India |

You can also download the dataset from - 
https://drive.google.com/file/d/1u2DfkYnux4E_IraLVBd0LFSFp-xR9t5i/view?usp=sharing

**Key columns used:**
`name`, `city`, `locality`, `cuisines`, `average_cost_for_two`, `price_range`, `aggregate_rating`, `rating_text`, `votes`, `photo_count`, `delivery`, `latitude`, `longitude`

---

## 🔍 Key Findings

- 💸 **Higher price ≠ Higher rating** — No strong correlation between cost and customer ratings
- 📸 **Photos drive engagement** — More restaurant photos → more votes → more business
- 🚗 **Delivery is underutilized** — Only a minority of restaurants offer delivery (first-mover opportunity)
- 🗺️ **Northeast region** leads in restaurant density and cuisine variety
- 🏷️ **Price Range 3** provides the best rating-to-cost ratio
- ⭐ **Popular = Well-rated** — Higher vote count strongly correlates with better ratings

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| `Python 3.11` | Core language |
| `pandas` | Data wrangling & analysis |
| `numpy` | Numerical computations |
| `matplotlib` | Base visualizations |
| `seaborn` | Statistical plots & heatmaps |
| `Jupyter Notebook` | Interactive analysis environment |

---

## 📁 Repository Structure

```
food-delivery-eda/
│
├── miniProject.ipynb       # Main EDA notebook
├── food_dely.csv           # Dataset
├── README.md               # Project documentation
├── requirements.txt        # Python dependencies
└── .gitignore              # Git ignore rules
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/dshah-ds/food-delivery-eda.git
cd food-delivery-eda
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Add the dataset
Place `food_dely.csv` in the root directory of the project.

### 5. Launch the notebook
```bash
jupyter notebook miniProject.ipynb
```

---

## 📈 Analysis Walkthrough

| Section | Description |
|---|---|
| **1. Import & Setup** | Libraries loaded, display options configured |
| **2. Read Data** | Dataset loaded and initially inspected |
| **3. Data Preparation** | 11 irrelevant columns dropped, copy created |
| **4. EDA Basics** | Shape, dtypes, duplicates checked |
| **5. Missing Values** | Null values filled with `'unknown'` (<5% threshold) |
| **6. Feature Engineering** | `average_cost_for_one` derived; `region` column created using lat/lon midpoints |
| **7. Correlation Analysis** | Scatter plots, heatmaps, boxplots, count plots |
| **8. Business Insights** | Actionable recommendations for owners |
| **9. Extra Insights** | City-level counts, cuisine splits |

---

## 💡 Business Insights Summary

### For Existing Restaurant Owners
- Encourage photo uploads via discounts — photo count directly correlates with votes and business
- Enable delivery — most restaurants don't offer it, creating a first-mover advantage
- Keep prices economical to maximize order volume and engagement

### For New Business Owners
- North Indian cuisine is the safest volume bet; Continental scores highest ratings
- Target the Northeast region — highest concentration of restaurant activity and cuisine variety
- Aim for Price Range 3 — it hits the "premium feel" without the harsh expectations of Range 4

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open a PR or issue.

---

## 📜 License

This project is for educational and portfolio purposes.

---

## Author

**Devam Shah** · Data Scientist & Analytics Engineer

- Website: [devam-shah.com](https://devam-shah.com)
- LinkedIn: [linkedin.com/in/devam-a-shah](https://www.linkedin.com/in/devam-a-shah)
- GitHub: [github.com/dshah-ds](https://github.com/dshah-ds)
- Medium: [@devamshah26](https://medium.com/@devamshah26)
- Blog: [One Notebook at a Time](https://onenotebookatatime.blogspot.com)

