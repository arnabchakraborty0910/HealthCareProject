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
- Arnab
- Yatharth

## Data

### Source

**OECD Health Expenditure and Financing Database** (System of Health Accounts, dataflow `DSD_SHA@DF_SHA`, version 1.1), downloaded from the [OECD Data Explorer](https://data-explorer.oecd.org/) on November 7, 2026.

- **Country:** United States
- **Time period:** 1970–2022, annual
- **Measure:** Health expenditure per person
- **Unit:** US dollars per person, PPP converted
- **Price base:** Current prices (not adjusted for inflation)
- **Size:** 1,052 rows, ~365 KB

The data is broken down by **financing scheme**, meaning who pays for the healthcare:

| Code | Financing scheme |
|------|------------------|
| `_T` | Total (all schemes) |
| `HF11` | Government schemes |
| `HF121` | Social health insurance schemes |
| `HF12HF13` | Compulsory contributory health insurance schemes |
| `HF2` | Voluntary healthcare payment schemes |
| `HF21` | Voluntary health insurance schemes |
| `HF23` | Enterprise financing schemes |
| `HF3` | Household out-of-pocket payments |
| `HF2HF3` | Voluntary schemes and out-of-pocket payments combined |

**Key columns used in the analysis:**

- `TIME_PERIOD`: year
- `OBS_VALUE`: spending per person (USD, PPP)
- `FINANCING_SCHEME`: financing scheme code

### Access

The raw data file is included in this repository:

`OECD.ELS.HD,DSD_SHA@DF_SHA,1.1,filtered,2026-11-07 23-20-50.csv`

It is publicly available, aggregate national data and contains no individual or patient information.

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
