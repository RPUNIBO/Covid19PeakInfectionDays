# COVID-19 Data Analysis Using Pandas, PySpark, and Dask

## 📊 Overview

This project performs comprehensive analysis on a COVID-19 dataset using Python-based data analytics tools including **Pandas**, **PySpark**, and **Dask**. It covers data wrangling, visualization, performance benchmarking, and advanced data querying on both national (India and Switzerland) and global scales.

## 📁 Dataset

The dataset used is a CSV file (`COVID.csv`) containing COVID-19 statistics for multiple countries including:

- Date
- Country
- Cumulative positive cases
- Deaths
- Hospitalization
- ICU admissions
- Geolocation data

> The dataset is loaded from Google Drive within the notebook.

---

## 🔍 Analysis Performed

### 🇮🇳 India-Specific Analysis (Using Pandas)

- Tracked the daily increase in COVID-19 cases.
- Identified the worst day (highest number of daily active cases).
- Visualized daily trends using Matplotlib.

### 🇨🇭 Switzerland Seasonal Hospitalization Trends

- Compared average hospitalized patients during **summer** (June–September) and **winter** (December–March).
- Visualized time series of hospitalization data.

### 🌎 Global Analysis

- Computed **average cumulative positive cases** per country.
- Identified the top countries with highest average case numbers.
- Benchmarked execution time using:
  - **Pandas**
  - **PySpark**
  - **Dask**

### 🧮 Monte Carlo Integration

Implemented a Monte Carlo integration method to numerically estimate the integral of a function `f(x) = x^2` over a given range.

---

## ⚙️ Tools & Libraries

- **Python 3.x**
- **Pandas** (for initial data processing)
- **Matplotlib** (for plotting)
- **PySpark** (for distributed computing)
- **Dask** (for parallelized operations on large datasets)
- **Google Colab** (as execution environment)

---

## 📈 Visualizations

- Line plots of daily active cases (India)
- Hospitalization trends (Switzerland)
- Bar chart of average positive cases by country

---

## ⏱️ Performance Comparison

| Tool      | Task                             | Time Taken |
|-----------|----------------------------------|------------|
| Pandas    | Average cases per country        | ~0.26 sec  |
| PySpark   | Average cases with groupBy       | ~1.41 sec  |
| Dask      | Average cases (lazy execution)   | ~0.62 sec  |

---

## 🚀 Getting Started

1. Clone the repository or open the notebook in Google Colab.
2. Ensure your dataset `COVID.csv` is placed correctly (e.g., in Google Drive).
3. Install required packages using pip commands within the notebook:

   ```bash
   !pip install pyspark dask[dataframe] memory_profiler
