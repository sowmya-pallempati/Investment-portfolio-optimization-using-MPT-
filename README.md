**Problem Statement**

In this project, we have created an investment portfolio using Modern Portfolio Theory (MPT). This portfolio is designed to predict risk and profit by enhancing the value of a stock over a period of time.
Optimized allocations across different sectors by bringing out top three best-performing stocks.

**Sectors choosen:**
1. Industrials Sector
2. Financials Sector
3. Materials Sector
   
**Stocks choosen based on Linear Regression:**
Industrials Sector ['FDX', 'ROL', 'PAYC']
Financials Sector ['WFC', 'CMA', 'AIG']
Materials Sector ['CF', 'NUE', 'MOS']

**Portfolio Optimization Model Setup**
In this section, we establish an optimization model to allocate investments across the sectors using Bonmin:

1. Defining variables for the covariance and the mean of stocks.
2. Specifying the Concrete Model.
3. Defining decision variables and the bounds (between 0 and 1).
4. Defining constraints.
5. Defining objective function.

**Stock Allocation with respect to Different Risk Levels**

![image](https://github.com/sowmya-pallempati/Investment-portfolio-optimization-using-MPT-/assets/112984551/0280cba9-6d24-4381-8ec5-5d9393dccb99)

![image](https://github.com/sowmya-pallempati/Investment-portfolio-optimization-using-MPT-/assets/112984551/536077de-211d-4f87-9de7-0bf2400373d2)

**Buy & Hold Strategy for MPT Portfolio Allocation**

Calculating how much money to invest in each stock of the portfolio, making sure to spread out the investment evenly according to the MPT allocation.
Then, we are printing out the allocated amounts for each stock, ensuring a balanced investment strategy.

**Buy & Hold Strategy Performance for MPT Stock Allocation Strategy**

**Volatility:** The strategy experienced significant volatility, with monthly returns ranging from -0.1044 to 0.1257.

**Positive and Negative Months:** There were 5 months with positive returns and 5 months with negative returns.

**Consecutive Monthly Returns:** The strategy experienced both positive and negative consecutive monthly returns, with a maximum consecutive return of 0.149962 and a minimum of -0.074354.

**Cumulative Return:** Over the entire period, the strategy returned 25.67% (from 89558.054876 to 112569.367303).

**Buy & Hold strategy for the S&P 500 index (^GSPC)**

Retrieving the adjusted close prices of the S&P 500 index to analyze its performance during the specified period.
This data allows us to assess how investing in the S&P 500 index would have performed over the given timeframe, facilitating comparisons with other investment strategies.

![image](https://github.com/sowmya-pallempati/Investment-portfolio-optimization-using-MPT-/assets/112984551/4c80ed12-51d6-4168-9163-498c984af687)

**Comparision of MPT Stock Allocation & SP500 Buy & Hold Strategies**

**Monthly Returns:** The MPT strategy generally outperformed the SP500 Buy & Hold strategy in terms of monthly returns, with an average monthly return of -0.0156% compared to -0.1041% for the SP500.
Consecutive Monthly Returns: The MPT strategy showed more consistent performance, with a maximum consecutive monthly return of 0.149962, while the SP500 had a maximum consecutive monthly return of 0.091116.

**Volatility:** The SP500 Buy & Hold strategy experienced higher volatility, with a standard deviation of monthly returns of 0.1389, compared to 0.0649 for the MPT strategy.

**Cumulative Returns:** Over the entire period, the MPT strategy returned 12.56%, while the SP500 Buy & Hold strategy returned -19.95%.

The MPT stock allocation strategy outperformed the SP500 Buy & Hold strategy in 2022, with more consistent returns, lower volatility, and higher cumulative returns. 
This suggests that the MPT strategy was more effective in managing risk and maximizing returns over this period. However, it's essential to note that past performance is not a guarantee of future results, and both strategies carry inherent risks and uncertainties.

**Recommendation:** Investors may consider incorporating MPT principles into their investment approach, diversifying their portfolios, and regularly rebalancing to manage risk. 
However, it's crucial to consult with a financial advisor and conduct thorough research before making investment decisions.

**MONTE CARLO SIMULATION**

![image](https://github.com/sowmya-pallempati/Investment-portfolio-optimization-using-MPT-/assets/112984551/8762dd16-f038-4be4-abaf-4b23434b6dde)

![image](https://github.com/sowmya-pallempati/Investment-portfolio-optimization-using-MPT-/assets/112984551/802a3b12-3472-46b1-b249-cdef232a3abb)

Investing in stocks with a high probability of losing money carries a higher risk of loss compared to others in the portfolio.

**Based on the Monte Carlo simulation results, we can say that:**

**Overall Portfolio Risk:** The probability of the portfolio losing money is relatively low, at 3.8% (0.038). 
This suggests that the portfolio has a high likelihood of generating positive returns.

**Individual Stock Risk:** The probabilities of each stock losing money vary significantly, ranging from 13.9% (PAYC) to 40.5% (CMA and FDX). This highlights the importance of diversification, as some stocks are more risky than others.

**Diversification Benefits:** The overall portfolio risk is significantly lower than the individual stock risks, demonstrating the benefits of diversification. This is because the portfolio's returns are spread across multiple stocks, reducing the impact of any one stock's potential losses.

**CONCLUSION**
1. Effective investment strategies strive for maximizing returns while minimizing risks, though there's inevitably a balance to strike.
2. It's crucial to keep a constant eye on investment strategies to spot underperforming stocks. Strategies should be flexible, allowing for adjustments based on changing market conditions and asset performance.
3. Monte Carlo simulations provide forecasts of future stock performance based on historical data. These forecasts can help investors set realistic expectations and develop appropriate investment strategies.
4. It is smart to invest in stocks that have positive returns and a low probability of losing money. Based on our analysis investing in "PAYC" stock will have higher returns and lower risk while investing in "FDX" has higher risk to lose money
5. Learned how to create effective models that automate in finding stocks that are profitable to invest in with lower risk. Aiming to become as good as David Bergman.
6. Based on efficient frontier, we have observed that CMA, PAYC and ROL are the 3 stocks that are better suited to be allocated in the portfolio.
7. We learned to integrate optimization solvers like Bonmin into our portfolio optimization. This helped us understand how these tools search for the best solutions, making it easier to find the right investment mix for our needs.
8. By trying out the Buy-and-Hold strategy for both the MPT portfolio and the S&P 500 index, we learned a lot about long-term investing. which showed us how important it is to choose the right mix of assets and how market changes can affect investment outcomes. Moreover, Comparing these strategies also helped us see the pros and cons of actively managing a portfolio versus simply investing in an index.




   
