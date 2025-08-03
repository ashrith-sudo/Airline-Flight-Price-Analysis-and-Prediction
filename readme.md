# Airline Flight Price Analysis and Prediction

This project provides an in-depth analysis of airline flight price data, aiming to identify patterns and insights that can help in understanding and predicting flight prices. The core of the analysis is performed in the notebook [`Airline_Flight_Price_Analysis_and_Prediction.ipynb`](Airline_Flight_Price_Analysis_and_Prediction.ipynb).



## Project Overview

The main task is to analyze airline flights data to discover patterns and insights related to flight pricing. The notebook walks through loading the data, exploring its structure, performing basic statistics, and handling data preprocessing. This pipeline sets the stage for further modeling and prediction tasks.

## Dataset

The analysis uses a dataset named `airlines_flights_data.csv` with over 300,000 entries and 12 columns, including:

- `airline`, `flight`, `source_city`, `departure_time`, `stops`, `arrival_time`, `destination_city`, `class`, `duration`, `days_left`, `price`

Sample rows:

| airline  | flight | source_city | departure_time | stops | arrival_time | destination_city | class   | duration | days_left | price |
|----------|--------|-------------|---------------|-------|--------------|------------------|---------|----------|-----------|-------|
| SpiceJet | SG-8709| Delhi       | Evening       | zero  | Night        | Mumbai           | Economy | 2.17     | 1         | 5953  |
| AirAsia  | I5-764 | Delhi       | Early_Morning | zero  | Early_Morning| Mumbai           | Economy | 2.17     | 1         | 5956  |

## Analysis Steps

The notebook proceeds through the following stages:

1. **Loading the Data**
   - Uses pandas to load the CSV into a DataFrame.
2. **Initial Exploration**
   - Displays the first few rows for verification.
   - Checks data types, missing values, and basic statistics for both numerical and categorical columns.
3. **Data Cleaning and Preprocessing**
   - Handles missing values, outliers, and inconsistencies.
   - Prepares the data for further analysis or modeling.
4. **Exploratory Data Analysis (EDA)**
   - Investigates the distribution of numerical columns (duration, days_left, price) and unique values in categorical columns (airline, city, stops, etc.).
   - Visualizes data distributions and relationships.
5. **Feature Engineering (Potential for extension)**
   - Identifies and handles potential outliers.
   - Assesses categorical features for modeling.

## Key Insights

- The dataset contains no missing values and covers major Indian airlines, cities, and classes.
- Price varies significantly with days left, airline, stops, and other features.
- Majority flights are operated by Vistara, and the most frequent route is between Delhi and Mumbai.

## How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/ashrith-sudo/Airline-Flight-Price-Analysis-and-Prediction.git
    ```
2. Install dependencies (Python 3, pandas, matplotlib, seaborn):
    ```bash
    pip install pandas matplotlib seaborn
    ```
3. Place the dataset (`airlines_flights_data.csv`) in the notebook directory.
4. Open and run the notebook:
    - Using Jupyter:
        ```bash
        jupyter notebook Airline_Flight_Price_Analysis_and_Prediction.ipynb
        ```
    - Or in Google Colab.

## Repository Structure

- `Airline_Flight_Price_Analysis_and_Prediction.ipynb` - Main analysis notebook
- `airlines_flights_data.csv` - Dataset (not included for copyright reasons)
- Other files/folders (add as needed)

## License

This project is licensed under the MIT License. See the LICENSE file for details.
