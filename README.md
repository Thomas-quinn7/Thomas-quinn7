# Thomas Quinn

Actuarial & Financial Studies student at UCD (on track for First Class Honours), aiming at quantitative trading. Most of what I build is in relation to financial markets: Tools to trade, price and model them.

I build and test trading strategies and try just as hard to break them.

### What I'm working on

**A systematic trading system for Polymarket prediction markets** â€” data, execution, fractional-Kelly sizing, backtesting, risk, and a live dashboard. It began as an open-source framework I built with a friend ([`Polymarket_trader`](https://github.com/Thomas-quinn7/Polymarket_trader)); when the strategies started showing what looked like a real edge I took it private and rebuilt it end-to-end, largely solo, behind 3,700+ tests. It stays private because the live execution stack and the promotion-gate thresholds live there, and unfalsified candidate strategies still run against them â€” but the system's main output so far is public knowledge: the proof that the edge wasn't real. The part I learned most from wasn't a winning strategy â€” it was building the promotion gate that refused my own flagship strategy live capital, and the winner's-curse analysis that explained why.

### Selected projects

- **[options-toolkit](https://github.com/Thomas-quinn7/options-toolkit)** â€” options analytics with the checks attached: JAX Black-Scholes & CRR American pricing, arbitrage-free SSVI vol surfaces fitted to bidâ€“ask bands (butterfly/calendar conditions verified numerically, never assumed), a GLFT optimal market-making simulator with adverse-selection experiments, a no-arbitrage scanner, and a daily option-chain capture pipeline feeding surface-dynamics studies.
- **[market-regime-detection](https://github.com/Thomas-quinn7/market-regime-detection)** â€” Markov-switching volatility regimes on S&P 500 returns, built to be look-ahead-free and tested for it: filtered vs smoothed vs walk-forward probabilities (the look-ahead premium lives almost entirely in smoothing), Student-t emissions from scratch, absorption-ratio false-alarm accounting, point-in-time macro data (ALFRED first releases), and a costed regime-gated allocation backtest â€” null results published alongside the positive ones.
- **[equity-forecasting](https://github.com/Thomas-quinn7/equity-forecasting)** â€” ARIMA (mean) and GJR-GARCH (volatility) forecasting with a walk-forward out-of-sample backtest: QLIKE-scored against EWMA and rolling baselines, with Mincer-Zarnowitz and Diebold-Mariano tests. Headline honest finding: the ARIMA side loses to forecasting zero.
- **[pairs-trading-toolkit](https://github.com/Thomas-quinn7/pairs-trading-toolkit)** â€” Engle-Granger cointegration screening, mean-reversion spread backtesting with carry costs and quarterly recalibration, paired block bootstrap, and portfolio optimisation. The strict screen admits nothing on the current universe â€” a no-trade year is a result, not a failure.
- **[Polymarket_trader](https://github.com/Thomas-quinn7/Polymarket_trader)** â€” open-source Polymarket trading infrastructure: CLOB execution, wall-clock backtester, pre-trade slippage gate, probability-fed fractional-Kelly sizing with a no-signal floor, FastAPI dashboard, 816 tests.

### Toolkit

`Python` (NumPy Â· pandas Â· SciPy Â· statsmodels Â· JAX Â· pytest) Â· `R` Â· `SQL` Â· `Git` Â· options pricing Â· time-series Â· Kelly sizing

### Beyond the screen

Co-president of one of Ireland's largest college poker societies. Competed in RITC x Dublin (the Rotman International Trading Competition's Dublin event, hosted at Trinity College Dublin) â€” live and in person, 6th of 100 teams. Actuarial internships at Aviva (two summers, group-protection pricing) and Grant Thornton (seconded to BMA Regulator Data Analytics & AI team).

### Reach me

[LinkedIn](https://www.linkedin.com/in/thomassquinn/) Â· thomas.quinn3@ucdconnect.ie
