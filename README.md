# Gobble Wobble 5K Results Explorer

Static GitHub Pages app for filtering and ranking Gobble Wobble 5K results across the 2024, 2025, and 2026 editions. Supports runner search, gender and age-range filters, sorting, and filtered-set rankings.

## Data sources and limitations

The app uses checked-in snapshots from RaceRoster (2026) and Elitefeats (2024 and 2025). RaceRoster does not allow browser-origin requests, and the Elitefeats pages are also treated as snapshots so the static site has reliable data without a backend. Snapshots were retrieved November 26, 2026; they are not live and must be refreshed in the repository. The event selector links to each original results page.

- 2026 RaceRoster: `data/results.json` (821 results)
- 2025 Elitefeats race 24887: `data/elitefeats-24887.json` (749 results)
- 2024 Elitefeats race 23962: `data/elitefeats-23962.json` (683 results)

The Elitefeats exports include the published overall place, bib, age, gender, time, pace, and gender place. City/team information is not provided by those result listings. Age-band rankings are calculated from available ages and are not necessarily official award categories.

## Run locally

Open `index.html` directly or run `python3 -m http.server 8000` in this folder.
