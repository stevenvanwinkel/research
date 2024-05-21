# Research

## Machine Learning
### Intraday ML
A simple machine learning strategy based on intraday data. The strategy uses a large set of pre-calculated features based on minute bars, which are resampled to hourly bars. The Machine Learning model used is a hyper-parameter tuned LGBM.
The idea of the strategy is to open a trading position in the morning and close it in the evening.

### Machine Learning Strategy using Trend Scanner (Daily data)
In this notebook we will try to implement a simple Machine Learning based strategy to forecast and trade an S&P 500 ETF. The strategy uses a set of very simple technical features, permutation as a feature selection algorithm and an optuna-based hyper parameter optimization. The label for the strategy is based on Marcos Lopez de Prado's Trend Scanner.

### Conditional Probability to improve an options selling strategy
In this notebook we try to use Ernest Chan's ideas on Conditional Probability (https://www.youtube.com/watch?v=nBy7b_oZ7mE) to improve an options selling strategy introduced by "Quant Galore" (https://quantgalore.substack.com/p/selling-volatility-the-right-way). 
According to Chan, we can use Machine Learning to predict the profitability of our next trade, which allows to vary exposure, reduce drawdowns and improve the strategy's performance.
I am aware that the history is very short, therefore using a cross-validation and walk-forward optimization only makes limited sense. This notebook is more a showcase of the conditional probability idea.

## Portfolio

### HERC
In this notebook we try to create a few simple long-only ETF Portfolios using different portfolio optimization methods.
The methods we will look at are: equal risk, Hierarchical Equal Risk Contribution (HERC) and a HERC with a momentum overlay.
The HERC optimization is based on the paper by: [Raffinot, Thomas, The Hierarchical Equal Risk Contribution Portfolio (August 23, 2018)](https://ssrn.com/abstract=3237540 )
The portfolio is then backtested and the results are compared. We try to create a diversified portfolio meanwhile keeping in mind transaction costs.

### ETF Sector Rotation
In this notebook we create a sector rotation strategy implemented with sector ETFs. 
The idea is taken from the post by: [Sector Momentum - Rotational System](https://quantpedia.com/strategies/sector-momentum-rotational-system/)
and uses Rob Carver's definition of momentum.

### Momentum
#### Carver
In this notebook we investigate a few ideas presented by [Rob Carver](https://qoppac.blogspot.com/p/about-me.html) <br>
We are especially interested in the momentum strategies suggested in his [latest book](https://www.systematicmoney.org/advanced-futures): EWMAC, Breakout, Skew 
