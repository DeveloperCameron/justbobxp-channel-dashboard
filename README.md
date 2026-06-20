# 📊 JustBobXp Channel Performance Dashboard

An interactive Tableau dashboard analyzing six months of real YouTube channel data — tracking subscriber and view growth, identifying viral spikes, and breaking down which content categories drive the most engagement.

**[🔗 View the live dashboard on Tableau Public](https://public.tableau.com/app/profile/cam.bob/viz/JustBobXpChannelPerformanceDashboard/JustBobXpChannelPerformanceDashboard)**

## Overview

This project pulls daily channel statistics and video metadata directly from the [JustBobXp](https://www.youtube.com/@JustBobXp) YouTube channel via the VidIQ API, then visualizes growth patterns and content performance in Tableau Public.

## Key Insights

- **Viral growth event:** Total views jumped from ~96K to ~280K between March 5–31, 2026 — a roughly 190% increase in under a month, following a long flat period in January and February.
- **Two distinct spike windows:** A primary spike in early-to-mid March (peaking at ~38K views in a single day) and a smaller secondary spike in mid-May (~6–7K/day).
- **Content category dominance:** Of the channel's top-performing Shorts, content tagged under "Jujutsu Shenanigans (JJS)" outnumbers every other category combined, confirming it as the channel's strongest content pillar.
- **Data quality note:** A small negative dip in views around January 24 reflects a real YouTube view-count correction (likely invalid/bot view removal) rather than a data error — flagged and retained rather than smoothed over.

## Tools & Process

- **Data source:** VidIQ API (channel stats + video metadata)
- **Data processing:** Python (cleaning, categorization, CSV export)
- **Visualization:** Tableau Public

## Repo Contents

| File | Description |
|---|---|
| `justbobxp_channel_growth.csv` | Daily subscriber count, total views, total videos, and day-over-day deltas (Jan 1 – Jun 20, 2026) |
| `justbobxp_shorts_categorized.csv` | The channel's most popular Shorts, tagged by content category (JJS, AOT Revolution, Blox Fruits, Shindo Life, etc.) |

## Dashboard Components

1. **Channel Growth Timeline** — cumulative view growth over time
2. **Daily View Spikes** — daily view gains as a bar chart, isolating exact viral days
3. **Content Category Breakdown** — which content type drives the most top-performing videos
