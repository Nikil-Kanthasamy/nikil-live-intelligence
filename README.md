# Nikil Live Intelligence

A responsive, browser-based live information dashboard that brings together world-news headlines, developer-community stories, and noteworthy GitHub projects in one searchable interface. Built as a lightweight static web app with no server-side setup or API key requirement.

**Live demo:** https://nikil-live-intelligence.vercel.app  
**Repository:** https://github.com/Nikil-Kanthasamy/nikil-live-intelligence

## Overview

Nikil Live Intelligence is a multi-source briefing dashboard for quickly scanning developments across global news and the software ecosystem. Each source is presented in its own tab, with search and refresh controls to make browsing and revisiting stories straightforward.

## Data sources

| Section | Source | What it shows |
| --- | --- | --- |
| World Briefing | [GDELT DOC API](https://www.gdeltproject.org/) | English-language news article results, ordered by recency |
| Developer Radar | [Hacker News Algolia Search API](https://hn.algolia.com/api) | Stories and discussions from the Hacker News community |
| GitHub Pulse | [GitHub REST API](https://docs.github.com/en/rest) | Public developer-tool repositories, filtered by topic and popularity |

## Features

- Three dedicated feed tabs for news, developer discussions, and GitHub projects
- Search across displayed titles and sources
- Feed counts and last-updated information
- Manual refresh and automatic refresh every five minutes
- Responsive layout for desktop and mobile screens
- Direct links to original articles, discussions, and repositories
- Lightweight static deployment; no application server or API key required

## Technology

- HTML, CSS, and client-side JavaScript
- Public HTTP APIs fetched directly by the browser
- Static-site hosting (deployed on Vercel)

## Run locally

No build step or package installation is required.

1. Clone or download this repository.
2. Open a terminal in the repository folder.
3. Start a local static server:

```bash
python -m http.server 8000
```

4. Visit http://localhost:8000 in your browser.

You can also use another static file server of your choice.

## Deployment

This project is designed for static hosting.

- Import this GitHub repository into Vercel.
- Set the project root to the repository root.
- No build command is required.
- Deploy the static files.

Live URL: https://nikil-live-intelligence.vercel.app

## API, privacy, and limitations

- The app requests data from public APIs directly in the visitor's browser.
- No API key is required for the documented feeds.
- Availability, rate limits, response formats, and content are controlled by the third-party services.
- The dashboard links to source material; it does not republish articles or guarantee complete or instantaneous breaking-news coverage.
- Search applies to the content currently loaded into the dashboard.

## Project structure

The main application is organized around:

- `index.html` — dashboard markup and page structure
- `styles.css` — responsive visual styling
- `app.js` — feed requests, rendering, search, tabs, and refresh behavior

## Future improvements

Potential extensions include configurable topics, additional trusted data sources, saved searches, and richer filtering.

## Author

Created by **Nikil Kanthasamy** as a practical project exploring information aggregation, API integration, and responsive front-end development.
