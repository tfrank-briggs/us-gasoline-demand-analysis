# U.S. Gasoline Demand Analysis

## Overview

This project examines the relationship between retail gasoline prices and gasoline consumption in the United States from January 2010 through December 2025.

The analysis was completed as an applied economic research project using monthly U.S. data and multiple regression analysis.

## Business Question

How responsive is U.S. gasoline consumption to changes in retail gasoline prices, and what does the estimated relationship imply for businesses operating in the gasoline market?

## Data

The analysis uses 192 monthly observations from January 2010 through December 2025.

The primary variables are:

- U.S. finished motor gasoline product supplied, used as a proxy for gasoline consumption
- U.S. regular retail gasoline price
- Real disposable personal income
- Month-of-year controls for seasonality

### Data Sources

- U.S. Energy Information Administration (EIA)
- U.S. Bureau of Economic Analysis (BEA)
- Federal Reserve Economic Data (FRED)

## Method

The analysis estimates the following log-log regression model:

ln(Q_t) = β0 + β1 ln(P_t) + β2 ln(I_t) + Monthly Controls + ε_t

where:

- Q_t = U.S. gasoline consumption
- P_t = U.S. retail gasoline price
- I_t = real disposable personal income
- β1 = estimated gasoline price elasticity coefficient

The model was estimated using ordinary least squares (OLS) with monthly controls for seasonal variation.

Additional validation checks were conducted to examine autocorrelation and the influence of the COVID-19 period.

## Key Results

The baseline model produced:

- Gasoline price coefficient: -0.0094
- Price coefficient p-value: 0.610
- R-squared: 0.2589
- Adjusted R-squared: 0.2047
- Observations: 192

The estimated gasoline price coefficient was negative, consistent with economic theory, but was not statistically significant.

The strongest patterns in the data were seasonal. Gasoline consumption was generally higher during summer months, particularly June through August.

Validation tests also showed that the estimated relationship between gasoline prices and consumption was sensitive to the sample period.

## Business Implications

The results suggest that businesses operating in the gasoline market should avoid relying on a single national price-elasticity estimate when forecasting gasoline sales.

Seasonality, market conditions, local competition, wholesale costs, traffic patterns, and unusual economic disruptions may all be important when making pricing and inventory decisions.

## Files

- `paper/` — Final research paper
- `data/` — Dataset and Excel analysis
- `results/` — Selected figures and analysis outputs

## Reproducibility

The Excel workbook contains the monthly dataset, variable transformations, regression inputs, and analysis used in the paper.

The analysis covers January 2010 through December 2025.

## Research Paper

The SSRN link to the published paper will be added here after publication.

## Author

Tamunotonte Frank-Briggs  
MBA, Massry School of Business  
University at Albany
