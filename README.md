# Stock_Price_Prediction_Model_MSFT_Ticker
Model the randomness of the stock price and help us assess the uncertainty of the investment.
Monte Carlo Simulations are used to forecast stock prices
Stock returns have a random process. Any future changes are based on new random information.
Monte Carlo simulations help us model the random processes over time.
We need to generate plausible scenarios while watching the price evolve over a 250-day period.
That means That means 250 consecutive daily returns.

Simple Return = (Pt-Pt-1) /Pt-1
Simple returns are not additive, which makes them difficult to work with.
Simple returns are not symmetric. Simple returns cannot be approximated by a normal distribution.

Log Returns to the Rescue
The benefits of log returns:
• Time additive: The log returns over the whole period are equal to the sum of the log returns over the period.
• Symmetric: The upside and downside movements are more balanced.
• The log returns are assumed to be more closely represented by a normal distribution.

Steps
1. Place the historical stock prices into a pandas dataframe
2. Create a dataframe of daily log returns
3. Plot a distribution of returns to confirm assumptions
4. Calculate the historical statistical measures of the daily log returns
5. Simulate price movements over the next 250 days (random log returns)
6. Convert Log returns into simple returns
7. Calculate the price progressions for each simulations
8. Repeat the simulation 10,000 times
9. Quantify the best, worst, and average stock price scenarios and the distribution of the outcomes.
