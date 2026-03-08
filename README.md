# Steam Game Data Analysis – OLAP & Data Mining

A data warehouse and online analytical processing (OLAP) project built on Steam game data, covering the full pipeline from ETL to multidimensional analysis, reporting, and data mining.

---

## Project Overview

This project was developed as part of a data warehousing course. The goal is to analyze Steam game data across multiple dimensions (sales trends, genre performance, player behavior) using a structured data warehouse, OLAP cube, and machine learning models.

**Team size:** 2 members. Each member owned an independent data table across all pipeline stages. The data mining module was completed individually.

---

## Pipeline

```
Raw Steam Data
     ↓
ETL Pipeline (SSIS)
     ↓
Data Warehouse (SQL Server – Star Schema)
     ↓
OLAP Cube (SSAS) + MDX Queries + Pivot Table
     ↓
Reporting (AI-powered tools + Google Data Studio)
     ↓
Data Mining (Preprocessing → Feature Engineering → ML Models)
```

---

## Modules

### 1. Data Warehouse (SSIS)
- Designed a star-schema data warehouse in SQL Server
- Built ETL pipelines using SSIS to extract, clean, and load raw Steam datasets
- Each team member handled an independent data table end-to-end

### 2. OLAP Analysis (SSAS)
- Developed an OLAP cube with dimensions and measures for multidimensional analysis
- Authored 15 MDX queries covering:
  - Game sales trends
  - Genre performance comparison
  - Player behavior patterns
- Analyzed results via Pivot Table

### 3. Reporting
- Built interactive dashboards and reports using AI-powered reporting tools and Google Data Studio
- Designed for non-technical audiences with visual summaries of key findings

### 4. Data Mining (Individual)
- Preprocessed and engineered features from raw Steam data
- Trained and compared three classification models:

| Model | Purpose |
|---|---|
| Decision Tree | Baseline interpretable classifier |
| XGBoost | Gradient boosting for improved accuracy |
| LightGBM | Efficient boosting for large-scale data |

- Evaluated models using classification metrics (accuracy, precision, recall, F1-score)
- Identified patterns in game popularity and user engagement

---

## Tech Stack

| Layer | Tools |
|---|---|
| ETL | SSIS (SQL Server Integration Services) |
| Data Warehouse | SQL Server (Star Schema) |
| OLAP | SSAS (SQL Server Analysis Services), MDX, Pivot Table |
| Reporting | AI-powered reporting tools, Google Data Studio |
| Data Mining | Python, scikit-learn, XGBoost, LightGBM |
| Data Processing | pandas, NumPy |

---

## Requirements

- SQL Server + SSMS
- Visual Studio with SSIS/SSAS components
- Python 3.x
- Libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `lightgbm`
