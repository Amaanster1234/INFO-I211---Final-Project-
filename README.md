# Diabetes Health Indicators Analysis

## Overview

This project analyzes a large-scale public health dataset to explore the relationships between lifestyle, medical, and demographic factors and diabetes status. Using Python and several data analysis libraries, we perform data cleaning, exploratory analysis, statistical testing, and machine learning to identify key patterns and predictive relationships.

The goal of this project is to determine which factors are most strongly associated with diabetes and whether diabetes status can be predicted using these variables.

---

## Dataset

The dataset used in this project is the **Diabetes Health Indicators dataset** obtained from Kaggle. It originates from the **CDC Behavioral Risk Factor Surveillance System (BRFSS)**, a nationwide survey conducted in the United States.

* Over 200,000 observations
* 20+ variables
* Includes:

  * Health conditions (BMI, blood pressure, cholesterol)
  * Lifestyle behaviors (physical activity, smoking)
  * Demographics (age, sex, income, education)
  * Diabetes status (0 = No Diabetes, 1 = Prediabetes, 2 = Diabetes)

---

## Project Structure

```
INFO-I211---Final-Project--main/
│
├── data/
│   └── diabetes_012_health_indicators_BRFSS2015.csv
│
├── outputs/
│   ├── cleaned_data/
│   │   └── diabetes_cleaned.csv
│   ├── figures/
│   ├── tables/
│
├── final_project.ipynb
├── README.md
```

---

## Libraries Used

This project uses the following Python libraries:

* os (file and directory management)
* pandas (data manipulation and analysis)
* numpy (numerical operations)
* matplotlib (data visualization)
* seaborn (statistical visualization)
* scipy (statistical analysis)
* scikit-learn (machine learning)

---

## Methodology

### 1. Data Cleaning

* Loaded dataset using pandas
* Renamed columns for readability
* Removed duplicate rows
* Checked for missing values
* Saved cleaned dataset for reuse

---

### 2. Exploratory Data Analysis (EDA)

* Generated summary statistics
* Visualized distributions of key variables
* Created:

  * Count plots (diabetes distribution)
  * Boxplots (BMI vs diabetes)
  * Bar charts (health and demographic factors)
  * Correlation heatmap
* Identified patterns between variables and diabetes status

---

### 3. Statistical Analysis

* Performed hypothesis testing using scipy:

  * T-tests for comparing group means
  * ANOVA for comparing BMI across all diabetes groups
  * Chi-square tests for categorical variables
  * Pearson correlation for continuous relationships
* Determined statistical significance of relationships

---

### 4. Machine Learning

* Built a Logistic Regression model
* Used train/test split
* Predicted diabetes status using health indicators
* Evaluated model using:

  * Accuracy
  * Classification report
  * Confusion matrix

---

### 5. Final Results

* Identified key factors associated with diabetes:

  * Higher BMI is strongly associated with diabetes
  * Physical activity is associated with lower diabetes risk
  * High blood pressure and cholesterol are significant indicators
* Machine learning model confirmed predictive capability

---

## Key Findings

* BMI increases with diabetes severity
* Physical inactivity is linked to higher diabetes prevalence
* High blood pressure and cholesterol are strongly associated with diabetes
* Demographic factors (age, income, education) show meaningful differences
* Diabetes status can be predicted with reasonable accuracy using health indicators

---

## Limitations

* Data is self-reported and may contain bias
* Correlation does not imply causation
* Dataset may be imbalanced across classes
* Limited feature interactions explored

---

## Future Work

* Use more advanced machine learning models
* Perform feature engineering
* Explore longitudinal or time-based data
* Improve prediction accuracy with additional variables

---

## How to Run the Project

1. Clone the repository
2. Ensure the dataset is located in the `data/` folder
3. Open `final_project.ipynb`
4. Run all cells from top to bottom

---

## Authors

* Amaan Sadiq - (Section 1 and Combined all Code)
* Sebastian Quebrado-Segura (Section 2)
* Yusuf Omar (Section 4)
* Abdul Djama (Section 3)
* All commits and pushes were performed by Amaan to keep the repository organized and prevent confusion. Individual code was written and sent to Amaan to upload 

---

## Conclusion

This project demonstrates how Python can be used to analyze large-scale health data and uncover meaningful patterns. The results highlight the importance of lifestyle and health conditions in understanding diabetes and show that data-driven approaches can support public health insights.
