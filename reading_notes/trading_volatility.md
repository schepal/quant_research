# Trading Volatility by Colin Bennett


## Chapter 3 - Why Everything You Think You Know About Vol Is Wrong

- A short vol position is correlated with to the equity markets and is implicitly long equity risk.
- Implied volatility on average is overpriced on average due to hedging demand from investors
- Far-dated options are most overpriced due to upward term sloping term structure. ie: selling 12 x one month option earns more than 1 x one year option (but risk is much higher for selling front-month contracts)

### Why Volatility is Overpriced
- Demand for Put Protection: demand for hedging products from investors
- Demand for OTM options lifts wings: market-makers have to bid up the price on these "lotto ticket" OTM options.
- Index Implied Volatility Lifted From Structured Products: Demand from structured products increase overall index IV relative to single-stock IV.


### Long Volatility is a Poor Hedge
- Outright long-volatility exposure is expensive and not a good hedge against market turbulence
- Equity markets are more volatile when they decline and less volatile when they rise --> decrease in equity value of a company increases its leverage.
- Long volatility is inherently short equity risk - thereby being long vol is expected to have negative returns on average


### Stretching Black-Scholes Assumptions

1. Continuous delta-hedging with known volatility: profit/loss from vol trading is fixed. Unrealistic assumption that volatility is constant. There is a very strong relationship between gamma and theta - i.e, theta pays for gamma.
  -  Profit from delta-hedging = Price - Theoretical Price
  - Hedging with delta when volatility is known results in constant profit/loss

2. Continuous delta-hedging with unknown volatility: traders hedge with delta calculated using IV:

  - IV commonly used to calculate deltas. This introduces equity market risk as position now becomes path dependent as we do not know the true volatility.
  - Large potential for variation in profit/loss if there is a significant difference between implied and realized volatility.

3. Discrete delta hedging with known volatility: variance of payout inversely proportional to how frequent we delta-hedge.

  - Continuous delta-hedging is not practical in the real-world
  - In trending markets, it is more profitable to let positions run and re-hedge less frequently

4. Discrete delta hedging with unknown volatility: most realistic assumption. Payout is sum of variance due to hedging with unknown volatility plus variance due to discretely delta hedging.

  - Better to use expected volatility rather than implied volatility when calculating greeks for hedging positions.
