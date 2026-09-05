# U.S. Job Market Analysis 📊

### Exploring the relationship between employment, wages, and occupational specialization in the United States

## Overview

Does having more job opportunities mean higher pay?

This project explores that question using **May 2024 Occupational Employment and Wage Statistics (OEWS)** data from the **U.S. Bureau of Labor Statistics**.

I analyzed employment and wage data across U.S. occupations to understand how workforce size relates to compensation and how wage patterns change across different occupational classification levels.

The analysis focuses on three main variables:

* **Employment**
* **Mean Hourly Wage**
* **Mean Annual Wage**

Using Python, I cleaned the raw dataset and created multiple visualizations to explore employment distribution, wage variation, correlations, and the relationship between job availability and income.

---

## The Question

A common assumption about the job market is:

> **More jobs = better opportunities and higher pay.**

But does the data actually support that?

This analysis explores whether occupations with larger workforces tend to have higher wages and what patterns emerge when employment and compensation are analyzed together.

---

## Dataset

**Source:** U.S. Bureau of Labor Statistics (BLS)
**Dataset:** Occupational Employment and Wage Statistics (OEWS)
**Period:** May 2024

The dataset contains employment and wage information for occupations across the United States.

For this analysis, I focused on:

| Variable      | Description                       |
| ------------- | --------------------------------- |
| `occupation`  | Occupation title                  |
| `soc_group`   | Occupational classification level |
| `employment`  | Number of employees               |
| `hourly_mean` | Mean hourly wage                  |
| `annual_mean` | Mean annual wage                  |

---

# Data Cleaning

Before creating visualizations, the raw data needed to be cleaned and prepared.

The data preparation process included:

* Filtering the dataset to include only **U.S. national-level data**
* Removing unnecessary columns
* Renaming variables for readability
* Removing hidden spaces from column names
* Converting employment and wage values to numeric data types
* Removing commas from numerical values
* Handling missing values
* Removing the **"All Occupations"** row to prevent it from distorting the analysis

The cleaned dataset was then used for exploratory data analysis and visualization.

---

# Exploratory Data Analysis

## 1. Which occupations employ the most people?

The first visualization identifies the **top 15 occupations by employment**.

Employment values vary significantly between occupations, so a **logarithmic scale** was used to make comparisons easier and prevent the largest occupations from hiding smaller ones.

**Visualization:** Bar Chart

---

## 2. How do wages vary across occupational groups?

A box plot was used to examine the distribution of annual wages across occupational classification groups.

This helps reveal differences in wage ranges, variation, and potential outliers.

**Visualization:** Box Plot

---

## 3. Does higher employment mean higher pay?

A scatter plot was created to explore the relationship between:

* Employment
* Mean annual wage

Both axes use logarithmic scales because of the large differences in employment and wage values.

**Visualization:** Scatter Plot

---

## 4. What does the overall U.S. wage distribution look like?

A histogram with a density curve was used to examine the distribution of annual mean wages.

The chart also compares the:

* Mean
* Median

This provides insight into the shape and skewness of wage distribution across occupations.

**Visualization:** Histogram + KDE

---

#  Additional Analysis

## Employment Share by SOC Group

A pie chart was used to examine how employment records are distributed across occupational classification groups.

---

## Hourly Wage Distribution

A violin plot was created to visualize the shape, density, and spread of hourly wages across SOC groups.

This provides more information than averages alone and helps identify differences in wage variation.

---

## Correlation Analysis

A correlation heatmap was created to examine relationships between:

* Employment
* Mean hourly wage
* Mean annual wage

The goal was to determine whether workforce size has a strong relationship with compensation.

---

## Employment vs. Annual Wage

A bubble plot combines multiple variables into a single visualization:

* **X-axis:** Employment
* **Y-axis:** Mean annual wage
* **Bubble size:** Employment
* **Color:** SOC group

This visualization provides another perspective on the relationship between occupation size, wages, and occupational classification.

---

#  Key Findings

The analysis revealed several interesting patterns:

### Job availability does not necessarily mean higher pay

Occupations with large employment numbers are not automatically the highest-paying occupations.

###  Wage variation increases with specialization

More detailed occupational classifications reveal a wider range of wages, including highly specialized and high-paying occupations.

###  Employment and wages have a weak relationship

The analysis shows that workforce size alone is not a strong predictor of compensation.

###  The U.S. wage distribution is uneven

Most occupations are concentrated within lower and middle wage ranges, while a relatively small number of highly paid occupations extend the upper end of the distribution.

---

#  Tech Stack

**Language**

* Python

**Data Analysis**

* Pandas
* NumPy

**Data Visualization**

* Matplotlib
* Seaborn

**Environment**

* Google Colab
* Jupyter Notebook

---

#  Repository Structure

```text
us-job-market-analysis/
│
├── national_M2024_dl.csv       # Raw dataset
├── us_job_market_analysis.py   # Python analysis script
├── us_job_market_analysis.ipynb # Jupyter Notebook
└── README.md
```

---

#  Running the Project

### Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### Install dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### Run the Python script

```bash
python us_job_market_analysis.py
```

Or open the `.ipynb` file using:

* Jupyter Notebook
* JupyterLab
* Google Colab

---

# Project Context

This project was completed as part of a **Data Visualization course (DSC 502)** as a collaborative project.

The complete project incorporated multiple data visualization tools, including Python, R, Tableau, and ArcGIS.

### My Contribution

My primary contribution focused on the **Python-based data analysis and visualizations**.

I was responsible for:

* Cleaning and preparing the dataset for Python analysis
* Exploring employment and wage data
* Creating Python visualizations using Matplotlib and Seaborn
* Performing correlation analysis
* Identifying patterns and relationships between employment and wages
* Contributing to the overall interpretation of the results

---

# What I Learned

Through this project, I strengthened my skills in:

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Data visualization
* Statistical interpretation
* Correlation analysis
* Identifying patterns and outliers
* Communicating insights through visual storytelling


