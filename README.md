# AQI-Analysis-And-Prediction

## 📌Objective
To identify
pollution patterns, understand the relationship between air quality and public health (respiratory cases),
determine which pollutants drive AQI the most, and build a predictive model that estimates AQI from
pollutant levels.

## 🗂️Dataset Information
Source: https://airquality.cpcb.gov.in/ccr/#/caaqm-dashboard-all/caaqm-landing/aqi-repository
| Column            | Type    | Description                                     | Range / Values                                        |
| ----------------- | ------- | ----------------------------------------------- | ----------------------------------------------------- |
| Date              | String  | Observation date (DD-MM-YYYY)                   | 2023–2024                                             |
| Location          | String  | Monitoring station / city                       | 5 unique locations                                    |
| PM2.5             | Float   | Fine particulate matter concentration (µg/m³)   | 3.35 – 794.00                                         |
| PM10              | Float   | Coarse particulate matter concentration (µg/m³) | 11.80 – 790.75                                        |
| NO2               | Float   | Nitrogen dioxide concentration (µg/m³)          | 0.14 – 224.25                                         |
| NH3               | Float   | Ammonia concentration (µg/m³)                   | 0.04 – 232.56                                         |
| SO2               | Float   | Sulfur dioxide concentration (µg/m³)            | 0.22 – 161.20                                         |
| CO                | Float   | Carbon monoxide concentration (mg/m³)           | 0.04 – 7.45                                           |
| O3                | Float   | Ozone concentration (µg/m³)                     | 0.13 – 185.19                                         |
| AQI               | Integer | Composite Air Quality Index                     | 21 – 500                                              |
| Severity          | String  | AQI category (6 levels)                         | Good, Satisfactory, Moderate, Poor, Very Poor, Severe |
| Respiratory Cases (Synthetic) | Integer | Reported respiratory cases per day              | 4 – 163                                               |

##  ⛓️Project Workflow
Data Acquisition
      →
Data Cleaning
      →
Exploratory Data Analysis
      →
Feature Analysis
      →
Visualization
      →
Predictive Modeling
      →
Reporting
## 💡Key Findings
- PM2.5 and PM10 together account for over 78% of total feature importance in predicting AQI.
- Delhi recorded the highest average AQI (217.9) - 2.6x higher than Chennai (83.7), the cleanest city studied.
- Delhi's poor air quality is sustained rather than occasional  it spends a large share of the year in Poor or
worse severity bands.
- 3 of 5 cities improved year-on-year (Kolkata -35%, Mumbai -31%, Chennai -25%), while Delhi and Bengaluru stayed flat.
-  Respiratory cases rose approximately 7x between "Good" and "Severe" AQI days.
## 🛠️Tech Stack
| Layer              | Tool / Library                |
| ------------------ | ----------------------------- |
| Language           | Python                        |
| Data Handling      | pandas                        |
| Visualization      | matplotlib, seaborn           |
| Machine Learning   | scikit-learn                  |
| Model              | RandomForestRegressor         |
| Evaluation Metrics | r2_score, mean_absolute_error |

## 📈Future Improvements 
- Add more cities beyond the current 5 and extend the time range past 2023–2024 for stronger trend analysis.
- Incorporate temperature, humidity, wind speed, and rainfall — these strongly influence pollutant dispersion and are currently missing from the dataset.
- Move beyond predicting current AQI from its own pollutant inputs (R² = 0.84) toward forecasting next-day or future AQI using time-series methods (ARIMA, Prophet, or LSTM), with cross-validation.

## 📱Contact
Email: rajnistane9@gmail.com

LinkedIn: https://www.linkedin.com/in/raj-nistane/
