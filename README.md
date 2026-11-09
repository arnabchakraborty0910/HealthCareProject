# HealthCareProject

## Purpose

Healthcare costs in the United States have risen steadily for decades. This project uses linear regression to measure how healthcare spending has changed over time, estimate the average yearly increase, and explore what factors are associated with that growth.

## Research Question

How has healthcare spending in the United States changed over time, and how well does a linear trend explain that change?

- **Outcome (response variable):** national health expenditure per capita, in USD
- **Predictor:** Year

## Team

- Tanya
- Eric
- Arnav
- Yatharth

## Data

### Source

[e.g. Centers for Medicare & Medicaid Services (CMS) National Health Expenditure (NHE) Data, [link]]

- **Time period:** [e.g. 1960–2023]
- **Level:** [e.g. national, yearly totals]
- **Size:** [number of rows and columns]

### Data Cleaning

- Select the relevant years and spending columns
- Handle any missing values

### Exploratory Analysis

- Plot healthcare spending over time
- Calculate summary statistics and change each year
- Check for nonlinear patterns (like faster growth in recent decades)

### Modeling

- Fit a simple linear regression with year predicting healthcare spending


### Evaluation

- Residual plots to check changes in error
- Interpretation of the slope (average increase in spending per year)

### Requirements

- Python [version]
- pandas, numpy, matplotlib, scikit-learn

## Results

  _________

## Limitations

- Linear regression shows trends and associations, not causes
- Healthcare costs may grow exponentially, so a straight line may underestimate recent growth
- Without inflation adjustment, part of the increase reflects general price increases rather than healthcare specifically
- Yearly national data gives a small number of data points

## Ethics and Data Privacy

This project uses publicly available, aggregate national data. It contains no individual patient information or personally identifiable data.
