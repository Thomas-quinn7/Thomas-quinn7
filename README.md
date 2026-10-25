# Thomas Quinn

I am a final-year Actuarial and Financial Studies student at UCD in Dublin, on track for First Class Honours, and I am applying for a masters in statistics and quantitative finance to start in September 2027. I am very keen to work in quantitative research and trading. Most of my projects ask the same question, whether a model really beats a simple baseline once look-ahead bias and multiple testing are dealt with properly, and I report the answer either way.

### Research projects

- **Prediction-market pricing (private).** Can a model-based edge in 5-minute crypto contracts on Polymarket survive honest out-of-sample testing? The model prices them as digital options under a Merton jump-diffusion, and every strategy has to pass a promotion gate (cluster-bootstrap confidence intervals and calibration checks) before it could go near real money. The gate refused my own strategy. It ranked outcomes well but its probabilities were badly miscalibrated, and across 245,000+ signals the claimed edge was negative or not distinguishable from zero in every edge bucket, which is a winner's curse. It has only ever traded on paper. The open-source framework underneath is [`Polymarket_trader`](https://github.com/Thomas-quinn7/Polymarket_trader), started with [Ciaran McDonnell](https://github.com/CiaranMcDonnell).
- **[market-regime-detection](https://github.com/Thomas-quinn7/market-regime-detection)**: can a Markov-switching regime model forecast volatility better than the simple measures it competes with? The main claims were tested on four holdouts whose protocols were committed before the data was opened, and each holdout was run once. The answer was no. Adding a regime probability to a HAR forecast with implied volatility never made a measurable difference, and the write-up shows why the two-state probability behaves like a squashed EWMA volatility.
- **[equity-forecasting](https://github.com/Thomas-quinn7/equity-forecasting)**: ARIMA (mean) and GJR-GARCH (volatility) forecasts scored walk-forward out of sample against EWMA and rolling baselines. GJR-GARCH had the lowest QLIKE on all three tickers, however the Diebold-Mariano test against EWMA is significant at 5% on only two of the three, and neither survives a Holm correction.
- **[options-toolkit](https://github.com/Thomas-quinn7/options-toolkit)**: Black-Scholes and Greeks in JAX, arbitrage-free SVI/SSVI volatility surfaces fitted to bid-ask bands (butterfly and calendar conditions checked numerically), a delta-hedged market-making simulator with GLFT quoting and adverse selection, and surface studies on a small dataset of option chains captured since July 2026.
- **[pairs-trading-toolkit](https://github.com/Thomas-quinn7/pairs-trading-toolkit)**: Engle-Granger cointegration screening and a mean-reversion spread backtest with carry costs and quarterly recalibration, with tests that corrupt future prices and check that no earlier signal changes.

### Toolkit

`Python` (NumPy · pandas · SciPy · statsmodels · JAX · pytest) · `R` · `SQL` · `Git` · time series · volatility forecasting · bootstrap inference · calibration · options pricing

### Beyond the screen

President of the UCD Poker Society, running weekly tournament nights. Competed with my team in RITC x Dublin 2025 (the Rotman International Trading Competition's Dublin event, hosted at Trinity College Dublin), live and in person, finishing 6th of 100 teams. Actuarial internships at Aviva (two summers, group protection pricing) and Grant Thornton (seconded to the BMA Regulator Data Analytics & AI team).

### Reach me

[LinkedIn](https://www.linkedin.com/in/thomassquinn/) · tq3435@gmail.com
