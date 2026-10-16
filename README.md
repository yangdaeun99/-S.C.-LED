# LED Cube Simulation

A browser rig for the three LED cubes. Drop in one delivery file per cube and it
lands on the whole box at once — no per-face assignment.

**Open it:** https://yangdaeun99.github.io/-S.C.-LED/cube1.html

## The three rigs

| | delivery file | box | faces |
|---|---|---|---|
| **Cube 1** | 2000 × 1440 | 6020 mm cube | 2880 mm displays, 260 mm cross, 15 of 24 lit |
| **Cube 2** | 1536 × 768 | cube | one 384 × 384 display per face, no seam |
| **Cube 3** | 672 × 480 | 288 × 288 × 192 | front and bottom full, side faces part lit |

Each net unrolls as `left | front | right | back` with the bottom flap under the
front, so reading the file left to right runs continuously around the box.

### Cube 1 mapping

1 px = 8 mm. Four 2880 mm displays make a face with a 260 mm cross between them.
The cross is skipped, not cut — a picture jumps the gap and lines up again on the
far side, the way it does on the real wall. The nine dark displays meet at the
back-left edge where the pillar stands.

## Controls

- **CUBE 1 / 2 / 3 / ALL** (top left) — each cube keeps its own canvases and layers;
  ALL shows the three together in the order they hang: 3 — 1 — 2
- **drag** — orbit · **wheel** — zoom
- **IMAGE / VIDEO** — load a file (or drop one anywhere on the page)
- **SETTINGS** — layer stack: opacity, blend, fit, scale, shift, speed, start time;
  reorder with ↑ ↓, hide with ●, remove with ×. `+ COLOR` adds a flat fill.
- **RESET** — clears the layers of the canvas you are on
- **1 2 3 +** — separate canvases, so you can flip between versions and compare

With no layers loaded a cube shows the spec colours and panel codes from its net.

### Transparency

Browsers cannot decode ProRes, so a QuickTime master will not load. Either export
**WebM / VP9 with alpha**, or — simpler — export on black and set the layer's blend
to **screen**, which drops the black exactly like an alpha channel.

Everything runs locally in the browser. Nothing is uploaded.
