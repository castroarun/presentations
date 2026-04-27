# Trading Automation v2 — Field Notes (concept)

**Status:** Working draft · v0.1
**Inspired by:** [ciechanow.ski](https://ciechanow.ski) — the standard for "the diagram IS the explanation"
**Aesthetic:** Editorial paper / Td journal (matches the dashboard home)

## What this is

A reimagining of the Trading Automation deck not as slides but as a **scrollable
field-notes article with live, scrubbable diagrams**. The reader doesn't watch
the algorithm — they drive it.

## What's built (v0.1)

A single working interactive that proves the concept:

- **Synthetic intraday price path** for a NIFTY-ish day (375 minutes, 09:15 to 15:30)
- **Scrubbable timeline** — drag the slider, click the chart, or hit play
- **Live OR detection** — the orange box draws itself as the first 15 minutes complete
- **Real signal logic** — when the price closes outside OR, a marker fires (LONG/SHORT)
- **Stop-loss visualization** — dashed red line where the algo would exit
- **Two knobs** — change the OR window (5–60 min) or the SL distance and watch every readout recompute
- **Live readouts** — OR high, OR low, signal status, position P&L

All in a single self-contained HTML file. No build, no framework, ~500 lines.

## What's planned (sketched in the "Coming next" section)

1. Position sizing demo — drag risk-per-trade, watch a year of P&L deform
2. KC6 Keltner channels drawn live, candle by candle
3. Trailing stops visualized as a moving floor
4. One-year equity curve, hover any day to see that morning
5. MQ paper-trading sandbox

## Decisions to make before promoting from draft → delivered

- [ ] Real backtest data instead of synthetic random walk (the demo is honest about this — but real data hits harder)
- [ ] Dark-mode variant? Or commit fully to the editorial paper aesthetic?
- [ ] Should each "interactive" be its own page (scrollytelling) or sections within one long page?
- [ ] Add a "view as slide deck" mode that wraps each interactive in a reveal.js section, so it can also be presented live?

## Source / inspiration trail

- ciechanow.ski — every article on that site
- Bret Victor's *"Tangle"* and *"Up and Down the Ladder of Abstraction"*
- The Pudding's interactive essays
- Stripe Press for typography rhythm
