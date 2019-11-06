## Markowitz’s Efficient Frontier & Portfolio Optimization with Python

This project is part of course *"Programming - Introduction Level"* at the University of St. Gallen, HSG.

### Context 

Harry M. Markowitz is a 1990 Nobel prize winner for being a pioneer of the Modern Portfolio Theory (MPT) which is about how investors construct portfolios that maximise their expected returns for given levels of risk. 

Our aim is to showcase to the user the efficient frontier of desired stocks within a specific perido as well as the composition of the sharpe portfolio as well as the minimum variance portfolio.

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

(Depending on the compiler you use, you may have to close the efficient frontier window to get the optimization of the two desired portfolios to appear)

### Expected outcome

A graphical representation of the efficient frontier will appear, displaying the minimun variance portfolio as well as maximum sharpe ratio portfolio according to the stocks and time frame of your inputs.
In addition to this, for both portfolios, the return over the period, volatility, sharpe ratio as well as the weights of each stocks within your portfolio will be displayed.

### Example

Let's use 4 stocks: *Apple (AAPL); Credit Suisse (CS); AMAZON (AMZN); UBS (UBS).*
The time frame: 2010-10-10 until 2019-11-05

Efficient frontier: ![Alt Text](https://github.com/pescestefano96/Programming-Project/blob/master/Efficient_frontier.png)

**The sharpe portfolio is:** 
   
- **Returns**       0.290213
- **Volatility**    0.237612
- **Sharpe Ratio**  1.221374
- **AAPL Weight**   0.512437
- **CS Weight**     0.003984
- **AMZN Weight**   0.470743
- **UBS Weight**    0.012836
                
**The minimum variance portfolio is:**
 
- **Returns**       0.188358
- **Volatility**    0.213229
- **Sharpe Ratio**  0.883357
- **AAPL Weight**   0.463220
- **CS Weight**     0.264923
- **AMZN Weight**   0.271718
- **UBS Weight**    0.000138


### Credits

We inspired ourselves and took some of the code from:

- https://medium.com/python-data/effient-frontier-in-python-34b0c3043314
- https://medium.com/python-data/efficient-frontier-portfolio-optimization-with-python-part-2-2-2fe23413ad94

### Enjoy 😊📈
