# Student Performance Analysis

Data cleaning and preprocessing for student academic performance data. Prepares the raw dataset for analysis or modeling.

## What it does

- Loads student performance CSV data
- Validates data types and checks for missing values
- Standardizes categorical columns (gender, ethnicity, education level, etc.)
- Calculates composite scores (average and total)
- Outputs cleaned dataset for downstream analysis

## Setup

```
pip install pandas numpy
```

## How to use

1. Update the file path to point to your `StudentsPerformance_Preprocessed.csv`
2. Run cells from top to bottom
3. Cleaned data gets saved back to CSV

## Data flow

**Input:** Raw student performance CSV  
**Processing:**
- Data type inspection
- Null value checking
- Categorical formatting (title case, stripped whitespace)
- Score aggregation

**Output:** Cleaned CSV with new calculated columns

## What you get

After running:
- `average_score` - Mean of math, reading, and writing scores
- `total_score` - Sum of all three test scores
- Properly formatted categorical columns
- Data quality report (nulls, dtypes, row count)

## Expected columns

- gender
- race/ethnicity
- parental level of education
- lunch (type)
- test preparation course
- math score
- reading score
- writing score

## Notes

- The script is idempotent - safe to run multiple times
- Categorical columns get stripped of extra whitespace and title-cased
- If your CSV path differs, update it in cell 1
- Output overwrites the same file - back up your data first if needed

## Common issues

**FileNotFoundError:** Check the file path in the data loading cell matches your actual file location

**KeyError:** Make sure all expected columns exist in your CSV with exact names

**Unexpected values:** Run `df.head()` and `df.describe()` to inspect raw data before processing
