# Miami-Dade 311 Service Requests & Property Crime Analysis

**University of South Florida | Data & Text Mining | Spring 2026**

**Technologies:** R, R Markdown, tidyverse, ggplot2, tidytext, lubridate, readxl

## Project Overview

This group project analyzed **966,645 Miami-Dade County 311 service requests from 2017–2019** alongside county-level property crime statistics to investigate trends in public service requests and reported crime.

The project combined data cleaning, exploratory data analysis, visualization, and text mining to identify frequently reported community issues and compare service-request patterns with property crime trends.

**My Role:** Team Leader — Data & Text Mining

## Research Questions

1. How did 311 service-request volumes change between 2017 and 2019?
2. Which service-request categories were most frequently reported?
3. How did property crime change during the same period?
4. What similarities and differences appeared between service-request and crime trends?
5. Which terms were most prominent in service-request categories and department descriptions?

## Data Sources

- **Miami-Dade County 311 Service Requests:** Records from 2017, 2018, and 2019.
- **Property Crime Data:** Annual county-level property crime workbooks identified in the project as Florida Department of Law Enforcement data.

The original large 311 CSV files are excluded from this repository. The three property crime Excel workbooks and smaller processed summary datasets are included.

See [data documentation](data/README.md) for filenames and additional information.

## Methodology

### 1. Data Preparation

- Imported annual 311 service-request datasets.
- Standardized date and time variables.
- Handled missing issue-description values.
- Combined annual records and filtered the analysis to 2017–2019.
- Aggregated 311 request counts by year and category.
- Joined annual request totals with county-level property crime statistics by year.

### 2. Exploratory Data Analysis

Used R and ggplot2 to visualize:

- The ten most frequent service-request categories.
- Annual 311 service-request totals.
- Property crime trends from 2017–2019.
- Comparisons between 311 request volumes and reported property crime.

### 3. Text Mining

Used tidytext and stringr to analyze the `issue_type` and `case_owner_description` fields.

Techniques included:

- Text normalization and tokenization.
- Stop-word removal.
- Word frequency analysis.
- Comparison of service-request and department terminology.
- TF-IDF analysis to identify terms distinctive to individual years.

### 4. Reporting and Presentation

Produced an R Markdown report incorporating data preparation, statistical summaries, visualizations, findings, and interpretations. The group also presented its analysis and practical implications.

## Key Findings

| Year | 311 Requests | Reported Property Crimes |
|---|---:|---:|
| 2017 | 322,432 | 92,714 |
| 2018 | 325,879 | 86,809 |
| 2019 | 318,334 | 85,543 |
| **Total** | **966,645** | **265,066** |

- **Stable 311 request volume:** Annual service requests remained relatively consistent across the three years.
- **Declining property crime:** Reported property crime fell from 92,714 incidents in 2017 to 85,543 in 2019.
- **Common community concerns:** Bulky trash, green waste carts, recycling, sanitation, and other service-related issues appeared prominently in 311 records.
- **Text-mining insights:** Word frequency and TF-IDF analyses highlighted prominent service categories and differences in terminology across years and departments.

The analysis is descriptive and does not establish a causal relationship between 311 requests and property crime.

## Repository Structure

| File or Folder | Description |
|---|---|
| `Final_Project_3.Rmd` | R Markdown analysis and source code |
| `Final_Project_3.html` | Rendered report with results and visualizations |
| `data/` | Property crime Excel files and data documentation |
| `output/311_issue_counts.csv` | Counts of service-request categories |
| `output/311_issue_by_year.csv` | Service-request categories summarized by year |
| `output/crime_311_merged.csv` | Annual 311 totals joined with property crime figures |
| `presentation/` | Final team PowerPoint presentation |

## Reproducing the Analysis

1. Download or clone this repository.
2. Obtain the original three Miami-Dade 311 CSV files for 2017, 2018, and 2019, and place them in the `data/` folder using the filenames listed in the data documentation.
3. Open the repository folder in RStudio.
4. Install the required R packages: `rmarkdown`, `tidyverse`, `lubridate`, `readxl`, `tidytext`, `stringr`, `ggplot2`, and `scales`.
5. Open `Final_Project_3.Rmd` and knit the report to HTML.

**Reproducibility note:** The R Markdown analysis was successfully knitted to HTML in RStudio using the original source datasets stored locally. The large 311 CSV files are excluded from GitHub due to their size.

## Project Team

This project was completed collaboratively at the University of South Florida.

- **Zara Gonzalez** — Team Leader
- Johnny Nguyen
- Elston Miller
- Nicholas Alex
- Wesley Huang

## Limitations

The analysis covers only three years of county-level data. Annual trend comparisons do not account for potential confounding factors or establish causation. Text mining focuses on recorded issue categories and department descriptions rather than the full narrative content of individual complaints.

## Author

**Zara Gonzalez**

University of South Florida — Information Science, Data Science & Analytics

[GitHub](https://github.com/zaragz) | [LinkedIn](https://www.linkedin.com/in/zaragonzalez)
