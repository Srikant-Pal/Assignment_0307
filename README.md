# PE Analyst Assessment – Data Cleaning & Audit

This repository contains a detailed data cleaning and analysis report for a Process Excellence (PE) Analyst assessment. The goal was to identify inconsistencies, missing values, and logical errors in a support ticket dataset provided as an assignment.

##  Objective

To audit a raw ticket dataset and highlight:

- Logical date issues (e.g., resolved before created)
- Inconsistent date formats
- Missing or invalid values
- Conflicts in tagging vs issue identification
- Inconsistent ticket subjects
- Spelling and Grammatical error

## Technologies Used

- Python (pandas, numpy)
- Data Visualization: matplotlib, seaborn
- Jupyter Notebook / Script-based analysis
- Excel

## Key Steps Performed

### 1. Data Cleaning
- Standardized column names (lowercase, underscores)
- Converted string/object date columns to `datetime` type
- Extracted separate `date` and `time` components
- Handled and visualized missing values

### 2. Logical Date Error Check
- Found tickets with resolution date earlier than creation date
- Visualized resolution time in hours (negative = invalid)

### 3. Date Format Inconsistency
- Ticket Create Date: Mix of `YYYY-MM-DD` and `DD/MM/YYYY`
- Ticket Resolved Date: Consistent `DD/MM/YYYY`
- Ticket Assigned Date: `HH:MM:SS DD-MM-YYYY` format (inconsistent) + missing values
- Visualized format counts via bar plots

### 4. Tagging vs Issue Identification Conflict
- Detected 21 rows where tagging and identification disagreed
- Displayed result using a heatmap

### 5. Inconsistent Ticket Subjects
- Identified inconsistent values like `"Other issue"`, `"Others"`, `"Other Issue"`
- Counted and visualized as a bar chart

## Output

All insights were clearly visualized using bar plots and heatmaps for easy interpretation.

##  Files

- `PE Analyst Assessment.ipynb` – Main script for data cleaning and visualization
- Raw dataset file (not uploaded publicly due to confidentiality)

## Final Remarks

This project demonstrates my ability to:
- Perform real-world data cleaning.
- Identify subtle inconsistencies.
- Use Python tools to create clean, insightful visuals.

