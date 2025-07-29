In this first part of the integrated project, we investigate access to safe and affordable drinking water. You will need to create features, summaries, and visualizations as per the instructions in order to complete the compulsory project MCQ assessment. Download the datasets we’ll be using throughout this project from the Download Additional Files button.

# 🌍 Access to Drinking Water – Understanding the Data

This repository contains the first part of an integrated data analysis project focused on global **access to safe and affordable drinking water**, in alignment with **United Nations Sustainable Development Goal 6: Clean Water and Sanitation**.

## 📊 Project Overview

The goal of this phase is to **explore, clean, and understand** the structure and meaning of the dataset derived from the **WHO/UNICEF JMP (Joint Monitoring Programme) 2020 Estimates on the Use of Water**.

We aim to:
- Identify disparities in access to drinking water across income groups, urban/rural areas, and population sizes.
- Clean and prepare data for proper analysis and visualization in **Google Sheets**.
- Generate new insights through visual and statistical summaries.

---

## 🧾 Dataset Description

The dataset contains 16 original features, such as:
- `name`: Country or area
- `income_group`: Economic classification (e.g., Low income, High income)
- `pop_n`: National population (in thousands)
- `pop_u`: Urban population share (%)
- `wat_bas_n`, `wat_lim_n`, `wat_unimp_n`, `wat_sur_n`: National access levels
- `wat_bas_r`, `wat_bas_u`, etc.: Rural and Urban access breakdown

We added derived features including:
- `value_cnt` – to identify faulty imports
- `pop_u_val`, `pop_r`, `pop_n (m)` – for demographic calculations
- `wat_bas_n (rounded)` – to fix erroneous data (>100%)
- Rounded urban/rural population shares (`pop_u (rounded)`, `pop_r (rounded)`)
- Encoded `income_group_numeric` for easier sorting and visualization

---

## ✅ Tasks Completed

- ✅ Imported and cleaned the data (handled semicolon separators and missing values).
- ✅ Created derived columns for better population and access calculations.
- ✅ Built a new summary sheet: **Global 2020 Report**.
- ✅ Calculated total population, urban shares, and percentage differences with global estimates.
- ✅ Visualized key trends using:
  - 📈 Line charts for population vs urban/rural share
  - 📊 Box-and-whisker plots for access levels
  - 📉 100% stacked bar charts for national, rural, and urban access vs population size
- ✅ Grouped data by income group using pivot tables.
- ✅ Converted income group text labels into numbers for sorted visualizations.

---

## 📈 Key Insights

- The dataset does not cover 100% of the world’s population, but reflects key trends.
- Urban areas tend to have greater access to at least basic services than rural areas.
- As income group increases, access to basic water services increases, while limited/unimproved/surface services decrease.
- Data outliers can distort visualizations and require transformation or aggregation to present meaningful insights.

---

## 🛠️ Tools Used

- Google Sheets
- Pivot Tables
- Data Cleaning (COUNTA, ROUNDUP, FILTER, IF, SWITCH functions)
- Visualization: Line charts, 100% stacked bar charts, candlestick (boxplot)

---

## 📚 Next Step: Part 2

In the next phase, we will transform the data further, apply deeper statistical analysis or modeling, and potentially create dashboards or reports.

Stay tuned!

---

## 👤 Author

**Faissal Elmokaddem**  
Data Science & Engineering Student | [ALX Africa Program 2025]

---

> 📁 This repository is part of the ALX Integrated Project on Access to Drinking Water. Do not copy without permission.
