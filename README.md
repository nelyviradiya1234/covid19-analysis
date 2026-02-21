# COVID-19 Global Data Analysis

A Python data analysis project exploring global COVID-19 trends including cases, deaths, vaccination progress, recovery rates, and case fatality rates across 5 major countries.

**Author:** Nely Viradiya
**Tools:** Python, Pandas, Matplotlib, Seaborn
**Dataset:** Included locally — covid19_tableau_data.csv 

---

## What This Project Analyses

| # | Analysis | Description |
|---|---|---|
| 1 | Cases & Deaths Over Time | 4-week rolling average trend lines for 5 countries |
| 2 | Country-wise Comparison | Total cases & deaths per million population |
| 3 | Vaccination Progress | % population vaccinated vs 70% herd immunity target |
| 4 | Case Fatality Rate | Deaths as a % of confirmed cases per country |

---

## Countries Covered

- India
- United States
- Brazil
- United Kingdom
- Germany

---

## How to Run

### 1. Clone the repository
```bash
git clone https://github.com/nelyviradiya1234/covid19-analysis.git
cd covid19-analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the analysis
```bash
python covid_analysis.py
```

### 4. View results
All 4 charts are saved automatically to the `output_charts/` folder.

---

## Project Structure

```
covid19-analysis/
│
├── covid_analysis.py           # Main analysis script
├── covid19_tableau_data.csv    # Dataset (local — no internet needed)
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
└── output_charts/              # Generated charts (auto-created on run)
    ├── 1_cases_deaths_over_time.png
    ├── 2_country_comparison.png
    ├── 3_vaccination_progress.png
    └── 4_case_fatality_rate.png
```

---

## Sample Output

```
============================================================
  SUMMARY REPORT
============================================================

  India
    Total Cases   :       2,744,215
    Total Deaths  :          45,556
    CFR           :           1.66%
    Vaccinated    :          92.0%
    Recovery Rate :          98.3%

  United States
    Total Cases   :       3,722,131
    Total Deaths  :          62,750
    CFR           :           1.69%
    Vaccinated    :          92.0%
    Recovery Rate :          98.3%
...
```

---

## Tableau Dashboard

This project also includes a full interactive Tableau dashboard built using `covid19_tableau_data.csv`.

The dashboard contains:
- 4 KPI cards — Total Cases, Total Deaths, Avg CFR, Avg Vaccination %
- Line chart — Weekly cases over time with country filter
- Bar chart — Cases per million (population-adjusted)
- Line chart — Vaccination progress vs 70% herd immunity target
- Bar chart — Case fatality rate by country
- World heatmap — Global spread visualised geographically
- Cross-filtering — Click any country and all charts update together

---

## Key Insights

- Countries with earlier vaccination rollouts show a clear decline in death rates post-vaccination
- Case Fatality Rate varies by country due to differences in testing capacity and healthcare systems
- The 4-week rolling average smooths out reporting anomalies and reveals true epidemic curves
- Recovery rates remain consistently above 98% across all 5 countries

---

## Skills Demonstrated

- Data loading and processing using Pandas
- Time-series analysis and rolling averages
- Data visualisation with Matplotlib and Seaborn
- Population-adjusted comparative analysis
- Dashboard design using Tableau
- Writing clean, well-documented Python code

---

## License

This project is open source and available under the MIT License.
