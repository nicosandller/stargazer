# Stargazer

An explorable, real-time **3D** model of the solar system in a single HTML page (Three.js loaded from CDN — no build step).

Everything is at **true scale**: real planet/moon sizes, real distances. Planets are placed using JPL's approximate Keplerian elements (valid 1800–2050 AD) in full 3D — including orbital inclination — computed for the visitor's current clock time. Moons use mean circular orbits in their planet's equatorial plane (visualization-grade).

Lighting is physical: a point light at the Sun gives every body its correct day/night terminator, and a focused shadow camera renders true cast shadows in whichever planet system you visit — Saturn's shadow on its rings, moon eclipse shadows on Jupiter.

Beyond the planets and their moons it includes Ceres, Pluto, Eris, and Halley's Comet (all on real Keplerian orbits), plus the asteroid belt, the Kuiper belt, and the inner Oort cloud as particle fields. Earth gets a procedurally generated surface — continents, polar ice, and a slowly drifting cloud layer.

## Controls

A sidebar lists every major body and region — click to fly there.

- **Drag** to orbit the view, **scroll / pinch** to zoom, **right-drag** to pan
- **Click** a body (or its name) to fly there and see details
- Time-warp buttons speed up, reverse, or pause time; **Now** snaps back to the present
- `size` buttons can exaggerate body sizes ×10 / ×100 for easier sightseeing (distances stay real)

## Run locally

Serve it (ES modules need http):

```sh
python3 -m http.server 4173
```
