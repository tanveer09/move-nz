## Changes in Travel Behaviour to Education and Work in New Zealand (2018–2023)

**Author:** Tanveer Singh
**Institution:** Victoria University of Wellington
**Project Type:** Master of Data Science Research Project
**Industry Context:** NZTA – Insights & Analytics

---

## Project Overview

This project investigates structural changes in travel behaviour in New Zealand between the 2018 and 2023 Census periods, with a comparative focus on:

* **Journey to Education**
* **Journey to Work**

The study evaluates whether:

* Travel mode distributions changed significantly between 2018 and 2023
* Education and Work journeys exhibit different behavioural shifts
* Regional and urbanisation-based differences exist
* The magnitude of change differs between journey types

Statistical analysis includes:

* Pearson Chi-square tests
* Difference-in-Differences (DiD) analysis
* Multinomial logistic regression with Year × Journey interaction
* Subpopulation and regional extensions

---

## Data Sources

Data is derived from:

* **Stats NZ Census 2018 and 2023**
* Journey to Education dataset
* Journey to Work dataset

The repository includes:

```
data/
├── raw/          # Original datasets
├── interim/      # Cleaned but intermediate files
├── processed/    # Final analysis-ready datasets
```

Large datasets are managed using **Git LFS**.

---

## Repository Structure

```
move-nz/
│
├── code/                  # R scripts for full analysis pipeline
├── data/                  # Raw and processed datasets (LFS tracked)
├── dashboards/            # Power BI dashboard (.pbix)
├── figures/               # Figures included in the paper
├── text/
│   └── paper/             # RMarkdown research paper
├── common/                # References, CSL file
├── outputs/               # Statistical outputs & result tables
├── .gitattributes         # Git LFS tracking configuration
└── README.md
```

---

## Statistical Methodology

The analysis is conducted in R and includes:

1. **Distributional Testing**

   * Chi-square tests of homogeneity
   * Tests of independence

2. **Model-Based Assessment**

   * Multinomial logistic regression
   * Year × Journey Type interaction
   * Predicted probability estimation

3. **Difference-in-Differences (DiD)**

   * Mode-specific change magnitude comparison

4. **Regional Extensions**

   * 17-region analysis
   * Urban vs non-urban comparison

---

## Dashboard (Industry Layer)

An interactive Power BI dashboard is included:

```
dashboards/powerbi/
```

The dashboard visualises:

* National mode share changes
* Education vs Work comparison
* Regional DiD results
* Urbanisation-based breakdown
* KPI summaries

To use:

1. Open the `.pbix` file in Power BI Desktop
2. Confirm data source path (relative to `data/processed/`)
3. Refresh

---

## Reproducibility Instructions

To reproduce the full analysis:

### 1️. Requirements

* R ≥ 4.x
* RStudio (recommended)
* Packages:

  * tidyverse
  * nnet
  * broom
  * knitr
  * rmarkdown
  * here (recommended)

### 2️. Reproducing the Analysis
The full statistical analysis is implemented in:
```
code/edu_vs_work.Rmd
```

This RMarkdown file contains:
* Data ingestion and transformation
* Descriptive statistics
* Chi-square testing
* Difference-in-Differences analysis
* Multinomial logistic regression
* Predicted probability estimation
* Figure and table generation
To Reproduce Results
1. Open the repository as an RStudio Project
2. Navigate to:
code/edu_vs_work.Rmd
1. Knit the document
This will regenerate all statistical outputs and figures used in the research paper.

---

## Research Paper
The final paper is located in:

```
text/paper/move_nz_research_paper.Rmd
```

The appendix contains the full analysis code for transparency and academic completeness.
To rebuild the paper:
1. Open paper.Rmd
2. Knit to PDF (XeLaTeX required)

---

## Research Questions

Key questions addressed include:

* Did Education travel modes change significantly between 2018 and 2023?
* Did Work travel modes change significantly?
* Were Education and Work distributions different in each year?
* Is there evidence that the magnitude of change differs by journey type?
* Do regional and urbanisation effects moderate these changes?

---

## Computational Environment

* OS: macOS
* R: [Insert your version]
* LaTeX Engine: XeLaTeX
* Power BI Desktop (latest)

---

## License

All rights reserved.

This repository is made available for academic review and reference purposes only.  
No reuse, modification, or redistribution is permitted without explicit written permission from the author.

---

## Contact

Tanveer Singh
Victoria University of Wellington
Master of Data Science

---

# Notes on Reproducibility

* Large data files are tracked via Git LFS.
* All figures are generated via R code.
* No manual statistical manipulation was performed outside scripts.
* Relative paths are used throughout.

---