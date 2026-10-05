# Changes in Travel Behaviour to Education and Work in New Zealand (2018–2023)

A comparative analysis of New Zealand Census **Journey to Education** and **Journey to Work** data, examining changes in travel behaviour between 2018 and 2023 through statistical analysis and interactive Power BI visualisation.

**Author:** Tanveer Singh  
**Institution:** Victoria University of Wellington  
**Industry Partner:** NZ Transport Agency Waka Kotahi (NZTA)  
**Project:** Master of Data Science Research Project

---

## Project Resources

- 📊 [Interactive Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTBkMzI5OTgtZjEzNC00NzBjLWJiZDktY2ZiNTg3ZTU4MDk3IiwidCI6IjE3NzQzZjRkLTlkZDItNDk0NC1hNGE1LTYyNWMxNzMzMGNhYSJ9)
- 📄 [Final Research Paper](text/paper/move_nz_research_paper.pdf)
- 📈 [Statistical Analysis](code/edu_vs_work.Rmd)
- 🏢 [NZTA Research Presentation](presentations/nzta/Journey%20to%20Education%20vs%20Journey%20to%20Work%20-%20NZTA%20Presentation.pdf)
- 🎓 [NZTA Internship Presentation](presentations/university/NZTA%20Internship%20Presentation.pdf)
- 🎓 [Research Proposal Presentation](presentations/university/Research%20Proposal%20Presentation.pdf)

---

## Project Overview

This project investigates changes in travel behaviour in New Zealand between the **2018 and 2023 Census periods**, with a primary focus on Journey to Education and comparison with Journey to Work.

The research examines whether:

- Travel mode distributions changed significantly between 2018 and 2023.
- Education and Work journeys experienced different behavioural shifts.
- The magnitude and direction of change differed between journey types.
- Changes varied geographically and across demographic groups.

The project combines **statistical analysis in R** with an **interactive Power BI dashboard** to provide both analytical evidence and accessible visual exploration of the results.

---

## Research Questions

The research addresses five primary questions:

1. Did the distribution of Journey to Education travel modes change between 2018 and 2023?
2. Did the distribution of Journey to Work travel modes change between 2018 and 2023?
3. Did Journey to Education and Journey to Work have different travel-mode distributions in 2018?
4. Did Journey to Education and Journey to Work have different travel-mode distributions in 2023?
5. Did Education and Work travel behaviour change differently between 2018 and 2023?

Additional analysis explores differences by **region, urbanisation, age group and gender**.

---

## Data Sources

The analysis uses publicly available **Stats NZ 2018 and 2023 Census** data:

- **Journey to Education:** Main means of travel to education, age and gender.
- **Journey to Work:** Main means of travel to work, total personal income, age and gender.

The original travel modes were harmonised into five common categories to enable comparison:

- **At Home**
- **Private Transport**
- **Public Transport**
- **Active Transport**
- **Other Transport**

Analysis is conducted at national and subnational levels, including regional and demographic comparisons.

Large datasets in the repository are managed using **Git LFS**.

---

## Statistical Methodology

The statistical analysis was conducted in **R** and includes:

### Chi-Square Analysis

Pearson Chi-square tests were used to assess changes in travel-mode distributions between Census years and differences between Journey to Education and Journey to Work.

### Difference-in-Differences

Mode-specific percentage-point changes between 2018 and 2023 were calculated for Education and Work.

A Difference-in-Differences comparison was then used to quantify how the magnitude of change differed between the two journey types.

### Multinomial Logistic Regression

A multinomial logistic regression model incorporating a **Year × Journey Type interaction** was used to test whether Education and Work travel behaviour changed differently between 2018 and 2023.

### Geographic and Demographic Extensions

Additional analysis examines variation across:

- Regions
- Urban and non-urban areas
- Age groups
- Gender

---

## Key Findings

The analysis identified significant changes in travel behaviour between 2018 and 2023.

- **At Home increased for both Education and Work**, with the increase substantially larger for Journey to Work.
- **Private Transport changed differently across the two journey types**, increasing slightly for Education while declining for Work.
- **Public and Active Transport shares declined nationally**, although the magnitude of change varied geographically and between journey types.
- Statistical testing found significant differences in travel-mode distributions between Census years and between Education and Work.
- The **Year × Journey Type interaction was statistically significant**, providing evidence that Education and Work travel behaviour changed differently between 2018 and 2023.
- Geographic and demographic analysis showed that these changes were not uniform across New Zealand.

Detailed results are available in the [research paper](text/paper/move_nz_research_paper.pdf) and [interactive Power BI dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTBkMzI5OTgtZjEzNC00NzBjLWJiZDktY2ZiNTg3ZTU4MDk3IiwidCI6IjE3NzQzZjRkLTlkZDItNDk0NC1hNGE1LTYyNWMxNzMzMGNhYSJ9).

---

## Interactive Power BI Dashboard

An interactive Power BI dashboard was developed to make the results accessible for exploration and comparison.

The dashboard includes:

