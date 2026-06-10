# Climate Change Analysis

A data science project built to explore how CO2 emissions, energy consumption patterns, 
and global temperatures have changed over the past two decades — and where they might be heading.

This started as a university portfolio project but turned into something we genuinely found 
interesting to work on. The data tells a pretty clear story once you start digging into it.

---

## What this project does

We worked with 5 real-world datasets covering the period 2000-2023 and tried to answer 
some questions that actually matter:

- Which countries are responsible for the most CO2 emissions, and has that changed over time?
- Is there a measurable relationship between atmospheric CO2 and rising temperatures?
- How has the global energy mix shifted — are renewables actually making a dent?
- What do carbon market prices tell us about climate policy?
- Can we build a model that forecasts future CO2 emissions and temperature anomalies?

---

## Project structure
## Project structure

    climate-change-analysis/
    │
    ├── data/
    │   ├── raw/                          # original datasets as downloaded
    │   └── cleaned/                      # processed versions ready for analysis
    │
    ├── notebooks/
    │   ├── 01_data_cleaning.ipynb        # loading, inspecting and cleaning all 5 datasets
    │   ├── 02_visualizations.ipynb       # exploratory charts and trend analysis
    │   ├── 03_dashboard.ipynb            # multi-panel dashboard with event overlays
    │   ├── 04_machine_learning.ipynb     # CO2 emissions forecast model (Sasan Akbari)
    │   └── 05_temperature_prediction.ipynb  # temperature anomaly model (Arya Tahmasebi)
    │
    ├── outputs/
    │   ├── figures/                      # all saved charts and plots
    │   └── models/                       # trained ML models (.pkl files)
    │
    ├── requirements.txt
    └── README.md

---

## Datasets

| File | Description | Rows |
|---|---|---|
| carbon_prices_daily.csv | Daily EU carbon market prices from 2005 | ~15,800 |
| co2_emissions_yearly.csv | CO2 emissions by country with population and GDP | ~1,350 |
| energy_mix_yearly.csv | Energy source breakdown by country and year | ~1,350 |
| temperature_anomaly_monthly.csv | Global and regional temperature anomalies | ~2,500 |
| climate_events.csv | Major climate events and policy milestones | 50 |

---

## What we built

### Data Cleaning
Handled missing values, fixed date formats, removed duplicates and saved 
cleaned versions of all 5 datasets. Nothing groundbreaking here but it needed doing carefully.

### Visualizations
Six charts covering temperature trends, CO2 by country, energy transition 
progress, carbon prices and the correlation between CO2 concentration and warming.

### Dashboard
A multi-panel view that overlays real climate events (heatwaves, policy decisions, 
disasters) on top of the temperature and carbon price timelines. Gives a lot more 
context than looking at the numbers alone.

### Machine Learning
Two separate prediction models:

**CO2 Emissions Forecast** — trained on historical emissions data to project 
global CO2 output through to 2050. Uses polynomial regression to capture the 
non-linear growth curve. Built by Sasan Akbari.

**Temperature Anomaly Prediction** — predicts monthly global temperature anomaly 
using atmospheric CO2 concentration and emissions data as inputs. Tested Linear 
Regression against Random Forest and compared using MAE, RMSE and R2. Built by Arya Tahmasebi.

---

## How to run it

**1. Clone the repo**
```bash
git clone https://github.com/your-username/climate-change-analysis.git
cd climate-change-analysis
```

**2. Create and activate a virtual environment**
```bash
python -m venv venv

# Windows
venv\Scripts\activate

# Mac/Linux
source venv/bin/activate
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Launch Jupyter**
```bash
jupyter notebook
```

Then open the notebooks in order starting from `01_data_cleaning.ipynb`.

---

## Requirements
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
joblib

---

## Things we learned along the way

The CO2 vs temperature correlation is stronger than we expected — the scatter 
plot in notebook 02 makes it very visual. The energy mix charts were also 
surprising: renewables have grown significantly but fossil fuels still dominate 
in almost every region. The carbon price data has some dramatic spikes that line 
up directly with policy events in the climate events dataset.

The ML models are honest about their limitations — they project historical 
trends forward, which is the standard approach, but real future emissions depend 
heavily on policy decisions that no model can fully account for.

---

## Team

- Sasan Akbari(git hub id : sasanAkbari80) — data cleaning, visualizations, CO2 prediction model
- Arya Tahmasebi(git hub id : RealAriya) — dat cleaning, dashboard, temperature prediction model

---

## Acknowledgements

Data sourced from publicly available climate databases. 
This project was built as part of our preparation for applying to 
MSc programs in AI and Data Analytics.

