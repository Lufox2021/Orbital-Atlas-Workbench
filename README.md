# Orbital Atlas Workbench

A general chemistry learning tool for the quantum numbers **n** and **l**,
orbital names (1s … 4d), and **radial, angular and total nodes**, built on the
Orbital Atlas V3 3D viewer of exact hydrogen-atom wavefunctions.

## Modes

- **Learn** – 3D viewer for n = 1–4 (s, p, d), a rules card, and two tools:
  - **Nodes**: radial nodes drawn as gold spheres at their exact radii; angular
    nodes as violet planes (or the two cones of d_z²), with a readout of each
    node and a slider for the opacity of the angular-node sheets.
  - **Cut-away**: a textbook-style wedge cut (the upper-front quarter removed).
    The cut faces are pale and hatched, so each shell shows its thickness and
    the empty gaps between shells are the radial nodes.
- **Practice** – one question at a time with hints, immediate feedback and
  reasoning; after each answer the orbital appears with its nodes. Running
  tally by skill.
- **Test** – a self-check of 5–20 random questions with no hints or node
  display; score, per-skill breakdown and a review of every question.

## Question types

1. n, l → orbital name  2. Orbital name → n, l  3. Valid or invalid (n, l)
4. Allowed l for a given n  5. Nodes from the name  6. Nodes from n, l
7. Nodes → orbital name  8. Identify from the 3D picture
9. Identify from the radial distribution plot r²R(r)²

Scope: n = 1–4, s/p/d only; only n and l (no mₗ or mₛ). No data leaves the page.

## Running it

Open `index.html` in a browser, or the GitHub Pages URL once Pages is on
(Settings → Pages → Deploy from branch → `main` / `/ (root)`).

## Tech

Single self-contained HTML file; 3D via [Three.js](https://threejs.org/) r128
from cdnjs. Surfaces are built direction by direction from the exact radial
function, drawing every radial lobe; node radii are the exact zeros of R(r).
