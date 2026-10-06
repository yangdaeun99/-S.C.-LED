# Cube1 Simulation

A browser rig for the LED Cube 1 wall. Drop in one 2000 × 1440 delivery file and it
lands on the whole cube at once — no per-face assignment.

**Open it:** https://yangdaeun99.github.io/-S.C.-LED/cube1.html

## How the mapping works

1 px of the delivery file = 8 mm on the wall.

| | mm | px |
|---|---|---|
| one display | 2880 × 2880 | 360 × 360 |
| cross gap between displays | 260 | carries no pixels |
| one face | 6020 × 6020 | 752.5 |

Four displays make a face with a 260 mm cross between them. The cross is skipped,
not cut — a picture jumps the gap and lines up again on the far side, the way it
does on the real wall. 15 of the 24 displays are lit; the dark ones meet at the
back-left edge where the pillar stands.

## Controls

- **drag** — orbit · **wheel** — zoom
- **IMAGE / VIDEO** — load a file (or drop one anywhere on the page)
- **SETTINGS** — layer stack: opacity, blend, fit, scale, shift, speed, start time;
  reorder with ↑ ↓, hide with ●, remove with ×
- **RESET** — clears the layers of the canvas you are on
- **1 2 3 +** — separate canvases, so you can flip between versions and compare

With no layers loaded the cube shows the spec colours and panel codes from the net.

Everything runs locally in the browser. Nothing is uploaded.
