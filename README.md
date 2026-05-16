# Child Malnutrition Analysis in Kenya (DHS)

## Project Overview

This project analyzes child malnutrition in Kenya using data from the Kenya Demographic and Health Survey (KDHS). The study focuses on three internationally recognized nutritional indicators among children under five years of age:

- **Stunting** (Height-for-age)
- **Wasting** (Weight-for-height)
- **Underweight** (Weight-for-age)

The analysis also explores inequalities in malnutrition by:

- Place of residence (Urban/Rural)
- Household wealth index
- Mother's education level
- Sex of the child

The project was conducted in **R** using survey weights from DHS data to produce nationally representative estimates.

---

## Objectives

The main objectives of this project are to:

1. Estimate the national prevalence of stunting, wasting, and underweight.
2. Examine disparities by socioeconomic and demographic characteristics.
3. Create publication-quality visualizations.
4. Export summary tables and plots for reporting.
5. Demonstrate practical skills in data cleaning, analysis, visualization, and reproducible reporting.

---

## Data Source

The data used in this project comes from the **Kenya Demographic and Health Survey (KDHS)** and is distributed through the DHS Program.

- Dataset used: `KEBR8CFL.DTA`
- File type: Stata (`.dta`)
- Access requires registration and approval from the DHS Program.

DHS data are nationally representative household surveys that provide information on health and nutrition indicators in developing countries.

---

## Methodology

### Data Preparation

The analysis involved the following steps:

- Importing the DHS child recode dataset.
- Creating sampling weights using `v005 / 1,000,000`.
- Selecting relevant variables.
- Replacing invalid anthropometric values with missing values.
- Constructing binary indicators:
  - Stunted (`hw70 < -2 SD`)
  - Wasted (`hw72 < -2 SD`)
  - Underweight (`hw71 < -2 SD`)
- Recoding explanatory variables.

### Statistical Analysis

Weighted prevalence estimates were calculated using `weighted.mean()` to account for the complex DHS sampling design.

### Visualization

Bar charts were created using `ggplot2` to illustrate:

- Overall prevalence of malnutrition
- Stunting by wealth index
- Stunting by residence
- Combined wealth and residence inequalities
- Individual plots for each malnutrition indicator

---

## Tools and Packages Used

### Programming Language
- R

### R Packages
- `haven`
- `dplyr`
- `tidyr`
- `ggplot2`
- `knitr`

### Development Tools
- RStudio
- Git
- GitHub

---

## Project Structure

```text
DHS-Child-Malnutrition-Project/
│
├── Child_Malnutrition_Analysis_Kenya.Rmd
├── Child_Malnutrition_Analysis_Kenya.html
├── README.md
│
└── outputs/
    ├── prevalence_table.csv
    ├── stunting_plot.png
    ├── wasting_plot.png
    ├── underweight_plot.png
    └── overall_prevalence_plot.png
```
 
## Key Outputs

### Summary Table

- `prevalence_table.csv`

### Visualizations

- `stunting_plot.png`
- `wasting_plot.png`
- `underweight_plot.png`
- `overall_prevalence_plot.png`

### Reproducible Report

- `Child_Malnutrition_Analysis_Kenya.html`

---

## Key Skills Demonstrated

- Data cleaning and transformation
- Survey-weighted statistical analysis
- Public health data analysis
- Data visualization
- Reproducible reporting with R Markdown
- Version control with Git and GitHub

---

## How to Run the Project

1. Clone the repository.
2. Open the project in RStudio.
3. Install the required packages.
4. Update the file path to the DHS dataset if necessary.
5. Knit `Child_Malnutrition_Analysis_Kenya.Rmd` to generate the final report.

---

## Conclusion

This analysis estimates the prevalence of child malnutrition in Kenya and highlights important inequalities by socioeconomic and demographic characteristics. The results show that children from poorer households and rural areas experience higher levels of malnutrition, emphasizing the need for targeted nutrition and public health interventions.

---

## Author

- **Mkulu Salim**
- Statistics & Programming Undergraduate
- Machakos University, Kenya
- Email: mkulusalim7@gmail.com
- GitHub: https://github.com/Mkulu-Statix