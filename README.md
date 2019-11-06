## Markowitz’s Efficient Frontier & Portfolio Optimization with Python

This project is part of course *"Programming - Introduction Level"* at the University of St. Gallen, HSG.

### Context 
Harry M. Markowitz is a 1990 Nobel prize winner for being a pioneer of the Modern Portfolio Theory (MPT) which is about how investors construct portfolios that maximise their expected returns for given levels of risk. 


### Assumptions of MPT
- Investors are rational and avoid risks whenever possible
- Investors aim for the maximum returns for their investment
- All investors share the aim maximizing their expected returns
- Commissions and taxes on the market are left out of consideration
- All investors have access to the same sources and level of all necessary information about investment decisions
- Investors have unlimited access to borrow and lend money at the risk free rate


### How to use
1. Make sure that you have installed all the necessary modules

2. When runing the code, you will be asked for how many stocks you want to analyze. When this is done, you have to give their tickers name. We are using yahoo finance to get our datas, so make sure your tickers correpsond to the exiting ones on https://finance.yahoo.com/.

3. For the time frame to analyze, enter the desire starting date and then ending date under the format: YYYY-MM-DD


### Expected outcome

A graphical representation of the efficient frontier will appear, displaying the minimun variance portfolio as well as maximum sharpe ratio portfolio according to the stocks and time frame of your inputs.
In addition to this, for both portfolios, the return over the period, volatility, sharpe ratio as well as the weights of each stocks within your portfolio will be displayed.

### Example

Let's use 4 stocks: *Apple (AAPL); UBER (UBER); UBS (UBS); Credit Suisse (CS).*
The time frame: 2010-10-10 until 2019-11-05

Efficient frontier: ![Alt Text](https://github.com/pescestefano96/Programming-Project/blob/master/Efficient_frontier.png)

**The sharpe portfolio is:** 

- **Returns**       0.236359
- **Volatility**    0.258548
- **Sharpe Ratio**  0.914177
- **AAPL Weight**   0.887478
- **CS Weight**     0.077132
- **UBER Weight**   0.011053
- **UBS Weight**    0.024337
                
**The minimum variance portfolio is:**

- **Returns**      0.119080
- **Volatility**    0.224987
- **Sharpe Ratio**  0.529274
- **AAPL Weight**   0.624847
- **CS Weight**     0.341588
- **UBER Weight**   0.032467
- **UBS Weight**    0.001098


### Credits

We inspired ourselves and took some of the code from:

- https://medium.com/python-data/effient-frontier-in-python-34b0c3043314
- https://medium.com/python-data/efficient-frontier-portfolio-optimization-with-python-part-2-2-2fe23413ad94

### Enjoy 😊📈
