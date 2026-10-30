# Student Performance Data Cleaning

## Project Overview

This project demonstrates how Python and Pandas can be used to inspect, clean, validate, and document a student-performance dataset.

The sample dataset contains missing values, duplicate records, inconsistent gender formatting, invalid numeric text, and an attendance value outside the expected range.

## Project Objectives

- Inspect and profile the raw dataset.
- Identify missing values and duplicate records.
- Standardize inconsistent text.
- Convert numeric columns to suitable data types.
- Flag invalid attendance values for review.
- Export the cleaned dataset.
- Generate before-and-after data profiles.
- Document cleaning decisions and limitations.

## Project Structure

```text
data-handling/
├── data/
│   ├── raw/
│   │   └── student_performance_raw.csv
│   └── cleaned/
│       └── student_performance_cleaned.csv
├── outputs/
│   ├── before_data_profile.csv
│   └── after_data_profile.csv
├── data_cleaning.ipynb
├── data_dictionary.md
├── transformation_log.md
├── reproducibility_checklist.md
├── README.md
├── requirements.txt
└── .gitignore
```

## Technologies

- Python
- Pandas
- Jupyter Notebook
- Matplotlib
- Seaborn

## How to Run

1. Install Python.
2. Open a terminal in the project folder.
3. Create a virtual environment:

   `python -m venv .venv`

4. Activate it in Windows PowerShell:

   `.\.venv\Scripts\Activate.ps1`

5. Install the dependencies:

   `python -m pip install -r requirements.txt`

6. Open `data_cleaning.ipynb` in VS Code.
7. Select the project's `.venv` Python kernel.
8. Run the notebook cells in order.

## Outputs

- `data/cleaned/student_performance_cleaned.csv`
- `outputs/before_data_profile.csv`
- `outputs/after_data_profile.csv`

## Data Quality and Limitations

The original raw dataset is retained separately. Cleaning is performed on a working copy. Missing values are not filled with invented information, and invalid attendance values are flagged for verification.

This is a small educational sample and should not be used for real student-performance decisions.
