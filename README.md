# Anomaly Detection in Cricket Scores

## Project Overview

This project demonstrates how to detect anomalies in cricket scores using the Isolation Forest algorithm from the Scikit-learn library. The dataset includes scores from various overs, and the goal is to identify unusual score values that could indicate anomalies.


## Data Description

- **Overs**: Number of overs in a cricket match (integer).
- **Scores**: Runs scored in the respective overs (integer).
- **Row_Number**: A sequential identifier for each entry (integer).

A sample of the dataset is provided, including both original and randomly generated scores.

## Model Implementation

1. **Data Preparation**: 
   - The dataset is created with fixed overs and scores, along with random scores for demonstration.
   
2. **Anomaly Detection**: 
   - The Isolation Forest model is trained on the scores to identify anomalies. The model parameters include:
     - `n_estimators`: Number of base estimators in the ensemble.
     - `contamination`: The proportion of observations identified as anomalies.

3. **Prediction**:
   - Anomalies are detected and stored in the DataFrame.

## Visualization

The project includes various visualizations to help understand the data and the results:

- **Scatter Plot**: Displays scores with anomalies highlighted.
- **Histogram**: Shows the distribution of scores with a threshold line.
- **Box Plot**: Visualizes the spread and outliers in the scores.

## Results

After running the model, the output includes:

- Total anomalies detected.
- Descriptive statistics of the scores, including mean, standard deviation, and quartiles.

Example output:

```
Total anomalies detected: 28 
Descriptive Statistics:
count    150.000000
mean      37.973333
std       21.507591
min        1.000000
25%       20.000000
50%       36.500000
75%       56.000000
max       79.000000
```

