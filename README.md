# Emirates Route Profitability Explorer

An interactive data visualization dashboard exploring route-level profitability for Emirates Airlines. Analyzes 7,974 flight records across 30 destinations during 2024 to answer: *How do route distance, seasonal demand, and aircraft deployment interact to determine which Emirates routes from Dubai are profitable, and what does the underlying cost structure reveal about why?*

## Live Demo

[areebmohammed.github.io/emirates-dashboard](https://areebmohammed.github.io/emirates-dashboard)

## Key Findings

- Short-haul routes are systematically unprofitable (avg margin -26% vs. +23% for long-haul)
- Peak-season short-haul flights average -10% margin while off-peak shorts hit -46%
- Load factor is the strongest predictor of profitability
- The A380 averages +23% margin vs. -8% for the 737-800 due to revenue-per-hour differences

## Features

- **Bubble scatter plot** — each destination is a bubble (x = avg revenue/flight, y = selectable metric, area = flight count, color = route category) with geometric zoom and pan via D3
- **Brushable timeline** — monthly revenue and profit bars with D3 brush for date range filtering, cross-linked to all other views
- **Dynamic query filters** — toggle buttons for route category, travel season, and aircraft type implementing Shneiderman's dynamic queries paradigm
- **Details on demand** — tooltips on hover, persistent detail panel on click, and a cost breakdown donut chart
- **Top routes leaderboard** — ranked list of most profitable destinations with margin percentages

## Tech Stack

- Single-file HTML/CSS/JavaScript
- D3.js v7.9
- Hosted on GitHub Pages

## Data

Airline Route Profitability Dataset — 7,974 Emirates flights from Dubai to 30 destinations, 2024 (Kaggle)

## Running Locally

```bash
open index.html
```

---

Built for CSE 442: Data Visualization — University of Washington, 2024