- National travel-mode shares for 2018 and 2023
- Journey to Education analysis
- Journey to Work analysis
- Education vs Work comparisons
- Percentage-point changes
- Difference-in-Differences indicators
- Regional comparisons
- Urban vs non-urban analysis
- Age-group and gender analysis
- Mode-specific analysis and insight pages

### View the Dashboard

**[Open the Interactive Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTBkMzI5OTgtZjEzNC00NzBjLWJiZDktY2ZiNTg3ZTU4MDk3IiwidCI6IjE3NzQzZjRkLTlkZDItNDk0NC1hNGE1LTYyNWMxNzMzMGNhYSJ9)**

The Power BI source file and PDF export are available in:

```text
dashboards/powerbi/
├── MoveNZ_Edu_Work_Dashboard.pbix
└── MoveNZ_Edu_Work_Dashboard.pdf
```

---

## Research Paper

The final Master's research paper and its RMarkdown source are available under:

```text
text/paper/
├── move_nz_research_paper.pdf
└── move_nz_research_paper.Rmd
```

- **[View the Final Research Paper](text/paper/move_nz_research_paper.pdf)**
- **[View the RMarkdown Source](text/paper/move_nz_research_paper.Rmd)**

The RMarkdown source provides the reproducible workflow used to generate the research paper.

---

## Presentations

The repository includes presentations produced at different stages of the internship and research project.

### University Presentations

**[NZTA Internship Presentation](presentations/university/NZTA%20Internship%20Presentation.pdf)**  
Presentation delivered following the NZTA internship, covering the internship experience, work undertaken, key learnings and project outcomes.

**[Research Proposal Presentation](presentations/university/Research%20Proposal%20Presentation.pdf)**  
University presentation outlining the research motivation, research questions, data, methodology and proposed analysis.

### NZTA Presentation

**[Journey to Education vs Journey to Work – NZTA Presentation](presentations/nzta/Journey%20to%20Education%20vs%20Journey%20to%20Work%20-%20NZTA%20Presentation.pdf)**  
Presentation of the completed analysis, research findings and interactive Power BI dashboard to NZTA.

---

## Repository Structure

```text
move-nz/
│
├── code/
│   ├── edu_vs_work.Rmd
│   └── edu_vs_work.pdf
│
├── common/
│   ├── apa.csl
│   └── references.bib
│
├── dashboards/
│   └── powerbi/
│       ├── MoveNZ_Edu_Work_Dashboard.pbix
│       └── MoveNZ_Edu_Work_Dashboard.pdf
│
├── data/
│   ├── raw/
│   │   ├── education/
│   │   └── work/
│   ├── interim/
│   ├── transformed/
│   └── edu_work/
│
├── presentations/
│   ├── university/
│   │   ├── NZTA Internship Presentation.pdf
│   │   └── Research Proposal Presentation.pdf
│   └── nzta/
│       └── Journey to Education vs Journey to Work - NZTA Presentation.pdf
│
├── text/
│   └── paper/
│       ├── move_nz_research_paper.Rmd
│       └── move_nz_research_paper.pdf
│
├── .gitattributes
├── .gitignore
├── LICENSE
└── README.md
```

---

## Reproducibility

### Requirements

The analysis was developed using:

- **R 4.4.3**
- RStudio
- XeLaTeX
- Power BI Desktop

Key R packages include:

- `dplyr`
- `tidyr`
- `ggplot2`
- `readr`
- `purrr`
- `janitor`
- `nnet`
- `rcompanion`
- `broom`
- `knitr`
- `kableExtra`
- `pander`

### Reproducing the Statistical Analysis

The main statistical analysis is implemented in:

```text
code/edu_vs_work.Rmd
```

This file contains the workflow for:

- Data ingestion and transformation
- Descriptive analysis
- Chi-square testing
- Difference-in-Differences analysis
- Multinomial logistic regression
- Subgroup and regional analysis
- Figure and table generation

To reproduce the analysis:

1. Clone or download the repository.
2. Open the project in RStudio.
3. Install the required R packages.
4. Open `code/edu_vs_work.Rmd`.
5. Confirm the required data files are available.
6. Knit the RMarkdown document.

### Rebuilding the Research Paper

To regenerate the research paper:

1. Open `text/paper/move_nz_research_paper.Rmd`.
2. Ensure the required R packages and XeLaTeX are installed.
3. Knit the document to PDF.

---

## Tools and Technologies

- **R / RStudio** – data preparation, statistical analysis and modelling
- **RMarkdown** – reproducible analysis and research-paper generation
- **Power BI** – interactive dashboard development and data visualisation
- **DAX** – dashboard measures, percentage-point changes and Difference-in-Differences calculations
- **Git / GitHub** – version control and project repository
- **Git LFS** – management of large data and dashboard files
- **XeLaTeX** – PDF document generation

---

## License

All rights reserved.

This repository is made available for academic review, professional portfolio demonstration and reference purposes only.

No reuse, modification or redistribution is permitted without explicit written permission from the author.

---

## Contact

**Tanveer Singh**  
Master of Data Science, Victoria University of Wellington  
New Zealand

**LinkedIn:** [linkedin.com/in/-tanveer-singh](https://www.linkedin.com/in/-tanveer-singh/)