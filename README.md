# Datathon – Renovib

COVID-19 case analysis and forecasting focused on India. The notebooks explore similarity between India’s case trajectories and other countries, fit regression models to project near-term totals, and visualize results. Supporting data files and an R helper script are included for data cleaning and enrichment.

## Repository Layout
- `COVID 19 - Cleaned.ipynb`: main Jupyter notebook with EDA, cosine-similarity and MSE comparisons across countries, regression modeling (scikit-learn), and plotting.
- `COVID 19.ipynb`: earlier exploratory notebook comparing total confirmed deaths between countries.
- `Workspace.R`: R script snippets for joining Indian district/state data with zone codes; uses `dplyr`, `lubridate`, and `readr` in commented sections.
- `COVID India Final.pbix`: Power BI dashboard built from the cleaned datasets.
- Data files in the repo root: consolidated training data (`MLDataWithIndia.csv`), predictions (`predictions.csv`), state/district testing summaries, and country-level case/death counts.
- `Additional Data/`: reference CSVs (zones, population, hospital beds) with state codes produced by the R helper script.

## Key Technologies
- Python (Jupyter Notebook), `pandas`, `numpy`, `scikit-learn`, `matplotlib`.
- R (optional for additional preprocessing) with `dplyr`, `lubridate`, `tidyr`/`readr`.
- Power BI for dashboarding.

## Getting Started
1) Install Python dependencies: `pip install pandas numpy scikit-learn matplotlib jupyter`.
2) Start Jupyter: `jupyter notebook`, then open `COVID 19 - Cleaned.ipynb` to run the analysis. The notebook expects the CSVs in the repository root.
3) (Optional) For the R helper snippets, ensure `dplyr`, `lubridate`, and `readr` are available, then run sections from `Workspace.R` as needed.

Automated tests are not defined for this repository; verification is done by rerunning the notebooks or refreshing the Power BI report.
