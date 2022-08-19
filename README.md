# Algorithmic Trading

## Strategies

1. Simple Moving Average Crossover - Here, we take the 2 moving averages (say 20 days and 50 days). We place a buy order if the shorter moving average crosses the longer moving average and place a sell order otherwise.
For an exit strategy, we simply reverse the above logic. Note that we will analyse this for only one stock since I did this to just get a hang of how things work

2. Bollinger Band Bullish Strategy: For this, we first create the bollinger bands which are a set of 3 indicatiors, mean, mean + n\*std_deviation, mean - n\*std_deviation. n is choosen to be 1. This helps us to measure volatility. Here we will place a buy order if it crosses over the the top band (buy zone). The idea is to identify uptrends and place a long order. As an exit strategy, we will exit as soon as the price falls outside of the buy zone and there is a red candle that day. This strategy works quite well for bullish markets


3. We also extended this to multiple stocks. Some modifications in the code were needed for example looping over all data feeds, and creating a dict to store the values.
## Results

For our final strategy, we see that we get a nice return of around 450%




