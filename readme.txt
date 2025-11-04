project:
  title: "Crimes Against Women in India: 2001–2024"
  description: >
    This project analyzes trends in crimes against women in India from 2001 to 2024,
    combining official NCRB data with provisional data (2023–2024) sourced from
    reputable news and media. The goal is to uncover patterns, identify high-risk states,
    evaluate the impact of policies, and present insights through Python-based EDA and Power BI dashboards.

  objectives:
    - Analyze total crimes and crime types across states and years
    - Visualize year-over-year trends and highlight outliers or improvements
    - Compare pre- and post-policy impacts
    - Normalize crime rates based on population (where applicable)
    - Build a dashboard for intuitive exploration in Power BI

  tools:
    - Python (Pandas, Seaborn, Matplotlib, Jupyter Notebooks)
    - Power BI (Data Modeling & Visualization)
    - Microsoft Excel (for occasional data formatting)

  data_sources:
    - NCRB Official Reports (2001–2022) from [data.gov.in](https://data.gov.in)
    - News/media-based Provisional Data for 2023–2024
    - All cleaned datasets stored in `data/` folder

folder_structure:
  data/:
    - Cleaned_CrimesOnWomen_2001_2024.csv          # Combined dataset (official + provisional)
    - CrimesOnWomenData_Updated_Till_2024.csv       # Latest version used in dashboard
    - description.csv                               # Column descriptions and notes
    - ProvisionalData_2023_2024.csv                 # ✅ Provisional data (2023–2024 only)

  Jupyter_Notebooks/:
    - data_analysis.ipynb                           # Summary-level trends and comparisons
    - eda_and_insights.ipynb                        # Deep analysis (heatmaps, top states, YoY rates)

  Power_BI/:
    - women_dashboard.pbix                          # Final interactive dashboard

  (Optional) visuals/:                              # Exported plots (for presentation or reports)
  (Optional) docs/:                                 # Summary PDF or slide deck

how_to_use:
  1. Open `data_analysis.ipynb` to explore national and state-level crime patterns
  2. Use `eda_and_insights.ipynb` for trend deep dives and policy-based insights
  3. Open Power BI file `Power_BI/women_dashboard.pbix` for an interactive dashboard
  4. Explore `data/ProvisionalData_2023_2024.csv` for the most recent, unofficial crime data
  5. All datasets are already cleaned and structured — no transformation needed

notes:
  - 2023–2024 data is provisional and based on public news sources
  - All values represent officially *reported* crimes (not necessarily actual occurrences)
  - Population-normalized rates can be added for deeper insights if demographic data is added
