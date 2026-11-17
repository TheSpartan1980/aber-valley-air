# Aber Valley Air

Indicative PM2.5 and wood-smoke monitoring in Abertridwr, Caerphilly County Borough.

Two Pimoroni Enviro+ sensors — one in a rear garden, one at roof level — record PM1/PM2.5/PM10,
temperature, pressure and wind. The public site is built from a central SQLite database on the
author's home server and published here hourly:

<https://thespartan1980.github.io/aber-valley-air/>

## What this is, and is not

Low-cost optical sensors, not reference monitors. They cannot identify a source, cannot distinguish
wood smoke from other combustion, and are affected by humidity. An episode is only counted when both
units rise together. Nothing here is regulatory data.

The garden unit's humidity channel is faulty and excluded. Gas and noise channels are recorded
locally but not published.

## Licence

- Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- Code (collector, ETL, site generator): MIT, see `LICENSE`

## Layout

- `index.html`, `history.html`, `method.html`, `data.html` — generated
- `data/` — JSON and CSV exports
- Generated hourly; do not edit by hand.
