# ChartLab — Learn to Read Charts

An interactive, self-paced chart-literacy course for adults. Candlestick basics → support/resistance → trends → market structure → ICC → candlestick & chart patterns → Fibonacci → order blocks & FVG → liquidity → multi-timeframe → risk management → building a trade plan.

**13 tracks · 47 steps**, with lessons, quizzes, and hands-on charting practice where you draw levels, trendlines, and zones directly on real candlestick charts and get graded feedback.

Everything is a single self-contained `index.html` — no build step, no dependencies, no backend. Progress is saved in the browser (localStorage).

> Educational platform only. Not financial advice.

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
3. You get a live URL instantly (e.g. `your-site.netlify.app`).
4. Create a free Netlify account to keep the site and rename it.

To update later: drag the folder again, or connect the GitHub repo (below) for auto-deploys.

### Option B — GitHub Pages (free, version-controlled)

```bash
# 1. Create a repo on GitHub (e.g. "chartlab"), then:
git remote add origin https://github.com/<your-username>/chartlab.git
git branch -M main
git push -u origin main

# 2. On GitHub: Settings → Pages → Source: "Deploy from a branch"
#    Branch: main / root → Save
```

Your site goes live at `https://<your-username>.github.io/chartlab/` within a minute.
The included `.nojekyll` file tells Pages to serve the HTML as-is.

---

## Editing content

All course content lives in the `TRACKS` array near the top of the `<script>` in `index.html`.
Each track has `lessons`, `quizzes`, and `practice` steps. Chart visuals are defined in the
`buildChart()` function. Add a track by appending an object to `TRACKS` and a matching
chart case in `buildChart()`.
