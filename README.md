# Creating & Optimizing Equity Portfolios (without rebalancing)

__Objectives:__

1. Generate a portfolio with random weights
2. Generate a portfolio with the Highest Risk Adjusted Return (RaR)
3. Generate a portfolio with the Maximum Return
4. Generate the efficient Frontier

<img width="896" alt="image" src="https://github.com/user-attachments/assets/ebfa6c2f-a60c-47cf-953c-db87cd0dd8bf">


<img width="925" alt="image" src="https://github.com/user-attachments/assets/c5ec9b40-a117-4066-98ac-11a174ba7c17">


__Method 1:__

1. Python assigns random weights from 0-1 for each stock, takes the sum of weights, then divide each weight by the sum to get it's portfolio weight
2. The return is the weight of each stock times the return it generated

   
__Method 2:__

1. We import 'scipy.optimize', for python to optimise what we want, be it the maximum return portfolio, or the one with the lowest risk.
   - We need a constraint function, and a function to input what we want to maximize or minimize



__Learnings from this Project__:
1. When using scipy.optimize, we can consider setting a minimum weight for each stock for each tuple.
   - Otherwise, the portfolio may consist of only 1 stock (in our case TSLA when optimising for maximum return). This rids us of diversification benefits
   - Furthermore, past performance is not indicative of future performance!   
