# Week 2: Vibe Coding and Production UI

## Challenge Summary
A real-time analytics dashboard for a fintech app — "Verdant" — showing live
(mock) crypto and livestock-futures prices, a portfolio performance chart, and
AI-style investment insights, with a dark-mode toggle and full responsiveness.

## Live URL
https://fintech-dashboard-pi-one.vercel.app/

## GitHub Repository
https://github.com/techninja257/fintech-dashboard

## Key Metrics
- **Pages shipped**: 8 (Overview, Portfolio, Markets, Livestock, AI Insights, Alerts, Settings, Support)
- **Lint errors**: 0 (`next lint` / `eslint` passes clean)
- **Breakpoints supported**: mobile, tablet, desktop (sidebar collapses to a drawer < `lg`)

## What I Built
Verdant is a multi-page dashboard built on Next.js 16 (App Router) and Tailwind
CSS v4. All pages share one app shell:

- A **responsive sidebar** that becomes a slide-in drawer on smaller screens, with
  active-route highlighting.
- A **top bar** with search, notifications, a working **dark-mode toggle**
  (`next-themes`, class-based), and the user profile.

The **Overview** page is built in full: KPI stat cards, a **Live Markets** strip
that ticks every 3 seconds over mock data (BTC, ETH, Live Cattle, Lean Hogs), a
**Recharts** portfolio-performance area chart with a benchmark line and 7D/30D/90D
range toggle, an asset-allocation bar, and an AI-insights feed with sentiment
badges and confidence bars.

The remaining seven pages are minimal but functional: a searchable/filterable
markets table, a livestock futures curve, an AI-insights grid, toggleable alerts,
an editable settings form, and a support/FAQ page.

## Challenges & Solutions
1. **Challenge**: The starter had two conflicting `app/` directories and a broken,
   half-pasted `page.tsx` that didn't compile.
   **Solution**: Consolidated to a single `src/app/` tree, fixed the `@/*` path
   alias, and rewrote the page as a valid client component.

2. **Challenge**: Recharts v3 changed its tooltip typings, breaking the type check
   for the custom tooltip.
   **Solution**: Switched to the `TooltipContentProps` type, passed the tooltip as
   a render function, and coerced payload values to numbers.

3. **Challenge**: Dark mode didn't respond to the toggle.
   **Solution**: The CSS used `prefers-color-scheme` while `next-themes` was set to
   `attribute="class"`; moved to a class-based `.dark` variant so the toggle drives it.

## Key Learnings
1. A small set of reusable UI primitives (a `Panel`, a `Change` badge, an avatar)
   makes adding new pages fast and keeps the design consistent.
2. Route groups (`(dashboard)`) are a clean way to share a layout shell across many
   pages without repeating markup.
3. Class-based theming is what makes a dark-mode *toggle* work — media-query dark
   mode can't be toggled by the user.
4. Verifying the deployed URL (not just a green build) is what actually proves the
   "deployed with a live URL" requirement.

## Next Steps
- Swap the simulated feed for a real one (e.g. the CoinGecko API) — it only touches
  `src/lib/data.ts` and the tick logic in `live-markets.tsx`.
- Add a favicon and richer accessibility passes (focus states, reduced motion).

## Note on tooling
The Week 2 brief specifies **v0.dev** for generating the UI. In the interest of
honesty (a stated community value), this UI was **built directly** in
Next.js/Tailwind with AI-assisted coding (Claude Code) rather than generated with
v0.dev. It meets the functional objectives of the challenge — production-quality,
responsive, dark-mode, deployed — but did not use the v0.dev workflow specifically.
