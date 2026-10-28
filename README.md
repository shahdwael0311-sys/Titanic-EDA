# Titanic Exploratory Data Analysis (EDA)

## Project Overview

This project explores the Titanic passenger dataset using Python to understand passenger characteristics, assess data quality, and investigate patterns associated with survival.

## Objectives

- Inspect dataset structure and data types.
- Identify and handle missing values.
- Generate descriptive statistics.
- Compare survival rates by sex, passenger class, and age group.
- Visualize survival patterns using bar plots and heatmaps.
- Examine correlations between selected numerical variables.
- Communicate findings and analytical limitations.

## Tools and Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

```text
Titanic-EDA/
├── titanic_eda.ipynb
├── train.csv
├── README.md
├── requirements.txt
└── screenshots/
```

## Analysis Workflow

1. Load and inspect the dataset.
2. Examine data types, missing values, and duplicate records.
3. Clean selected columns and validate the results.
4. Generate descriptive statistics.
5. Compare survival rates across passenger groups.
6. Create visualizations and a correlation heatmap.
7. Summarize findings, limitations, and conclusions.

## Key Findings

- **Overall survival:** 38.38% of passengers survived (342 out of 891).
- **Survival by sex:** Female passengers had a survival rate of 74.20%, compared with 18.89% for male passengers.
- **Survival by passenger class:** First-class passengers had the highest survival rate (62.96%), followed by second class (47.28%) and third class (24.24%).
- **Survival by sex and class:** First-class females had the highest survival rate (96.81%), while third-class males had the lowest (13.54%).
- **Survival by age:** Passengers aged 0–12 had a survival rate of 57.97%, while passengers aged 61 and above had the lowest rate at 22.73%.
- **Correlation analysis:** Passenger class had the strongest numerical correlation with survival (-0.338), followed by fare (0.257). Higher passenger-class numbers were associated with lower survival rates.
- **Data quality:** Missing ages were filled using the median, missing embarkation ports using the mode, and the `Cabin` column was excluded because approximately 77% of its values were missing. The cleaned dataset contained 891 rows and 9 columns, with no remaining missing values.

## How to Run

1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

4. Ensure `train.csv` is in the project root directory.
5. Open `titanic_eda.ipynb` in Jupyter Notebook or VS Code.
6. Select the project's Python environment and run all cells.

## Limitations

- Missing ages and embarkation ports were imputed using the median and mode, respectively.
- The `Cabin` column was excluded due to substantial missingness, potentially removing useful information.
- Median imputation may create an artificial concentration around the median age.
- The analysis describes the available dataset and should not be generalized beyond its scope.
- Correlations indicate associations, not causation, and variables such as sex, age, passenger class, and fare may overlap in their relationship with survival.

## Conclusion

This exploratory analysis identified differences in survival rates across passenger demographics and ticket classes. Female passengers and first-class passengers had substantially higher survival rates, while passenger class showed the strongest numerical correlation with survival. Further statistical testing or predictive modeling could investigate these relationships in greater depth.

## Data Source

Kaggle — Titanic: Machine Learning from Disaster

https://www.kaggle.com/competitions/titanic/data
