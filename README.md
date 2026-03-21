# 📈 Trading Terminal — @darrenhillofficial

A free, self-hosted trading dashboard with live market data. No backend, no frameworks — just one HTML file.

## Features

- **ETF Discount Tracker** — Buy-the-dip levels at 25/35/45% from all-time highs with mini charts
- **Breakout Screener** — Scans 50 large-cap stocks for 20-day and 52-week breakouts, filtered by P/E, P/B, D/E, ROE
- **Mean Reversion** — Draws SMA (50/100/200-day) and highlights below-mean buy zones with backtest alpha
- **Metals Portfolio** — Equal-weight gold, silver, copper, platinum, uranium with custom start date, rebalancing, correlation matrix
- **Compound Calculator** — Model DCA + discount entry + compound growth over time
- **Market Sentiment** — Fear & greed gauge using VIX, SPY, GLD, TLT
- **Sector Heatmap** — All 11 S&P sectors sized by weight, coloured by daily change
- **Alert System** — Browser notifications, sound alerts, and visual banners when discount tiers trigger
- **Dark/Light Theme** — Global toggle, persists across sessions

## Quick Start (Local)

1. Download `index.html`
2. Open it in Chrome, Firefox, or Safari
3. Click the 🔑 button and enter your free [Finnhub API key](https://finnhub.io/register)
4. Data starts loading automatically

## Deploy to GitHub Pages (Free Hosting)

1. **Create a new repository** on GitHub (e.g. `trading-terminal`)
2. **Upload `index.html`** to the root of the repository
3. Go to **Settings → Pages**
4. Under **Source**, select `main` branch and `/ (root)` folder
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/trading-terminal/` within 1-2 minutes

### To Update

Just replace `index.html` in the repo — GitHub Pages auto-deploys on every push.

## API Key

This terminal uses [Finnhub](https://finnhub.io) for live market data. The free tier gives you:
- 60 API calls per minute
- Real-time US stock quotes
- Historical candle data
- Company fundamentals

Sign up at [finnhub.io/register](https://finnhub.io/register) — no credit card required.

Your API key is stored in your browser's localStorage (never sent anywhere except Finnhub).

## Customisation

- **Edit ETFs**: Click the ✎ ETFs button to add/remove tickers and change discount tiers
- **Adjust filters**: The screener filters (P/E, P/B, etc.) are all adjustable in real-time
- **Change metals start date**: Pick any date or use the quick presets (1yr, 2yr, 3yr, 5yr, 10yr)
- **Theme**: Toggle dark/light with the moon/sun button — persists via localStorage

## Tech Stack

- Pure HTML/CSS/JavaScript — no build step, no dependencies, no Node.js
- Canvas API for all charts (no charting libraries)
- Finnhub REST API for live data
- localStorage for settings persistence

## Notes

- Free Finnhub tier: 60 calls/min — data loads progressively (~3s per ETF)
- Works best during US market hours; weekends show previous close
- The screener scans 50 stocks and takes ~4 minutes on free tier
- Not financial advice — past performance doesn't guarantee future results

## Author

**@darrenhillofficial** — [Instagram](https://instagram.com/darrenhillofficial)

---

*Built with data from [Finnhub](https://finnhub.io). Not affiliated with any financial institution.*
