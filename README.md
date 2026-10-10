# Chicago Taxi Analysis

This project analyzes taxi ride data in Chicago using Python. The objective is to perform exploratory data analysis (EDA) on taxi companies, trip destinations, and ride patterns, as well as test a statistical hypothesis regarding trip duration under different weather conditions.

## Project Objectives

- Identify the most popular drop-off neighborhoods in Chicago.
- Determine which taxi companies completed the highest number of trips.
- Analyze ride duration patterns under different weather conditions.
- Test whether weather conditions have a significant impact on trip duration.

## Datasets

The project uses the following datasets:

- `project_sql_result_01.csv` - Taxi companies and number of trips.
- `project_sql_result_04.csv` - Neighborhoods and average trips.
- `project_sql_result_07.csv` - Trips from the Loop to O'Hare International Airport, including weather conditions and trip duration.

## Technologies and Libraries

- Python
- Pandas
- Plotly Express
- SciPy

## Project Structure

```text
Sprint 8/
│
├── datasets/
│   ├── project_sql_result_01.csv
│   ├── project_sql_result_04.csv
│   └── project_sql_result_07.csv
│
├── notebook.ipynb
├── README.md
└── .gitignore
```

## Key Findings

### Neighborhood Analysis
- Loop is the most popular drop-off destination.
- River North and Streeterville rank second and third.
- Taxi demand is concentrated in a small number of neighborhoods.

### Taxi Companies
- Flash Cab is the market leader with 19,558 trips.
- Flash Cab completed approximately 71% more trips than the second-ranked company.
- Most competitors show similar trip volumes, indicating a highly concentrated market.

### Hypothesis Testing
- Levene's test indicated that the equal variances assumption was satisfied (p-value = 0.53).
- A Student's t-test found a statistically significant difference in trip durations between rainy and non-rainy conditions (p-value < 0.05).
- The null hypothesis was rejected.

## Conclusion

The analysis shows that taxi activity is concentrated in a limited number of neighborhoods and among a few major companies. Additionally, weather conditions have a statistically significant impact on trip duration, with adverse weather associated with longer trips between the Loop and O'Hare International Airport.

## Author

Juan Pablo Ramirez Guerra
