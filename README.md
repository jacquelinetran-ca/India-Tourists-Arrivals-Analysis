# India Tourist Arrivals: Seasonality & 2014 Forecast

A time series analysis of monthly foreign tourist arrivals to India (2001–2013), used to understand the tourism season and forecast 2014 arrivals for staff planning. This is an example of a project completed in my Competing with Analytics course. 

## Tools
Python (pandas, NumPy, statsmodels, matplotlib) in Google Colab

## Data
`IndiaTouristsArrivalsData.csv`: monthly tourist arrivals, January 2001 to December 2013 (156 months).

## What the Notebook Does
1. **Plots the series** to check for trend, seasonality and volatility.
2. **Decomposes it** into trend, seasonal and residual parts (multiplicative model, because the seasonal swings grow as arrivals grow).
3. **Checks growth** by comparing the trend for January 2013 with January 2012, rather than the raw numbers.
4. **Forecasts 2014** with a linear regression on a time trend plus month dummies.
5. **Turns the forecast into a staffing recommendation** by comparing the upper end of the 2014 forecast range with actual 2013 arrivals.

## Key Findings
- **Peak season is November to February.** December runs about 34% above an average month. May is the low point, about 30% below.
- **Real growth is about 3%, not 8%.** Comparing trend values gives 3.3% growth from 2012 to 2013, well below the 8% claimed in the case.
- **July 2010 was an outlier**, about 51% above what the trend and season predicted.
- **The model fits well:** R² = 0.92. Arrivals grow by about 2,800 per month on trend.
- **2014 forecast:** from about 503,000 arrivals (May) to about 776,000 (December).

## Recommendation
Increase staff by **up to about 30% from April to September** compared with 2013 levels, and by about 12% in October. Staffing from November to March can stay close to 2013 levels.
