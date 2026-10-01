# Early Warning Prediction of Coral Bleaching Risk in the Central Saudi Arabian Red Sea

XGBoost model forecasting coral bleaching risk from public satellite data.

F1 = 0.972 for urgent risk (onset within two weeks) on 2019–2022 test data. First warning issued 10 days before the Degree Heating Week crossed the bleaching threshold in both the 2020 and 2024 events.

Full paper: [`paper/`](paper/)

## Data

| Source | Variables |
|---|---|
| [NOAA Coral Reef Watch](https://coralreefwatch.noaa.gov/product/vs/data/madinah_makkah.txt) | DHW, HotSpot, SST anomaly |
| [NOAA PSL Dipole Mode Index](https://psl.noaa.gov/data/timeseries/month/DMI/) | Indian Ocean Dipole |
| [CAMS Solar Radiation](https://ads.atmosphere.copernicus.eu/datasets/cams-solar-radiation-timeseries) | GHI, clear-sky GHI |

Station: Al Madinah and Makkah region (21.125°N, 39.45°E).

## Running

Runs in Google Colab without setup. Upload the files from `data/` to the session, then run all cells.

Requires: `pandas`, `numpy`, `matplotlib`, `xgboost`, `scikit-learn`, `shap`.

---

Wiam Fahad Alhafedhi
