## Markowitz’s Efficient Frontier & Portfolio Optimization with Python

This project is part of the course *"Programming - Introduction Level"* at the University of St. Gallen (HSG). The purpose is to construct a so-called *“Efficient Frontier”* (Markowitz, 1952) and implement a stock portfolio optimization in Python for a specific time period using real stock data. Moreover, we want to find the composition of the maximum Sharpe ratio (Sharpe, 1966) portfolio as well as the minimum variance portfolio. 

Afterwards, the theoretical background and the structure of the code are explained.

### Context 
Harry M. Markowitz is a 1990 Nobel prize winner for being a pioneer of the Modern Portfolio Theory (MPT), which deals with how investors should construct investment portfolios in order to the expected returns for given levels of risk. 

Assumptions of MPT:
- Investors are rational and avoid risks whenever possible.
- Investors aim for the maximum returns for their investment.
- All investors share the aim maximizing their expected returns.
- Commissions and taxes on the market are left out of consideration.
- All investors have access to the same sources and level of all necessary information about investment decisions
- Investors have unlimited access to borrow and lend money at the risk free rate (for simplicity's sake a risk free rate of 0% is assumed for this project).

### The concept of the Efficient Frontier
According to the theory, it is possible to build an "efficient frontier", which graphically represents the optimal portfolios that offer the highest possible expected return for a given level of risk. This is based on the principle of diversification, i.e. the reduction of the portfolio's risk (standard deviation) by adding additional assets to the same portfolio. In practice, an investor tries to populate the portfolio with securities that offer high returns, but whose combined standard deviation is less than their individual standard deviations. If the optimization of the return/risk paradigm is successful, the portfolio aligns along the efficient frontier. If there are portfolios with higher returns for the same level of risk, the portfolio is not optimal and lies below the efficient frontier.

The following diagram gives an overview of this concept: ![Alt Text](https://github.com/pescestefano96/Programming-Project/blob/master/Efficient_frontier0.jpg)

Two portfolios along the efficient frontier are of particular interest: 
-	The portfolio that maximises the Sharpe ratio, i.e. the ratio of return to risk; and
-	The portfolio that minimizes variance and thus risk for the investor.

### Building an Efficient Frontier in Python
1.	Identify the assets to be considered in the portfolio.

2.	Identify the desired period of analysis.

3.	Calculate the return and covariance of the assets in the portfolio.

4.	Implement the Monte Carlo method to perform 50'000 simulations. Each simulation corresponds to a portfolio composed of the selected assets, for which every time different weights are randomly generated (making sure that the sum of the weights is 100%). Then calculate on the basis of them, the return, the volatility and the Sharpe Ratio for each of the randomly generated portfolios.

5.	Plot the efficient frontier: create a scatter plot with the combinations of returns and volatility obtained, highlighting the portfolio that maximizes the Sharpe ratio and the portfolio that minimizes the variance. In addition, it is also possible to color the data according to the Sharpe Ratio of each portfolio, to have a visible measure of comparison.

6.	Get the data for the two portfolios of interest: the max-sharpe-ratio portfolio and the min-variance-portfolio.

### How to use
1. Make sure that you have installed all the necessary modules.

2. When runing the code, you will be asked for how many stocks you want to analyze. When this is done, you have to input their tickers name. Yahoo finance is used to get the data, so make sure your tickers correpsond to the exiting ones on https://finance.yahoo.com/.

3. For the time frame of analysis, enter the desired starting date and the desired ending date under the format: YYYY-MM-DD.

Depending on the compiler you're using, you may have to close the efficient frontier window to get the optimization of the two desired portfolios to appear.

### Expected outcome
The expected outcome is a graphical representation of the efficient frontier, displaying the maximum Sharpe ratio portfolio as well as the minimum variance portfolio according to the stocks and time frame of your inputs. In addition, for these two portfolios, you will see the return, volatility, sharpe ratio and stock weights.

#### Example
Let's use 4 stocks: *Apple (AAPL); Credit Suisse (CS); AMAZON (AMZN); UBS (UBS).*
The time frame is from 2010-10-10 until 2019-11-05.

Outcome: ![Alt Text](https://github.com/pescestefano96/Programming-Project/blob/master/Efficient_frontier.png)

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
The project is inspired by and took part of the code from:
- https://medium.com/python-data/effient-frontier-in-python-34b0c3043314
- https://medium.com/python-data/efficient-frontier-portfolio-optimization-with-python-part-2-2-2fe23413ad94

### Enjoy 😊📈
