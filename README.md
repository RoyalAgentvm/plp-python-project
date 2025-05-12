# COVID-19 Data Analysis Project

## Overview

This project analyzes COVID-19 pandemic data across Kenya, the United States, and India, focusing on case numbers, death rates, and vaccination progress. The analysis provides insights into how different countries experienced the pandemic, the effectiveness of vaccination programs, and the relationship between various pandemic metrics.

## Dataset

The analysis uses the Our World in Data (OWID) COVID-19 dataset, which contains comprehensive COVID-19 data from countries worldwide. The dataset includes:

- Daily and cumulative case counts
- Daily and cumulative death counts
- Testing data
- Vaccination data
- Population metrics
- Various other pandemic indicators

## Features

This analysis includes:

1. **Data Cleaning and Preprocessing**
   - Handling missing values
   - Date conversion and validation
   - Linear interpolation of missing data points
   - Country-specific filtering

2. **Visualizations**
   - Total cases over time
   - Total deaths over time
   - Daily new cases (7-day rolling average)
   - Case fatality rates (total_deaths/total_cases)
   - Vaccination progress (total doses)
   - Population vaccination percentages

3. **Statistical Analysis**
   - Summary statistics for each country
   - Comparative metrics across countries
   - Monthly trends and averages
   - Correlation between vaccination and mortality

4. **Insights and Findings**
   - Comparative pandemic trajectories
   - Vaccination inequity analysis
   - Healthcare system effectiveness assessment
   - Identification of anomalies and interesting patterns

## Project Structure

```
covid-analysis/
├── data/
│   └── owid-covid-data.csv       # The OWID dataset
├── notebooks/
│   ├── data_cleaning.ipynb       # Data preprocessing and cleaning
│   ├── visualization.ipynb       # Visualization and analysis
│   └── insights.ipynb            # Insights and narrative
├── outputs/
│   ├── covid_analysis.png        # Cases and deaths visualizations
│   └── covid_vaccination_analysis.png  # Vaccination visualizations
├── README.md                     # This file
└── requirements.txt              # Required dependencies
```

## Requirements

This project requires the following Python packages:

```
pandas==1.5.3
matplotlib==3.7.1
seaborn==0.12.2
numpy==1.24.3
jupyter==1.0.0
```

## Installation and Usage

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/covid-analysis.git
   cd covid-analysis
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebooks:
   ```
   jupyter notebook notebooks/
   ```
   Or if using VS Code with Jupyter extension:
   ```
   code notebooks/
   ```

## Key Findings

The analysis reveals:

1. **Disparate Impact**: The pandemic affected countries differently based on demographics, healthcare infrastructure, and policy responses.

2. **Vaccine Access Inequality**: Stark differences in vaccine rollout speed and coverage across countries highlight global health inequities.

3. **Mortality Patterns**: Case fatality rates evolved differently across countries and pandemic phases, revealing healthcare system resilience and adaptability.

4. **Decoupling Phenomenon**: Post-vaccination, the relationship between case surges and death surges weakened significantly, demonstrating vaccine effectiveness.

5. **Data Limitations**: Significant differences in testing capacity, reporting methods, and demographic factors affect cross-country comparisons.

## Future Work

Potential extensions to this analysis:

- Include more countries for broader comparison
- Add hospitalization data for severity assessment
- Integrate mobility data to assess non-pharmaceutical interventions
- Analyze variant-specific impacts when data is available
- Develop predictive models for future pandemic waves

## Data Sources

The primary dataset used in this analysis is the Our World in Data COVID-19 dataset, available at:
https://github.com/owid/covid-19-data/tree/master/public/data

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Our World in Data for providing the COVID-19 dataset
- The global scientific community for their tireless work during the pandemic
- Open-source software tools that made this analysis possible
