# Student Performance Indicator EDA

**Author:** Kareeb Sadab  
**Date:** 2026-03-03  

---

## Overview
This project performs an **Exploratory Data Analysis (EDA)** on a dataset of student performance indicators.  
The goal is to understand how various factors impact academic outcomes and provide insights for educators and institutions.

Key objectives:
- Analyze student demographics and test scores.
- Explore the effect of gender, race/ethnicity, parental education, lunch type, and test preparation course.
- Visualize data trends and identify patterns affecting performance.

---

## Life Cycle of the Project
1. Understanding the Problem Statement  
2. Data Collection  
3. Data Checks & Cleaning  
4. Exploratory Data Analysis (EDA)  
5. Data Pre-processing  
6. Model Training (Optional)  
7. Choosing the Best Model (Optional)

---

## 1️⃣ Problem Statement
Investigate how student performance (math, reading, writing scores) is affected by:

- Gender  
- Race/Ethnicity  
- Parental level of education  
- Lunch type  
- Test preparation course  

---

## 2️⃣ Data Collection
**Dataset Source:** [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977)  

- 1000 rows, 8 columns  
- Columns: `gender`, `race/ethnicity`, `parental level of education`, `lunch`, `test preparation course`, `math score`, `reading score`, `writing score`

---

## 3️⃣ Data Checks & Cleaning
Performed checks for:
- Missing values → None  
- Duplicates → None  
- Data types and unique values  
- Summary statistics  

**Insights:**
- Average scores close across subjects (~66–68)  
- Standard deviations similar (~14–15)  
- Math scores lowest; Reading scores highest  
- Worst performance in Math, best in Reading  

---

## 4️⃣ Exploratory Data Analysis (EDA)

### 4.1 Score Distributions
- Histograms & KDE plots for `average` and `total score`  
- Females perform better overall  
- Standard lunch correlates with better scores  

### 4.2 Feature Analysis

#### Gender
- Balanced dataset: Female 48%, Male 52%  
- Females have higher overall scores; males score higher in Math  

#### Race/Ethnicity
- Most students belong to Group C and D  
- Group E students score highest, Group A lowest  

#### Parental Education
- Higher parental education correlates with better student scores, especially for male students  

#### Lunch
- Standard lunch students perform better  

#### Test Preparation Course
- Course completion positively impacts scores across subjects  

### 4.3 Visualizations
- Univariate: Countplots, Pie charts  
- Bivariate: Barplots comparing features and performance  
- Multivariate: Pairplots, Violin plots, KDE plots  
- Outliers checked using Boxplots  

---

## 5️⃣ Key Insights
- Performance influenced by lunch type, race/ethnicity, parental education  
- Females lead in pass percentage and top scores  
- Test preparation benefits students but impact is moderate  
- Math is the subject with lowest performance; Reading highest  

---

## 6️⃣ Tools & Technologies
- Python 3.x  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Jupyter Notebook  
