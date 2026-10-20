# Data Sources and Documentation

This folder contains data used in the Miami-Dade 311 Service Requests and Property Crime Analysis (2017–2019).

## Data Sources

### Miami-Dade County 311 Service Requests

The project analyzed 311 non-emergency service-request records from 2017, 2018, and 2019.

The original CSV files are not included because of their size.

**Required local files:**

- `311_Service_Requests_-_Miami-Dade_County_-_2017.csv`
- `311_Service_Requests_-_Miami-Dade_County_-_2018.csv`
- `311_Service_Requests_-_Miami-Dade_County_-_2019.csv`

These files must be placed in the `data/` folder to reproduce the full analysis.

### Property Crime Data

The following Excel files are included in this repository:

- `PROPERTY_17.xlsx`
- `Property-Crime-County-Type-2018.xlsx`
- `Property-Crime-County-Type-2019.xlsx`

These workbooks contain annual property crime statistics used to extract Miami-Dade County data.

The project documentation identifies the property crime source as the Florida Department of Law Enforcement.

## Processed Data

Smaller processed outputs are available in the repository's `output/` folder:

- `311_issue_counts.csv` — Request counts by issue category.
- `311_issue_by_year.csv` — Request counts by year and issue category.
- `crime_311_merged.csv` — Annual service-request totals and property crime statistics.

The full cleaned 311 dataset is excluded because of its size.

## Reproducibility Notes

The original large 311 CSV files are required to rerun the analysis from the beginning. The R Markdown code contains the transformation and analysis steps.

Exact official dataset download URLs, licensing details, and access dates should be verified and added here.

The project uses historical public datasets for educational analysis. Any additional data should be reviewed for sensitive or identifying information before public release.
