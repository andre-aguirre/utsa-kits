# UTSA Bleeding Control Kits

A fast, mobile-friendly finder for the bleeding control kits mounted across UTSA's campuses. Tap once to see the closest kits, with walking directions.

**Status: unofficial prototype.** Not yet affiliated with or approved by UTSA. Locations are approximate and photos are pending. Do not rely on it in an emergency. In an emergency: Please Call 911.

## What it does

- **Find nearest kit.** Uses your current location to show the 3 closest kits with distance and walking time.
- **Pick a building.** Works without location or when your location is unavailable. Choose where you are and get the closest kits.
- **Open or closed.** Kits in buildings known to be locked at certain hours are skipped, and the page says so.
- **Direct links.** Every kit has its own link (for example `#kit-10`) that opens straight to it. ***(Useful for physical QR Codes near kits)***
- **Full directory.** Every kit, by campus, with search.
- Works on any phone or computer. No app, no login, individually optimized for both.

## Data

Kit locations come from UTSA PD's AED and Stop the Bleed locations list. Every kit is mounted with an AED.

Coordinates are currently placeholders until each kit is surveyed on site once the project receives the green light. Similarly, building hours are only shown when they are confirmed, and each entry has a date range. Once it expires, the page shows "Hours not confirmed".

## How it's built

One self-contained file, `index.html`. No server code, no database, no build step, and no outside libraries or fonts. It can be easily hosted on any web server.

To quickly update the webpage kits, edit these blocks near the top of the script in `index.html`:

| Block | What it holds |
|---|---|
| `RAW` | Campus, building code, room, kit count |
| `NAMES` | Full building names |
| `C` | Latitude and longitude per building |
| `HOURS` | Confirmed hours with valid dates |
| `FLAGS` | Notes shown on a kit |

## Hosting The Prototype

Served with GitHub Pages from the `main` branch. A `noindex` tag keeps it out of search engines while it's a prototype.

## Contact

Andre Aguirre, Founder, Project BloodLine

projectbloodlinesatx@gmail.com
andre.aguirre@my.utsa.edu
aguirrea4@uthscsa.edu
andreaguirre20@outlook.com (personal)
