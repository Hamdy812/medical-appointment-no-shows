# Medical Appointment No-Shows Analysis

Exploratory data analysis of ~110k medical appointments in Brazil to understand **which factors are associated with patients missing their appointments**.

## Research question
Which factors are associated with a patient booking an appointment and then not showing up?

## Dataset
[Medical Appointment No Shows](https://www.kaggle.com/datasets/joniarroba/noshowappointments) (Kaggle), appointments from April to June 2016.
The CSV file is not included in this repository, download it from Kaggle and place it next to the notebook.

## What this project covers
- **Data cleaning:** duplicates, misspelled column names, a clear target variable, date parsing (including corrupted values), impossible ages, appointments dated before booking
- **Feature engineering:** waiting time, age groups, weekday, patient history (previous no-shows)
- **EDA:** waiting time, age, gender, weekday, SMS reminders, neighbourhoods, chronic conditions, scholarship, handicap
- **Confounding check:** the SMS effect is re-examined inside each waiting-time group
- **Statistical testing:** Chi-square tests with effect sizes (gap in percentage points)
- **Recommendations** for reducing no-shows

## Key findings
> Fill these in from your own results.

- Overall no-show rate: ___%
- Waiting time: ___% (same day) to ___% (30+ days)
- Patients who missed before are ___% likely to miss again, versus ___% for those who never missed
- SMS: ___ (describe the result after controlling for waiting time)

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, SciPy

## How to run
```bash
pip install -r requirements.txt
jupyter notebook project_1_final.ipynb
```
Update the CSV path in the first cells if needed.

## Limitations
Association, not causation. Data covers one region and about three months. No information on visit reason, distance or income.

## Author
Your name, graduation project, your university and year
