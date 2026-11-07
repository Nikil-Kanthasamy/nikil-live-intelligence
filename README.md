# Nikil Live Intelligence

A responsive, browser-based dashboard for public world-news headlines, software-development stories, AI discussions and recently updated GitHub repositories.

**Live site:** https://nikil-live-intelligence.vercel.app

## Feeds
- **World briefing:** GDELT DOC API (English-language article results, newest first).
- **Developer radar:** Hacker News Algolia Search API.
- **GitHub pulse:** GitHub public repository search API, filtered for developer-tools topic and repositories with over 500 stars.

## Features
- Separate tabs for each feed
- Search across titles and sources
- Feed counts, update time and manual refresh
- Automatic refresh every five minutes
- Responsive layout for desktop and mobile
- Original source links open in a new tab

## Run locally
Serve this directory with any static web server, for example:
```bash
python -m http.server 8000
```
Then open http://localhost:8000.

## Notes
This project uses public APIs directly from the browser and requires no API key. Availability, rate limits and returned content are controlled by those services. Headlines link to the original publisher URL where provided. The dashboard is an aggregator, not a publisher or a guarantee of real-time breaking-news coverage.

## Deployment
Deploy the repository as a static site on Vercel. No build command is required; use the repository root as the output directory.
