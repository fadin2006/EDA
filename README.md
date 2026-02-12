# Multisource Energy Dataset Collection for Load and Renewable Forecasting

## Overview
This repository contains a curated collection of 9 energy-related time series datasets for research on electricity load forecasting and renewable energy generation prediction. The datasets span univariate and multivariate structures and originate from various regions, offering rich diversity for benchmarking machine learning, deep learning, and hybrid forecasting models.

## Dataset Categories

| Category               | Source Location          | Type         | Feature Type     | Frequency      |
|------------------------|---------------------------|--------------|------------------|----------------|
| PJME                   | USA (PJM East)            | Univariate   | Load (MW)        | Hourly         |
| PJMW                   | USA (PJM West)            | Univariate   | Load (MW)        | Hourly         |
| AEP                    | USA (AEP)                 | Univariate   | Load (MW)        | Hourly         |
| Dayton                 | USA (Dayton)              | Univariate   | Load (MW)        | Hourly         |
| Northern Illinois (NI) | USA (NI)                  | Univariate   | Load (MW)        | Hourly         |
| Individual Household   | France (Sceaux)           | Multivariate | Load + Submeters | Per Minute     |
| Tetouan City           | Morocco (Tetouan)         | Multivariate | Load + Weather   | 10-Minute      |
| Wind Turbine (Turkey)  | Turkey                    | Multivariate | SCADA            | 10-Minute      |
| Solar Plant (India)    | India                     | Multivariate | PV Generation    | 15-Minute      |

## Dataset Details

### Univariate Load Datasets (5 Datasets)
These datasets contain regional electricity load data with hourly granularity from PJM ISOs in the United States. They serve as robust benchmarks for classical forecasting models and neural networks.

### Multivariate Load Datasets (2 Datasets)
1. **Individual Household Dataset** (UCI Repository): Contains power consumption data with submetering, voltage, and reactive power.
2. **Tetouan City Dataset** (UCI Repository): Aggregated load from 3 distribution areas with corresponding weather data.

### Renewable Energy Datasets (2 Datasets)
1. **Wind Turbine SCADA** (Turkey): 2018 SCADA data with wind speed, direction, temperature, and generated power.
2. **Solar Power Plant** (India): Power generation data with environmental sensor readings (irradiance, temperature, etc.).

### Load Electricity Consumption
This directory is divided into three subfolders:
- **America Electricity Consumption**: Includes PJME, PJMW, AEP, Dayton, and NI datasets (hourly).
- **Tetouan City**: Contains multivariate load data with local weather indicators.
- **Individual Household**: Submeter-level residential consumption from France with minute-level resolution.

### Energy Generation
This directory contains:
- **Solar Energy Power Plant**: India-based solar PV generation and environmental sensor readings.
- **Wind Energy Power Plant**: SCADA wind turbine dataset from Turkey.

## Applications
- Short-term and long-term load forecasting
- Renewable power prediction (solar, wind)
- Seasonal decomposition and anomaly detection
- Feature selection and multivariate correlation
- Comparative benchmarking of forecasting models (ARIMA, LSTM, XGBoost, etc.)


## File Structure
All datasets are in `.csv` format with consistent timestamps. Each file includes a `datetime` column and respective feature columns.

```plaintext
Dataset/
├── Electricity_Load_Demand/
│   ├── America_Electricity_Consumption/
│   ├── Tetouan_City/
│   └── Individual_Household/
└── Energy_Generation/
    ├── Solar_Energy_Power_Plant/
    └── Wind_Energy_Power_Plant/
```


## Citation
Please cite each dataset source individually using the provided BibTeX entries in the `references.bib` file.

## License
This repository is released under the [MIT License](LICENSE).

---

For questions or collaborations, feel free to open an issue or contact the maintainer.
