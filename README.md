# UTSA Bleeding Control Kits

A fast, mobile-friendly finder for the bleeding control kits mounted across UTSA's campuses. Tap once to see the closest kits, with walking directions.

**Status: unofficial prototype.** Not yet affiliated with or approved by UTSA. Locations are approximate and photos are pending. Do not rely on it in an emergency. In an emergency, call 911.

## What it does

- **Find nearest kit.** Uses your current location to show the 3 closest kits with distance and walking time.
- **Pick a building.** Works without location, or when your location is unavailable. Choose where you are and get the closest kits.
- **Open or closed.** Kits in buildings known to be locked at that hour are skipped, and the page says so.
- **Kit details.** Tap any kit for photos of where it's mounted, floor, entrance, directions and hours.
- **Direct links.** Every kit has its own link (for example `#kit-10`) that opens straight to it. Useful for physical QR codes near kits.
- **Full directory.** Every kit, by campus, with search.
- Works on any phone or computer, with a layout built for each. No app, no login.

## Data

Kit locations come from UTSA PD's AED and Stop the Bleed locations list. Every kit is mounted with an AED.

Coordinates are placeholders until each kit is surveyed on site, once the project gets the green light. Building hours are only shown when confirmed, and each entry has a date range. Once it expires, the page shows "Hours not confirmed" instead of guessing.

## How it's built

One self-contained file, `index.html`. No server code, no database, no build step, and no outside libraries or fonts. It can be hosted on any web server.

To update kits, edit these blocks near the top of the script in `index.html`:

| Block | What it holds |
|---|---|
| `RAW` | Campus, building code, room, kit count |
| `NAMES` | Full building names |
| `C` | Latitude and longitude per building |
| `HOURS` | Confirmed hours with valid dates |
| `FLAGS` | Notes shown on a kit |

## Hosting the prototype

Served with GitHub Pages from the `main` branch. A `noindex` tag keeps it out of search engines while it's a prototype.

## Contact

Andre Aguirre, Founder, Project BloodLine

- projectbloodlinesatx@gmail.com
- andre.aguirre@my.utsa.edu
