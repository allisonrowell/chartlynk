# ChartLYNK — Read Market Structure

A structure-first, self-paced chart-education course for adults. From a single candle to advanced smart-money concepts and the psychology behind execution — with real charts you practice on, not just theory.

**14 tracks · 74 steps**, with lessons, quizzes, and hands-on charting practice where you draw levels, trendlines, and zones directly on real candlestick charts and get graded feedback.

Everything is a single self-contained `index.html` — no build step, no dependencies, no backend. Progress is saved in the browser (localStorage).

> Educational platform only. Not financial advice.

## Curriculum

1. Candlestick Basics
2. Support & Resistance
3. Trends & Direction
4. Market Structure: HH / HL / LH / LL
5. ICC — Indication · Correction · Continuation
6. Candlestick Patterns
7. Chart Patterns
8. Fibonacci
9. Order Blocks & FVG
10. Liquidity & Smart Money
11. Multi-Timeframe Analysis
12. Risk Management
13. The Trade Plan
14. Trading Psychology

---

## Run locally

Just open the file:

```bash
open index.html
```

Or serve it (any static server works):

```bash
npx serve -p 5500 .
# then visit http://localhost:5500
```

---

## Deploy

### Option A — Netlify Drop (fastest, no account needed to start)

1. Go to **https://app.netlify.com/drop**
2. Drag this entire `trading-school` folder onto the page.
3. You get a live URL instantly (e.g. `chartlynk.netlify.app`).
4. Create a free Netlify account to keep the site and rename it.

To update later: drag the folder again, or connect a GitHub repo for auto-deploys.

### Option B — GitHub Pages (free, version-controlled)

```bash
git remote add origin https://github.com/<your-username>/chartlynk.git
git push -u origin main
# On GitHub: Settings -> Pages -> Source: "Deploy from a branch" -> main / root -> Save
```

Live at `https://<your-username>.github.io/chartlynk/`. The `.nojekyll` file serves the HTML as-is.

---

## Editing content

All course content lives in the `TRACKS` array near the top of the `<script>` in `index.html`.
Each track has `lessons`, `quizzes`, and `practice` steps. Chart visuals are defined in the
`buildChart()` function. Add a track by appending an object to `TRACKS` and a matching
chart case in `buildChart()`.

---

ChartLYNK is an independent venture, separate from any other business or brand.
