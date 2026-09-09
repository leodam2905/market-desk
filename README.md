# Market Desk

A single-file stock watchlist and market screener that runs entirely in your browser.

- **Watchlist** — live quotes, portfolio value and P/L, volume and relative volume
- **Movers** — ranks the whole US market (~12,500 tickers) by gainers, losers, dollar volume,
  12-1 momentum, or earnings surprise
- **Detail drawer** — 30-day trend, SMA 20/50/200, RSI(14), MACD, 52-week range, ATR(14),
  earnings history and recent news

## Setup

Open the page and paste two free API keys:

| Provider | Used for | Free tier |
|---|---|---|
| [Finnhub](https://finnhub.io/register) | real-time quotes, news, earnings | 60 calls/min |
| [Polygon](https://polygon.io/dashboard/signup) | market-wide daily bars, price history | 5 calls/min, end-of-day |

Either key alone works; features enable as keys are added.

## Notes

Keys are stored in your browser's local storage and sent directly to each provider over HTTPS.
There is no backend and no build step — it's one HTML file with no dependencies.

Polygon's free tier is end-of-day, so Movers reflects the last *completed* trading day.

This is a research tool, not investment advice.
