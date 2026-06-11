# Stargazer

An explorable, real-time model of the solar system in a single HTML page — no build step, no dependencies.

Planets are placed using JPL's approximate Keplerian elements (valid 1800–2050 AD), computed for the visitor's current clock time. Major moons of each planet are shown with mean circular orbits (visualization-grade accuracy).

## Controls

- **Drag** to pan, **scroll / pinch** to zoom
- **Click** a body to follow it and see details
- Time-warp buttons speed up, reverse, or pause time; **Now** snaps back to the present
- Zoom into a planet to reveal its moons

## Run locally

Just open `index.html`, or serve it:

```sh
python3 -m http.server 4173
```
