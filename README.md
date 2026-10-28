# Air Pollution and Weather Patterns

## Project Overview
This beginner-friendly data analysis project explores how air pollution measurements vary with observed weather conditions. It uses the supplied OpenWeather dataset and combines exploratory data analysis (EDA) with statistical hypothesis tests.

## Project Files
Keep these files together in the same project folder:

- `openweather_weather_airpollution_top3cities_per_country.csv` — source dataset used by the notebook.
- `Air_Pollution_Weather_Project_Guide_updated.ipynb` — main notebook containing data preparation, EDA, statistical tests, results, and **all project graphs**.
- `Air_Pollution_Weather_Presentation.pptx` — themed presentation summarizing the project and findings; it intentionally contains no graphs.
- `Air_Pollution_Weather_Report.docx` — written report; graphs are intentionally kept in the notebook only.
- `README.md` — project overview and instructions.

## Dataset at a Glance
- 108,467 rows and 88 columns.
- Records from 598 cities across 209 countries.
- Includes air-pollution measurements, AQI categories, weather descriptions, and weather-related measurements.

## Main Findings
- The median PM2.5 value was **3.73**, while the mean was **10.63**. Confirm the units in the source metadata before comparing these values with external standards.
- **17.34%** of records had AQI category 3 or higher, using the project's chosen definition of “high AQI.”
- Mean PM2.5 was **6.35** in records with observed rainfall and **11.26** in records without observed rainfall.
- Records labelled smoke and haze showed higher average PM2.5, although these weather groups had relatively few observations.

These results describe patterns in this dataset. They do not establish that a weather condition caused a change in pollution.

## Analysis Included
The notebook covers data understanding and quality checks, exploratory analysis, visualizations, and five hypothesis tests:
- One-sample proportion z-test.
- Two-sample t-test comparing PM2.5 in rainy and non-rainy records.
- Chi-square test of association.
- One-way ANOVA across continent groups.
- Two-proportion z-test comparing high-AQI proportions in rainy and non-rainy records.

The AQI category threshold and 20% benchmark used in the tests are project choices, not official health standards. Statistical significance does not by itself show that a difference is large or practically important.


### Dashboard 
- Image File Name: Dashboard_basic_themed
- Power BI File : Dashboard_powerBi_themed
  

## How to Run
1. Place the CSV, notebook, and this README in the same folder.
2. Open `Air_Pollution_Weather_Project_Guide_updated.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Make sure the required Python libraries used by the notebook are available (including **pandas**, **NumPy**, **Matplotlib**, and the statistical library or libraries imported in the hypothesis-testing cells).
4. Run the notebook cells from top to bottom. The tables, statistical results, and all graphs are produced in the notebook.

## Limitations and Cautions
- Missing values and uneven sample sizes may affect comparisons.
- Some weather categories, such as smoke and haze, contain few records; interpret their averages cautiously.
- Repeated city/time keys should be reviewed before treating every row as an independent observation.
- Verify timestamp consistency before making time-trend or seasonal claims.
- The analysis is observational: association does not prove causation.
