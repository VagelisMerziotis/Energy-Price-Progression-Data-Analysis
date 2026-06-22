# Energy-Price-Progression-Data-Analysis

Data analysis on price changes, energy consumption, crime rates, and related Greek economic indicators.

## Project layout

```
├── data/                  # CSV datasets (extracted from data_csvs.tar)
├── notebooks/             # Jupyter analysis notebooks
│   ├── energy.ipynb       # Energy balance and renewable energy trends
│   ├── economy.ipynb      # Economic indicators and debt dynamics
│   ├── DTW.ipynb          # Dynamic Time Warping on CPI / price data
│   └── UECF.ipynb         # Unemployment, employment, crime, fertility, wages
├── outputs/
│   ├── graphs/
│   │   ├── energy/        # Energy production and balance charts
│   │   ├── economy/       # GDP-sector and debt charts
│   │   ├── dtw/           # Correlation, Granger, DTW visualizations
│   │   └── uecf/          # Workforce, crime, fertility, wage charts
│   └── pdfs/              # Multi-page plot collections
├── docs/                  # Reference papers and supporting spreadsheets
├── data_csvs.tar          # Original dataset archive
└── README.md
```

## Datasets (`data/`)

| File | Topic |
|------|-------|
| `economy.csv`, `trimester-gross-debt.csv` | Economic indicators and debt |
| `daily_energy_balance.csv`, `energy_renewable.csv` | Energy |
| `DTK_2020.CSV` … `DTK_2023.CSV` | Consumer price index by product |
| `employment_in_thousands.csv`, `greece-unemployment-rate(1).csv`, `aggregated_employement_Data.csv` | Employment |
| `wages.csv`, `wages_clean.csv` | Wages (see `docs/wages_paper.pdf`) |
| `crime_data.csv`, `Greece_Crime_Rate_Statistics.csv` | Crime |
| `fertility.csv` | Demographics |
| `dtw.csv` | DTW analysis output |

## Running the notebooks
To run the notebooks and replicate results, the jupyter notebook package must be installed
Open and run notebooks from the `notebooks/` folder so relative paths resolve correctly:

```bash
cd notebooks
jupyter notebook
```

New charts and PDFs are written to `outputs/graphs/` and `outputs/pdfs/`.
