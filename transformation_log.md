# Data Cleaning Transformation Log

## Project
B5: Data Handling with Python — Student Performance Dataset

## Objective
To inspect, clean, validate, and document a student-performance dataset while preserving the original raw data.

## Transformations Performed

| Issue | Action Taken | Reason |
|---|---|---|
| Inconsistent gender formatting | Removed leading/trailing spaces and standardized capitalization | Improve consistency |
| Numeric columns stored as text | Converted attendance, study hours, and scores to numeric types | Enable valid analysis |
| Invalid score value (`abc`) | Converted to a missing value and retained for review | Avoid inventing a score |
| Exact duplicate row | Removed from the working copy | Prevent duplicate records from affecting analysis |
| Attendance above 100% | Flagged for investigation without changing the value | Preserve the original value until verified |
| Missing attendance | Retained as missing | Correct value is unknown |
| Missing study hours | Retained as missing | Correct value is unknown |

## Data Preservation
The original CSV file was retained in `data/raw/`. Cleaning operations were performed on a separate working copy.

## Output Files
- `data/cleaned/student_performance_cleaned.csv`
- `outputs/before_data_profile.csv`
- `outputs/after_data_profile.csv`

## Limitations
The dataset is a small sample. Missing values and invalid attendance require verification before the dataset is used for substantive student-performance analysis.

## Reproducibility
The cleaning workflow and transformations are documented in `data_cleaning.ipynb`.
