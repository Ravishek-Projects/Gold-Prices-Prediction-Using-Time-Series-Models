# Gold Price - Analysis & Forecasting

**Author:** Ravishek Kumar

## Significance
* Gold is a safe-haven asset, often used to hedge against inflation, currency devaluation, and market volatility.
* Predicting its future price helps investors make informed decisions about buying, selling, or holding gold-related assets (bullion, ETFs, mining stocks, etc.).
* Institutions use gold forecasts to diversify risk across asset classes.
* During times of crisis (like war, inflation, or financial collapse), gold prices usually surge.
* Accurate predictions allow risk-averse players to prepare.
* Gold prices are influenced by macroeconomic indicators like interest rates, inflation, USD strength, and geopolitical tensions.

## Dataset Insights
* The project utilizes monthly data of gold prices from January 1950 to July 2020.
* The Average gold price in last 70 years is $416.56.
* Only 25% of the time, the gold price is above $447.07.
* Highest Gold price ever touched is $1840.81.
* The time series components (Trend, Seasonality, Cyclical Components, Random Variations) were analyzed to evaluate long-term movements and regular patterns.

## Models Evaluated
Various time series forecasting models were evaluated on their performance using the Mean Absolute Percentage Error (MAPE).

| Model | Test MAPE (%) |
|-------|---------------|
| **2pointMA** | 1.23 |
| **3pointMA** | 2.05 |
| **Rolling SARIMA** | 2.26 |
| **Rolling Holt-Winters** | 2.38 |
| **5pointMA** | 3.33 |
| **7pointMA** | 4.18 |
| **Naive Model** | 19.38 |
| **Linear Regression** | 29.14 |
| **SimpleAverage Model** | 73.01 |

## Industrial Applications
The Gold Price Time Series Forecasting project is widely applicable across various industries that deal with gold.
* **Financial Institutions and Investment Firms**: Helps optimize portfolios by predicting the best times to invest in gold or other assets.
* **Commodity Trading**: Traders use forecasts to build algorithmic trading strategies and make better decisions on buying or selling gold, while also identifying arbitrage opportunities in different markets.
* **Gold Mining and Production**: Forecasting gold prices enables companies to adjust their production levels and maximize profitability, as well as to forecast potential revenue and plan operational costs.
* **Macroeconomic Policy**: Central banks benefit from gold price forecasting by using it to monitor inflation, adjust monetary policy, and manage foreign reserves more effectively.
* **Supply Chain and Retail**: Industries dealing with gold jewelry use predictions for inventory planning and forecasting demand.

## Project File Structure
```text
├── Data/
│   ├── annual_csv.csv - Historical annual gold price data.
│   └── monthly_csv.csv - Monthly gold price data used as the primary dataset.
├── Project Video.mp4 - Video presentation explaining the methodology and results.
├── RTSMReport.pdf - Comprehensive report detailing the analysis and model comparisons.
└── RTSM_Gold_prices_Python_code.ipynb - Jupyter Notebook containing data preprocessing, EDA, and model training code.
