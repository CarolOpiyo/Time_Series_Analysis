# Time_Series_Analysis
GARCH
The GARCH model is the generalised ARCH model is used to predict volatility. The equation of the GARCH model is:

σ2t+1=α0+α1∗r2t+β1∗σ2t 

where:

σ2t+1  is the ARCH predicted variance,
r2t  is the current period returns,
α0  is a constant,
α1  is the autoregressive coefficient and
β1  is the conditional regression coefficient.

The GARCH model in Python is implemented using the `arch_model` function. The syntax is shown below.

Syntax: 
```python
arch_model(historical_data, vol='GARCH', p=AR_order, q=MA_order, dist=distribution_of_the_data)
```
1. `historical_data`: Historical data whose volatility is to be predicted
1. `vol='GARCH'`: Type of model to use
1. `AR_order`: The AR order (p) of the GARCH(p,q) model
1. `MA_order`: The MA order (q) of the GARCH(p,q) model
1. `distribution_of_the_data`: distribution of the input data. Empirically, for most financial data, this is Skewed Student’s-t distribution or 'skewt'
