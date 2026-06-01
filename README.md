# Exoplanet Atlas

[exoplanetatlas.com](https://exoplanetatlas.com) — full-stack exploration of 6,000+ NASA-confirmed exoplanets.

Solo-built. The code is private; this repo is an overview of the technical work.

## What it does

Exoplanet Atlas lets users explore every NASA-confirmed exoplanet in a 3D visualization, search by stellar properties or discovery method, compare planets side-by-side, and learn about exoplanet science through gamified discovery flows.

<!-- Add 3–4 screenshots from the live site here:
![3D view](./screenshots/3d.png)
![Planet detail](./screenshots/detail.png)
![Comparison](./screenshots/comparison.png)
-->

## Tech stack

- Next.js, TypeScript
- PostgreSQL with Prisma ORM
- Three.js for 3D visualization of stellar systems
- NASA Exoplanet Archive data integration

## Features

- 3D visualization of 6,000+ confirmed exoplanets in their stellar systems
- Search and filter by stellar properties, distance, discovery method, planet type, and habitability indicators
- Side-by-side planet comparison
- Gamified discovery flows that walk users through exoplanet detection methods (transit, radial velocity, direct imaging)
- Mobile-responsive

## Data pipeline

Pulls from the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/) on a scheduled refresh. Records are normalized and joined against host-star catalogs in Postgres before being served to the Three.js renderer client-side.

## Status

Live at [exoplanetatlas.com](https://exoplanetatlas.com).
