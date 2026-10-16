# Miami-Dade 311 Service Requests & Property Crime Analysis

**R | Data Cleaning | Exploratory Data Analysis | Text Mining | ggplot2 | tidytext**

## Overview

This group project examined Miami-Dade County 311 service requests from **2017–2019** alongside property-crime data to explore patterns in resident-reported concerns and crime trends. The analysis involved approximately **960,000+ service-request records** and combined structured-data analysis with text mining of complaint descriptions.

**Role:** Team Leader — Data & Text Mining Project, University of South Florida (March–April 2026)

## Research focus

- How did 311 service-request volumes and property-crime trends change during 2017–2019?
- Which types of requests appeared most frequently?
- What themes could be identified in complaint descriptions through text mining?

The comparison is descriptive; it does not establish that 311 requests caused changes in crime or vice versa.

## Methods

1. **Data preparation:** standardized date formats, identified or removed duplicates, and combined annual service-request data with property-crime data.
2. **Exploratory analysis:** summarized annual activity, compared request types and crime trends, and created visualizations using `ggplot2`.
3. **Text mining:** tokenized complaint text, removed stop words, calculated word frequencies, and used TF-IDF to identify informative terms with `tidytext`.
4. **Reporting:** documented analysis and visualizations in an R Markdown report and presented findings to an audience.

## Main observation

The project observed declining property-crime totals over the period examined, while 311 complaint volumes appeared comparatively stable. This motivates further investigation; it should not be interpreted as evidence of a causal relationship.

## Repository guide

| Path | Contents |
| --- | --- |
| `Final_Project_3.Rmd` | Main analysis and report source (R Markdown) |
| `Final_Project_3.html` | Rendered report, if included |
| `output/311_issue_by_year.csv` | Summary of 311 issues by year, if included |
| `output/311_issue_counts.csv` | Summary of request-category counts, if included |
| `presentation/` | Final presentation slides, if included |
| `data/README.md` | Input-data descriptions and access notes |

The complete raw datasets, large intermediate files, and saved R workspace are **not** included in this public repository.

## Reproducing the work

1. Obtain the original 2017–2019 311 datasets and corresponding property-crime datasets from their official sources. See [`data/README.md`](data/README.md).
2. Place the input files in a local `data/` folder. Confirm that the file names and column layouts match those expected by `Final_Project_3.Rmd`.
3. Open `Final_Project_3.Rmd` in RStudio and install the R packages required by its `library()` calls (including packages used for plotting and text analysis).
4. Check file paths in the report, preferably making them relative to the project folder, and run or knit the report.

**Reproducibility note:** These instructions describe the intended workflow. The report has not yet been verified to run end-to-end from a clean checkout without the omitted input datasets. Update this section after testing.

## Credits

This was a collaborative university project. Zara Gonzalez served as team leader. Additional team-member acknowledgments and precise data-source citations can be added after confirmation.
