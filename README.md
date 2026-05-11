# DHS Child Malnutrition Analysis in Kenya

## Project Overview
This project analyzes child malnutrition in Kenya using data from the Demographic and Health Surveys (DHS) Program. The study focuses on three key nutritional indicators among children under five years of age:

- Stunting (height-for-age)
- Wasting (weight-for-height)
- Underweight (weight-for-age)

The analysis was conducted using R and demonstrates data cleaning, indicator creation, prevalence estimation, and data visualization.

## Objectives
- Measure the prevalence of child malnutrition in Kenya.
- Create nutritional indicators using WHO z-score thresholds.
- Visualize the prevalence of stunting, wasting, and underweight.
- Demonstrate practical statistical programming skills using real-world survey data.

## Dataset
- Source: Demographic and Health Surveys (DHS) Program
- Country: Kenya
- File: KEKR8AFL.DTA
- Population: Children under five years of age

## Methodology
1. Import DHS data.
2. Select relevant anthropometric variables.
3. Recode WHO z-scores.
4. Create binary indicators using WHO thresholds (DHS stores z-scores multiplied by 100):
- Stunted: hc70 < -200 (equivalent to height-for-age z-score < -2 SD)
- Wasted: hw72 < -200 (equivalent to weight-for-height z-score < -2 SD)
- Underweight: hw71 < -200 (equivalent to weight-for-age z-score < -2 SD)
5. Calculate prevalence percentages.
6. Produce summary tables and visualizations.

## Tools and Packages
### Software
- R
- RStudio
- Git
- GitHub

### R Packages
- haven
- dplyr
- tidyr
- ggplot2

## Repository Structure
dhs-data-analysis-kenya/
├── README.md
├── Child_Malnutrition_Report.Rmd
├── data/
│   └── KEKR8AFL.DTA
├── scripts/
│   └── Child_Malnutrition_Analysis_Kenya.R
└── outputs/
    ├── prevalence_table.csv
    ├── stunting_plot.png
    ├── wasting_plot.png
    ├── underweight_plot.png
    └── child_malnutrition_report.pdf

## Key Findings
The analysis estimates the prevalence of:
- Stunting
- Wasting
- Underweight

These indicators are essential for monitoring child health and nutrition and informing public health interventions.

## Skills Demonstrated
- Data cleaning and transformation
- Statistical analysis
- Public health data analysis
- Data visualization
- Reproducible reporting
- Version control with Git and GitHub

## How to Run the Project
1. Clone the repository.
2. Open the project in RStudio.
3. Install required packages.
4. Run the script in `scripts/`.
5. Knit `Child_Malnutrition_Report.Rmd` to generate the final report.

## Author
Salim Mkulu  
Statistics & Programming Undergraduate  
Machakos University, Kenya  
Email: mkulusalim7@gmail.com  
GitHub: https://github.com/Mkulu-Statix
