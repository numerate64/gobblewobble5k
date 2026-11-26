# Gobble Wobble 5K Results Explorer

Static GitHub Pages app for filtering and ranking the Gobble Wobble 5K results. Supports live results, name/bib/town/team search, gender and inclusive age-range filters, sorting, and filtered-set ranking.

## Data source and limitation

RaceRoster returns no `Access-Control-Allow-Origin` header for the GitHub Pages origin, so browsers cannot fetch it directly. This app therefore uses `data/results.json`, a checked-in snapshot retrieved November 26, 2026. Results are not live and must be refreshed in the repository when desired. The source endpoint is `https://results.raceroster.com/v2/api/result-events/126228/sub-events/386489/results?filter_search=&limit=1000`.

## Run locally

Open `index.html` directly or run `python3 -m http.server 8000` in this folder.
