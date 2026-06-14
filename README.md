# Rare Earths, Materials Data Series #4

An interactive data dashboard and LinkedIn carousel on the 17 elements behind every magnet, motor and screen: how little we mine, where they hide, what they do, and the most concentrated supply chain of any major material.

Part of my Materials Data Series, where I take one material at a time and tell it as a materials engineer who works in data. Steel, aluminium and copper came first. Lithium is next.

**Live dashboard:** _(deploy `index.html` to Netlify/GitHub Pages)_

---

## What's inside

| File | What it is |
|------|-----------|
| `index.html` | Interactive Chart.js dashboard, 5 tabs: The Elements, Where They Hide, What They Do, The Supply Chain, Why It Matters |
| `fetch_data.py` | Reproducible Python pipeline that compiles the cited figures into `data/*.csv` |
| `data/*.csv` | Tidy datasets (mine output, China's share along the chain, trend, metals comparison, demand by use and element, device content, reserves, scale) |
| `carousel/index.html` | 9-slide LinkedIn carousel (1080x1080) |
| `Rare_Earths_Materials_Carousel.pdf` | Exported carousel, ready to upload |
| `linkedin-post.txt` | Post caption |

## Reproduce the data

```bash
python fetch_data.py      # writes data/*.csv
```

The dashboard embeds the same numbers in JS so it runs from `file://` with no server. `fetch_data.py` documents where each figure came from and keeps it reproducible.

## What the data shows

- The world mines only **390,000 tonnes** of rare earths a year. It makes more steel than that every **two hours**.
- They are not actually rare. **Cerium is more common than copper.** The difficulty is separating them, not finding them.
- **China's grip tightens down the chain: 69% of mining, 91% of refining, 94% of finished magnets.** The chokepoint is processing, not the mine.
- They hide in tiny amounts everywhere: ~0.5 g in a smartphone, ~2 kg in an EV motor, ~1 t of magnets in an offshore wind turbine, ~418 kg in an F-35.
- Nearly **half of demand is permanent magnets**, and magnet-metal demand could rise 11 to 13x by 2050.

## Sources

USGS Mineral Commodity Summaries 2025 (mine production, reserves) · IEA Rare Earth Elements analysis (supply-chain shares, demand) · Adamas Intelligence (F-35 content) · JRC / Benchmark Minerals (device content).

Output in kt (thousand tonnes) of rare-earth oxide. Device and supply-chain figures are 2024 estimates, rounded and attributed.

---

*Built by Ibtisam Ahmed Khan · June 2026 · [linkedin.com/in/ibtisam-ahmed-khan](https://linkedin.com/in/ibtisam-ahmed-khan)*
