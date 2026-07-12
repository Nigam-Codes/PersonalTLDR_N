# TLDR Intelligence

A personal, single-file news terminal — a Bloomberg-Terminal-meets-Linear dashboard for scanning, filtering, searching and saving the world's most important stories across AI, markets, science, geopolitics and innovation.

**No AI features.** No chat, no generative summaries, no ML recommendations. Just a beautifully organized personal intelligence dashboard built for fast reading and discovery.

## Features

- **Three-column layout** — fixed nav · center feed · insights rail · sticky search
- **Left sidebar** — Home, Today's Brief, Bookmarks, Saved Searches, 12 categories, and followable custom `#tags`
- **Hero** — time-aware greeting, story counts per desk, Read Brief / Listen (text-to-speech) / Watch Summary
- **News cards** — category badge, headline, TL;DR bullets, Why It Matters, impact meter, source badges, tags, bookmark/save/share
- **Right rail** — Trending Topics, Trending Companies, Breaking Timeline, Trending Tags, Global Focus map, Watchlist with live sparklines
- **Instant search** across headlines, companies, people, technologies, countries, tags, categories and topics — with recent + saved searches
- **Advanced filters** — region, source, importance, reading time
- **Reading view** — hero, TL;DR, key points, why it matters, timeline, related articles, original sources, reading time
- **Bookmarks** with folders (AI, Markets, Research, Must Read, Watch Later)
- **Personalization** — hide categories, dark/light theme, density, watchlist editor — all persisted to `localStorage`
- **Premium mobile app** — horizontal category tabs, bottom navigation, responsive cards

## Live data

The dashboard connects to free, keyless public sources directly from the browser — no backend, no API keys:

- **Live Wire** — real headlines from Google News RSS (via public CORS proxies) with Hacker News Algolia as fallback, filterable by desk, auto-refreshing every 90s
- **Live Quote Board** (Stock Market desk) — real prices and daily change for NVDA, AMD, TSLA, MSFT, AAPL, META, TSM, INTC, the SMH chip ETF and WTI crude, from the Yahoo Finance chart API, refreshed every 2 minutes
- **Candlestick charts** — 6 months of real OHLC + volume rendered on canvas with hover tooltips and 1M/3M/6M ranges
- **Flash Wire** — live headline stream on Oil & Energy, AI & Robotics, and Chip Money
- **Watchlist** — rail prices and sparklines hydrate from real quotes
- **Custom desks** — follow/unfollow any category, or add your own keyword desk that pulls a live feed (Categories → Edit)

Every live surface carries a **LIVE / DEMO DATA** pill: if a feed is unreachable (offline, proxy down, strict CSP), the app falls back to built-in demo data and says so.

## Design

Charcoal/graphite/navy dark theme (with a full light theme), glassmorphism cards, soft gradients, monospace for all terminal data (prices, times, counts), smooth micro-animations, keyboard shortcuts (`⌘K` search, `Esc` close).

## Running

It's a single self-contained `index.html` — zero dependencies, zero build. Open the file in any modern browser, or host it anywhere static.
