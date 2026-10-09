# Haze Watch

Single-page app showing Singapore's 24-hour PSI by region (NEA via data.gov.sg)
and current weather for ASEAN capitals (Open-Meteo). No build step, no API keys.

## Deploy to Vercel

**Dashboard:** vercel.com/new → import this folder (or a Git repo containing it).
Framework preset: "Other". Leave build command and output directory empty.

**CLI:**

    npm i -g vercel
    cd haze-watch
    vercel --prod

## Notes
- Data is fetched in the browser; refreshes every 5 minutes.
- If an API is unreachable, the page shows a banner and sample values.
- Haze data comes only from data.gov.sg; Open-Meteo is used for weather only.
