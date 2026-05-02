# Design Reference — shipflow-intro

## Identity

| Token          | Value                        | Usage                              |
| -------------- | ---------------------------- | ---------------------------------- |
| `--bg`         | `#070d1a`                    | Deep navy black — all backgrounds  |
| `--ink`        | `#e8edf5`                    | Primary text, node labels          |
| `--accent`     | `#38bdf8`                    | Sky blue — lines, rings, data text |
| `--green`      | `#22c55e`                    | Best carrier, savings, optimal     |
| `--amber`      | `#f59e0b`                    | Reserved for warnings / alerts     |
| `--muted`      | `#4a6080`                    | Secondary text, axis labels        |
| `--card`       | `#0d1829`                    | Card / node backgrounds            |
| `--border`     | `#1a2d4a`                    | Card borders, dividers             |
| `--accent-dim` | `#0c2d42`                    | Subtle accent backgrounds          |
| `--font-display` | `"DM Sans", sans-serif`    | Headlines, carrier names — weight 900 / 300 |
| `--font-data`  | `"IBM Plex Mono", monospace` | Code, data, labels, counters       |

## Typography scale

| Role         | Family        | Weight | Size  |
| ------------ | ------------- | ------ | ----- |
| Hero         | DM Sans       | 900    | 104px |
| Title        | DM Sans       | 900    | 68px  |
| Logo         | DM Sans       | 900    | 118px |
| Body         | DM Sans       | 300    | 28px  |
| Data / label | IBM Plex Mono | 400    | 13–23px |
| Query text   | IBM Plex Mono | 400    | 23px  |

## Scene plan

| Scene | Time     | Content                              | Transition  |
| ----- | -------- | ------------------------------------ | ----------- |
| s1    | 0–2s     | Voice command + waveform             | Hard cut    |
| s2    | 2–4s     | Node graph filling in                | Hard cut    |
| s3    | 4–6.5s   | Carrier evaluation + score bars      | `cinematic-zoom` shader → s4 |
| s4    | 6.5–9s   | Recommendation + analytics chart     | Hard cut    |
| s5    | 9–10s    | ShipFlow logo close                  | —           |

## Mood

Operator-grade dark UI. Precise, technical, trustworthy. The accent blue feels like
a terminal or satellite dashboard — deliberate and data-driven, not playful.
Green only appears on the winning carrier and savings, making it feel earned.
