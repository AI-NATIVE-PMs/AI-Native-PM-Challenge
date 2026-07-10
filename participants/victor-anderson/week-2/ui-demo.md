# UI Demo — Verdant Fintech Dashboard

**Live app:** https://fintech-dashboard-pi-one.vercel.app/

## Screens

| Route | What it shows |
| --- | --- |
| `/` | Overview — stat cards, live markets, performance chart, allocation, AI insights |
| `/portfolio` | Holdings table with price, quantity, value, 24h change, allocation |
| `/markets` | Searchable + filterable markets table (Crypto / Livestock) |
| `/livestock` | Front-month cattle/hog cards + a futures curve table |
| `/ai-insights` | Grid of AI signal cards with confidence bars |
| `/alerts` | Toggleable price/signal alerts (interactive state) |
| `/settings` | Editable profile form + notification toggles |
| `/support` | Contact channels + expandable FAQ |

## Requirements coverage

- **Live prices (mock)** — the Live Markets strip re-prices BTC, ETH, Live Cattle,
  and Lean Hogs every 3 seconds.
- **Dark mode toggle** — top-bar toggle using `next-themes`, defaults to system
  preference.
- **Fully responsive** — sidebar collapses to a drawer on mobile/tablet; card grids
  reflow 1 → 2 → 4 columns; tables scroll horizontally on small screens.

## How to run locally

```bash
git clone https://github.com/techninja257/fintech-dashboard.git
cd fintech-dashboard
npm install
npm run dev      # http://localhost:3000
```

## Suggested demo flow (for the Sunday review)

1. Open the Overview and let the Live Markets prices tick.
2. Toggle dark mode in the top bar.
3. Resize the window (or open on a phone) to show the sidebar collapse into a drawer.
4. Go to Markets and use the search + Crypto/Livestock filter.
5. Toggle an alert on the Alerts page to show interactive state.
