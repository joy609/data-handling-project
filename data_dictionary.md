# Data Dictionary

This document describes the columns in the student-performance dataset.

| Column | Description | Data type | Validation |
|---|---|---|---|
| `student_id` | Unique identifier for a student | Text | Should not be missing; investigate repeated IDs |
| `name` | Student's name | Text | Should not be blank |
| `gender` | Recorded gender category | Text | Standardized spacing and capitalization |
| `attendance_percent` | Student attendance percentage | Numeric | Expected range: 0–100 |
| `study_hours` | Hours spent studying | Numeric | Must be non-negative |
| `score` | Student's recorded score | Numeric | Must follow the official scoring range |
| `attendance_flag` | Indicates attendance outside the expected range | Boolean | `True` means the attendance needs review |

## Missing and Invalid Values

Missing values are retained when the correct value cannot be verified. Invalid numeric text, such as `abc` in the score column, is converted to a missing numeric value.

## Limitations

The dataset is a small sample for learning purposes. Suspicious attendance and missing values should be verified before the data is used for real decisions.
