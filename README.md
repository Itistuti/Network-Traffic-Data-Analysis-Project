

## Overview

This project analyzes a dataset (`ids.csv`) using Python and common data science libraries. It focuses on data preparation, cleaning, descriptive statistics, correlation analysis, visualization, and hypothesis testing to understand differences between Normal Traffic and Attack classes.
This work was completed as part of a **coursework assignment and learning exercise** to strengthen practical skills in data analysis using Python, pandas, and statistical methods.

## Objectives
* Load and inspect data in a pandas DataFrame
* Select relevant columns for analysis
* Handle missing values and duplicate records
* Rename label categories for clarity
* Compute summary statistics (mean, standard deviation, skewness, kurtosis)
* Compute correlation matrix and identify key feature relationships
* Explore label distribution and feature behavior using visualizations
* Perform hypothesis testing on Flow Duration between classes

## Tech Stack
* Python
* pandas
* numpy
* matplotlib
* seaborn
* scipy

## Dataset
* Input file: `ids.csv`
* Key features include:

  * Destination Port
  * Flow Duration
  * Total Forward/Backward Packets
  * Packet Length metrics
  * Flow Bytes/s, Flow Packets/s
  * Active Mean, Idle Mean
  * Label

## Workflow Summary

### 1. Data Preparation

* Load dataset using pandas
* Display last 50 rows
* Select relevant subset of columns for analysis

### 2. Data Cleaning

* Check for missing values
* Remove duplicate records if present

### 3. Data Transformation

* Rename label categories:

  * `BENIGN` → Normal Traffic
  * `Infiltration` → Attack

### 4. Analysis

* Compute descriptive statistics (mean, std, skewness, kurtosis)
* Generate correlation matrix
* Identify top correlated features

### 5. Exploration & Visualization

* Bar chart: Label distribution
* Pie charts:

  * Average Flow Duration by label
  * Average Packet Length Mean by label
* Boxplot: Fwd Packet Length Mean by label

### 6. Hypothesis Testing

* Independent t-test on Flow Duration between:

  * Normal Traffic
  * Attack

## Key Findings

* The dataset is slightly imbalanced, with more Normal Traffic than Attack samples
* Average Flow Duration is slightly higher for Normal Traffic
* Average Packet Length Mean is slightly higher for Attack
* Boxplot shows substantial overlap between classes
* The t-test indicates no statistically significant difference in Flow Duration (p > 0.05)

## Note

This project was completed as part of coursework and used as a learning exercise to practice data analysis, visualization, and statistical testing in Python.
