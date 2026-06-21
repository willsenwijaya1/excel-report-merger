# Excel Report Merger

A Streamlit application that automates the extraction, cleaning, and consolidation of multiple Excel reports into a single dataset.

This project was developed to solve a recurring reporting problem where operational reports from different periods needed to be manually cleaned and combined. The application automatically identifies the table header, removes unnecessary summary rows, extracts the reporting period, and merges all files into a single Excel file.

## Features

- 📂 Upload multiple Excel files simultaneously.
- 🔍 Automatically detect the table header.
- 🧹 Remove unnecessary summary rows.
- 📅 Extract reporting period information.
- 📊 Merge all reports into one dataset.
- 📥 Export the consolidated data to Excel.

---

## Business Problem

Operational reports often come in separate Excel files and contain:

- Headers located in different rows.
- Summary information that is not needed for analysis.
- Data spread across multiple reporting periods.

Manually combining these files is repetitive, time-consuming, and prone to human error.

This application automates the entire process and produces a clean dataset ready for analysis.

---

## Tech Stack

- Python
- Streamlit
- Pandas
- XlsxWriter
- OpenPyXL

## How It Works

### Step 1
Upload multiple Excel reports.

### Step 2
Automatically locate the table header by searching for:

```text
Download
```

### Step 3
Remove unnecessary summary rows such as:

- RESPONSE RATE
- PASSED RESPONSE RATE
- FAILED RESPONSE RATE
- ABANDONES RATE

### Step 4
Extract the reporting period from each file.

### Step 5
Add the reporting period as a new column.

### Step 6
Merge all reports into a single dataset.

### Step 7
Download the consolidated Excel file.

---

## Workflow

```text
Multiple Excel Files
          ↓
   Header Detection
          ↓
      Data Cleaning
          ↓
   Period Extraction
          ↓
     Data Consolidation
          ↓
      Excel Export

## Key Features

### Automatic Header Detection
The application can identify the beginning of the data table even when the header position changes between files.

### Data Cleaning
Removes unnecessary rows that are not part of the dataset.

### Period Extraction
Automatically retrieves the reporting period from each report.

### Data Consolidation
Combines multiple reports into one structured dataset.

---

## Use Cases

This application can be used for:

- Customer service reporting
- Operational reporting
- KPI monitoring
- Monthly report consolidation
- Data preparation for dashboards
- ETL and reporting automation

---

## Future Improvements

- Support additional report templates.
- Automatic column mapping.
- Scheduled processing.
- Database integration.
- Data validation checks.
- Dashboard integration.
- Cloud deployment.

---

## Author

**Willsen Wijaya**
