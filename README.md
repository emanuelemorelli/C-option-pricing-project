In this project, I implemented a Monte Carlo simulation to compute the theoretical price of an up-and-out barrier call option.
The theoretical price of the option is evaluated using the following parameters:
- Initial price of the underlying asset: S₀ = 100
- Strike price: K = 110
- Annualized volatility: σ = 25%
- Annualized risk-free interest rate: r = 5%
- Time to maturity: t = 0.75 years

Regarding the barrier level (B), I selected reasonable values that slightly affect the price compared to the corresponding vanilla call option, while avoiding configurations that would trivially drive the option price to zero.
To analyze the sensitivity of the option price to the barrier, I also performed experiments with different barrier levels.
For this reason, the barrier value is implemented as an additional data member of the option class, allowing flexibility and easy testing of alternative scenarios.
