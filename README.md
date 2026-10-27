# spy put premium

A single Jupyter notebook that asks what a short SPY put is really paid for.

It values SPY puts under real-world probabilities with filtered historical simulation, tests whether those values are
calibrated, and measures how much the market pays above them, from 1.2 times the value at the money to 2.3 times at
5-delta. It then splits the daily P&L of a delta-hedged 15-delta put into time decay, realised moves, vega and costs,
and shows that the trade is variance carry. Every method is demonstrated on synthetic data that runs live, and the
results on 2012–2025 SPY option chains enter as aggregate tables.

Open [spy_put_premium.ipynb](spy_put_premium.ipynb) to read it with all outputs, or run it top to bottom with `numpy`,
`scipy`, `pandas` and `matplotlib` installed.
