# ORBit Dashboard

A clean, single-file web dashboard for trading the **Opening Range Breakout (ORB)** strategy with directional **Fibonacci** levels. It streams real US market data and mirrors the logic of the companion TradingView Pine Script indicator.

## What it does
- **Live scanner** across your watchlist: price, % change, ORB bias (bullish/bearish), the opening range, key Fib levels, and breakout/failure status.
- **Chart** panel with an embedded TradingView chart for the selected symbol.
- **Alerts** feed for breakouts, breakdowns, and bias failures.
- **P&L tracker** to log trades and see win rate / totals.

## Getting started (about 1 minute)
1. Open the dashboard (`index.html`).
2. Click **Connect data** (top right).
3. Click **Get your free key** — it opens [Twelve Data](https://twelvedata.com/pricing). Create a free account (no card needed) and copy your API key.
4. Paste the key, click **Test & Save**. That's it — it's stored on your device, so you only do this once.

Each person uses their **own free key**, so there are no shared limits.

## How the data works
- Prices and opening-range bars come from the Twelve Data API (free tier).
- The Opening Range is captured once per session (default first 5 minutes; 15/30 selectable) and then locked, exactly like the indicator. Live price is polled while the market is open.
- When the market is closed, the dashboard shows the last session's data, clearly labeled.

## Notes
- No install, no build step — it's one HTML file. Open it locally or host it anywhere static.
- No account or login required; your settings live in your browser.
- Educational tool only — **not financial advice.**
