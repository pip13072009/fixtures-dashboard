# Fixtures dashboard

Upcoming fixtures, UK kick-off times and confirmed UK TV channels for:

- Northampton Saints
- MK Lightning
- Colorado Avalanche
- Chelsea
- Arsenal Women

Open `index.html` through GitHub Pages (or any static web server). It reads:

- `data/fixtures.json`: one row per fixture (`team`, `kickoff_utc`, `time_tbc`, `opponent`, `home_away`, `competition`, `venue`, `tv`, plus source links)
- `data/results.json`: each team's latest result
- `data/meta.json`: when the data was last refreshed

Home games are shaded green. Avalanche games with a puck drop outside midnight–5am UK time get a coloured stripe.

The data is refreshed every Friday morning by a scheduled Claude task that re-checks fixtures, TV picks and results and commits the updated files here.
