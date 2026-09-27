# Thomas Quinn

Final-year Actuarial and Financial Studies student at UCD (on track for First Class Honours), aiming at quantitative trading. Most of what I build is about financial markets: tools to trade, price and model them, and the testing to know when to trust them.

### What I'm working on

**A systematic trading system for Polymarket prediction markets.** It began as an open-source framework I built with a friend ([`Polymarket_trader`](https://github.com/Thomas-quinn7/Polymarket_trader)). Since then I have taken it private and built it out end to end, largely on my own:

- a live data layer streaming Polymarket order books and Binance prices, with around 40 scheduled services recording market data around the clock (150+ GB so far)
- pricing for short-dated crypto binaries as digital options under a Merton jump-diffusion, with volatility and jump intensity estimated live
- fractional-Kelly sizing with correlation haircuts, slippage-aware caps and drawdown circuit breakers
- a wall-clock backtester that runs the exact same strategy code as the live loop
- a statistical promotion gate (cluster-bootstrap confidence intervals, calibration checks, latency replay) that any strategy has to pass before it gets near real money
- a FastAPI dashboard over all of it

Roughly 140,000 lines of Python behind 3,800+ tests, paper trading unattended 24/7. It stays private because the execution stack and the strategies live there.

### Selected projects

- **[options-toolkit](https://github.com/Thomas-quinn7/options-toolkit)**: options analytics with the checks attached. JAX Black-Scholes and CRR American pricing, arbitrage-free SSVI vol surfaces fitted to bid-ask bands (butterfly and calendar conditions verified numerically, never assumed), a delta-hedged market-making simulator with GLFT quoting and adverse-selection experiments, a no-arbitrage scanner, and a daily option-chain capture feeding surface-dynamics studies. 132 offline tests.
- **[market-regime-detection](https://github.com/Thomas-quinn7/market-regime-detection)**: Markov-switching volatility regimes on the S&P 500, built to be look-ahead-free and tested for it. Filtered vs smoothed vs walk-forward probabilities, Student-t emissions from scratch, financial turbulence, the Kritzman absorption ratio with its false-alarm rate measured, point-in-time macro data (ALFRED first releases) and a costed regime-based allocation backtest.
- **[equity-forecasting](https://github.com/Thomas-quinn7/equity-forecasting)**: ARIMA (mean) and GJR-GARCH (volatility) forecasting with a walk-forward out-of-sample backtest, scored with QLIKE against EWMA and rolling baselines, with Mincer-Zarnowitz and Diebold-Mariano tests. The GJR-GARCH volatility forecasts beat both baselines on QLIKE for all three tickers.
- **[pairs-trading-toolkit](https://github.com/Thomas-quinn7/pairs-trading-toolkit)**: Engle-Granger cointegration screening, mean-reversion spread backtesting with carry costs and quarterly recalibration, paired block bootstrap and portfolio optimisation, with causality tests that corrupt future prices and check no earlier signal changes.
- **[Polymarket_trader](https://github.com/Thomas-quinn7/Polymarket_trader)**: the open-source framework layer of the system above. CLOB execution, wall-clock backtester, pre-trade slippage gate, probability-fed fractional-Kelly sizing, FastAPI dashboard, 816 tests.

### Toolkit

`Python` (NumPy Â· pandas Â· SciPy Â· statsmodels Â· JAX Â· pytest) Â· `R` Â· `SQL` Â· `Git` Â· options pricing Â· time-series Â· Kelly sizing

### Beyond the screen

Co-president of one of Ireland's largest college poker societies. Competed in RITC x Dublin (the Rotman International Trading Competition's Dublin event, hosted at Trinity College Dublin), live and in person, 6th of 100 teams. Actuarial internships at Aviva (two summers, group-protection pricing) and Grant Thornton (seconded to the BMA Regulator Data Analytics & AI team).

### Reach me

[LinkedIn](https://www.linkedin.com/in/thomassquinn/) Â· thomas.quinn3@ucdconnect.ie


Co-president of one of Ireland's largest college poker societies. Competed in RITC x Dublin (the Rotman International Trading Competition's Dublin event, hosted at Trinity College Dublin), live and in person, 6th of 100 teams. Actuarial internships at Aviva (two summers, group-protection pricing) and Grant Thornton (seconded to the BMA Regulator Data Analytics & AI team).

### Reach me

[LinkedIn](https://www.linkedin.com/in/thomassquinn/) Â· thomas.quinn3@ucdconnect.ie
