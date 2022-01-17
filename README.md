# Exchange Rate Forecast for Bitcoin
<div align="center">
  <img src="https://s2.coinmarketcap.com/static/img/coins/200x200/1.png" />
</div>

## The Idea
* **Making exchange rate forecast for Bitcoin**
* **Studying working with GitHub**
* **Researching the properties of time series**

## The Progress
### Getting data
So we found and downloaded bitcoin change data [**here**](https://finance.yahoo.com/quote/BTC-USD/history/?guccounter=1&guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAAAWoIdcDol-5rdFT-yFAJP_8t5XiP0K9HMkE3yInMoytwMCcmdqnd5LhN5f5tjOpJPpBX6oOaG8lkoQtlrU8bsi4gUO-4Eo-gkFVvJrOMkusfe5n-GERCEoeWLF3h-nzHAj6reN32AEZCyxrqXOceQ5E5U9_b86FSXTSbVFF-G6z).

The data contains of exchange rate of Bitcoin from 2017 till the 15th of January 2022
<div align="center">
  <img src="https://github.com/optimist2point0/exchange_rate_forecast/blob/main/Graphs/Bitcoin_graph_15.01.2022.png" />
</div>

### Data processing
First of all, we needed to get wanted data from the raw one to make a time series. Next, we defined its seasonality and tendency, made time series stationary by differencing.

#### Seasonality
<div align="center">
  <img src="https://github.com/optimist2point0/exchange_rate_forecast/blob/main/Graphs/Seasonality.jpg" />
</div>

#### Tendency
<div align="center">
  <img src="https://github.com/optimist2point0/exchange_rate_forecast/blob/main/Graphs/Trend.jpg" />
</div>

#### Stationarity
<div align="center">
  <img src="https://github.com/optimist2point0/exchange_rate_forecast/blob/main/Graphs/Stationarity.jpg" />
</div>

Now it was ready to fit some models.

### Fitting the model
The latest version of the model SARIMA is 0.0.3 with parameters ()x(). And its forecast compared to real data looks like:
<div align="center">
  <img src="https://github.com/optimist2point0/exchange_rate_forecast/blob/main/Graphs/Predict_v.0.0.3.jpg" />
</div>
