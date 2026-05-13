# data-storytelling

Data journalism and visual storytelling projects by Josep Ferrer · DataBites

Each story follows the same pipeline: raw data from public sources, Python analysis, Datawrapper visualisations, published piece.

## Stories

| # | Title | Topic | Data source | Published |
|---|-------|--------|-------------|-----------|
| 01 | [Europe's renewable energy divide is getting wider, not narrower](https://reads.databites.tech/p/europes-renewable-energy-divide-is) | EU renewable energy 2004-2024 | Eurostat `nrg_ind_ren` | May 2026 |
| 02 | [Europe's tourist nights hit a record in 2024](https://reads.databites.tech/p/europes-tourist-nights-hit-a-record) | EU tourism nights distribution 2019-2024 | EU Tourism Dashboard `TOUR_NIGHT_SPENT` | May 2026 |

## Stack

Python · pandas · requests · Eurostat API · EU Tourism Dashboard API · Datawrapper · Substack

## Structure

Each story lives in its own folder under `stories/`:

```
stories/
  the_green_divide/
    data/              raw data files (cached API responses)
    outputs/           chart-ready CSVs for Datawrapper
    renewable_analysis.ipynb
  tourism_nights_distribution/
    data/              raw data files (cached API responses)
    outputs/           chart-ready CSVs for Datawrapper
    tourism_analysis.ipynb
```

Each notebook is self-contained: it fetches data from the source API, caches it locally, runs the analysis, and exports the chart-ready CSVs. No manual data download required.

## Links

- Website: [databites.tech](https://databites.tech)
- Newsletter: [reads.databites.tech](https://reads.databites.tech)
- X: [@iamjosepferrer](https://x.com/iamjosepferrer)
