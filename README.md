# Delays in NYC Airports

This repository explores the factors influencing departure delays at New York City airports using data from the `nycflights13` package. The analysis is divided into two main parts: examining variables affecting departure delays and building a predictive model to classify flights departing from EWR airport as late or on time.

## Dataset

The analysis primarily uses two datasets:

- **flights**: On-time data for flights departing from NYC airports (JFK, LGA, EWR) in 2013.
- **weather**: Hourly meteorological data for NYC airports in 2013.

## Part 1: Exploratory Data Analysis

### 1.1 Planned Departure Hour

The analysis examines the average departure delay for each hour of planned departure across the three airports (EWR, LGA, JFK). Notably, airports like LGA and JFK perform relatively better than EWR during peak hours.

### 1.2 Number of Flights

For each origin airport, the average departure delay is plotted against the number of flights to explore their relationship. Generally, as the number of flights increases, the average departure delay also tends to increase.

### 1.3 Weekday

Departure delays are analyzed by weekday, revealing higher average delays on Thursdays and Fridays across all airports. EWR consistently shows higher delays compared to JFK and LGA.

### 1.4 Month

Delays are examined by month, showing higher delays during the holiday season (December) and lower delays in months like September, October, and November. EWR typically experiences higher delays compared to LGA and JFK.

### 1.5 Wind

The impact of wind conditions (wind speed > 25) on departure delays is explored using boxplots, indicating varying effects across airports and time of day.

## Part 2: Predictive Modeling

### 2.1 Target Variable

The target variable for predictive modeling is defined as whether a flight departing from EWR arrives late (delay >= 15 minutes).

### 2.2 Data Preparation

Data cleaning involves filtering flights departing from EWR and excluding observations with missing departure delay information.

### 2.3 Model Building

A predictive model (logistic regression or decision tree) is constructed to classify flights departing from EWR as late or on time based on available predictors.

### 2.4 Model Evaluation

The model's performance is evaluated using appropriate metrics such as accuracy, precision, recall, and F1-score.

---

This README provides an overview of the project's objectives, datasets used, and the structure of analysis. For detailed insights and code implementation, refer to the respective sections in the repository.



Conclusion
This repository provides insights into the factors influencing departure delays at NYC airports and offers a predictive model to anticipate flight delays departing from EWR. Future improvements could involve incorporating additional variables or refining the modeling approach to enhance prediction accuracy.

For further details, refer to the detailed R scripts and outputs in this repository.

