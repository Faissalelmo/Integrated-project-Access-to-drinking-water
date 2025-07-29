In this second part of the integrated project, we extend our investigation on access to safe and affordable drinking water. You will need to create features, summaries, and visualizations as per the instructions in order to complete the compulsory project MCQ assessment. Download the datasets we’ll be using throughout this project from the Download Additional Files button.

# 💧 Access to Drinking Water – Transforming the Data

This repository contains the second part of the integrated project on **global access to safe and affordable drinking water**, aligned with **UN Sustainable Development Goal 6**.  
In this phase, we transform and analyze the full dataset ranging from **2000 to 2020**, tracking changes over time, comparing regions, and calculating Annual Rates of Change (ARC).

---

## 🔍 Objective

- Transform and clean the dataset (2000–2020) to prepare for temporal analysis.
- Calculate **Annual Rates of Change (ARC)** for national, rural, and urban populations.
- Investigate **yearly trends**, **region-level insights**, and **progress toward full water access**.

---

## 📂 Dataset Overview

We use the **WHO/UNICEF JMP dataset (2000–2020)**. It includes estimates on water access broken down by:
- **National, rural, and urban levels**
- Four access levels: Basic, Limited, Unimproved, Surface

### 📈 Added Features:

| Feature                | Description                                                      |
|------------------------|------------------------------------------------------------------|
| `y_diff`               | Year difference between two observations of the same country     |
| `ARC_n`, `ARC_r`, `ARC_u` | Annual Rates of Change (ARC) for national, rural, and urban basic access |
| `ARC_n_full`, etc.     | Flags for full access (100%) over time                           |
| `wat_bas_x (rounded)`  | Rounded water access values (for detecting full access)          |
| `ARC_diff`             | Difference in ARC between rural and urban areas                  |
| `region`               | Region classification (merged from external file)                |

---

## ✅ Tasks Completed

- ✅ Imported full 2000–2020 dataset
- ✅ Cleaned duplicate values and handled missing/null entries
- ✅ Created `y_diff` to identify time gaps per country
- ✅ Calculated **ARC_n**, **ARC_r**, **ARC_u** using time-series logic
- ✅ Created conditions to classify:
  - Countries with **no data**
  - Countries with **ARC = 0**
  - Countries with **full access**
  - Countries with **ARC < 0** or **ARC > 0**
- ✅ Grouped countries by region and calculated **average ARC per region**
- ✅ Created multiple visualizations including:
  - Histogram of years
  - Histogram of ARC differences
  - Scatterplot: rural ARC vs national ARC vs population vs region

---

## 📊 Key Insights

- Not all countries have data for every year between 2000 and 2020.
- **Rural ARC** is often higher than urban/national, suggesting more recent improvement efforts in rural areas.
- Some countries show **declines** in access over time (negative ARC).
- **Sub-Saharan Africa** has made improvements, but current trends predict full access only by **~2080** unless progress accelerates.
- The **difference between urban and rural ARC** is significant in many regions, emphasizing inequality.

---

## 🔗 Project Files

- **📄 Original Dataset**: WHO/UNICEF JMP (2000–2020)
- **🧮 Summary Sheet**: ARC statistics, access classifications, and regional summaries
- **📊 Charts**: Visualizing trends and disparities across countries and regions

---

### 📎 Access the Google Sheets Project

You can view the data transformation and visualizations on Google Sheets here:  
👉 [**Open Project Sheet**](https://docs.google.com/spreadsheets/d/YOUR-SHEET-ID-HERE)

> ℹ️ Replace `YOUR-SHEET-ID-HERE` with your actual Google Sheets link.

---

## 🛠️ Tools & Methods

- **Google Sheets**  
- Conditional logic (`IF`, `EQ`, `COUNTIFS`, etc.)  
- Error handling (`IFERROR`)  
- Sorting and filtering  
- Charting (Histogram, Scatterplot, Column Charts)

---

## 👤 Author

**Faissal Elmokaddem**  
Data Science & Engineering Student | [ALX Africa Program 2025]

---

> 🛑 This repository is part of the ALX Integrated Project on Access to Drinking Water. Please do not copy without permission.
