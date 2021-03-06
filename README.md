# Simulation Codes : Markov Chain, GBM for retirement portfolio, HMC, Discretization Schemes, Greeks via Simulation

## Markov chain Part A : 
Consider a Continuous-Time Markov Chain with finite states S = {0,1,2,...N) and some given transition matrix. Assuming the waiting time, 
H_i has an exponential distribution at rate - <img src="https://latex.codecogs.com/gif.latex?\lambda&space;_{i}" title="\lambda _{i}" />  The input to the code is: (a) initial state, (b)
T, (c) transition probability matrix P which is an (N+1)x(N+1) matrix and (d) <img src="https://latex.codecogs.com/gif.latex?\lambda&space;_{i}" title="\lambda _{i}" /> for  for i = 0,1,2,...N. 
Output would be (a) tj switching times and (b) states at those times.

## Saving for Retirement (GBM simulation) Part B :
(Saving for retirement) This question asks you to use Monte Carlo simulation to investigate various
investment strategies for retirement savings. For simplicity, assume that the S&P500 index follows
the usual Black-Scholes assumptions with a mean return of 7% (per year) and a standard deviation
of 23% (per year) and zero dividends. Assume further that there is a constant riskless interest rate
of 3%, and that there is no inflation (ever).
Suppose that the worker starts saving for retirement at age 30, retires at 65, and lives to 85.
Suppose that the worker earns $100,000 per year. (Income stays constant over time for simplicity
and for consistency with the zero in ation assumption.) Assume that the worker invests 10% of
his/her earnings at the end of each year. To make the timing of cash-flows precise, assume that
the worker's 30th birthday is January 1, 2018, that the worker makes the rst payment of $10,000
on January 1, 2019, and that the worker retires at 65 on January 1, 2053. The worker's goal is to
have $1,000,000 in his/her account by age 65 on January 1, 2053.
This question asks you to compare investment strategies S1, S2, S3 (below) based on Monte
Carlo simulation using 10,000 trials:
####  S1: Invest 100% in the risk-free asset;
####  S2: Invest 100% in the S&P index;
####  S3: Re-balance the portfolio at the beginning of each period so that 50% is invested in the S&P
####  index and 50% is invested in the risk-free asset.
(a) For each strategy, estimate the mean, standard deviation, 10th, 50th, and 90th percentiles
of the portfolio value at the beginning of retirement (i.e., at age 65 on January 1, 2053).
Also, for each strategy estimate the probability that the portfolio value exceeds the target of
$1,000,000. Give standard errors for the mean and the probability of exceeding the target.

(b) Propose and analyze a new strategy (call it S4) which has the highest probability of exceeding
the target that you can determine. The worker cannot borrow and can only re-balance his/her
portfolio on January 1 of each year. Your new strategy could (i) use different constant
proportions in the S&P index and the risk-free asset, or (ii) vary the proportions in the S&P
index and the risk-free asset over time. You do not need to attempt any formal optimization
here | just think about the objective, try to come up with some reasonable strategies, and
see how much better you can do than strategies S1, S2, S3.

(c) Now, assume that the worker only makes an initial payment of $10,000 on January 1, 2018, and
makes no subsequent payments. For each of strategies S2 and S3, use Monte Carlo simulation
(again with 10,000 trials) to estimate the probability that the worker, by age 65, reaches
double his initial wealth ($20,000) before reaching half of his/her initial wealth ($5,000). Give
standard errors of your estimates. Explain how you are handling paths that neither double
nor halve by the end of the simulation time horizon.


# Hamiltonian Monte Carlo (HMC) Part C:
Simulate the following distribution:
f(x,y) = 1/2 : -1 < x < 0  & -1 < y < 0
       = 1/2 :  0 < x < 1 & 0 < y < 1

# Pricing Heston using various discretization schemes Part D:
Simulate stock pricing using heston model and princing a call option. 
Used Euler, Milstein and Runge-Kutta to simulate the model.

# Calculating Greeks via Simulation Part E
Calculation of Greeks for following type of options:
(a) Digital Call, (b) Up-and-
Out Call, (c) Average Option Call
spot price of S0 = 100, strike price of K = $115, risk-free rate
r = 0:04, continuous divided rate of q = 0:015, volatility of sigma = 0:28 for all options, maturity of T = 1 year for all options , barrier of H = 130 for up-and-out call, m = 12 monitoring times for average option.
