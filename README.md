# Slider Crank Lab

An interactive slider-crank mechanism simulator for teaching piston displacement, velocity, and acceleration kinematics. Built as a single self-contained HTML file — no build step, no dependencies beyond a Google Fonts CDN link (falls back to system fonts if that's unavailable).

**[Live demo](#)** — replace with your GitHub Pages URL once enabled (see below).

## What it does

- **Mechanism view** — drag the blue crank pin to set the crank angle θ, or press **Run** to spin the mechanism continuously at a chosen speed. Piston displacement x is measured from the outer dead centre (ODC), matching the lecture convention.
- **Velocity diagram (o–a–b)** — the classic vector-diagram method: `oa` is the crank-pin velocity, `ab` is the piston's velocity relative to the pin (⊥ connecting rod), and their closure `ob` gives the piston velocity.
- **x, v, a over one revolution** — live plots of exact displacement, velocity, and acceleration across a full crank revolution, with the textbook binomial approximation overlaid as dashed curves for comparison.
- **Readout panel** — exact and approximate values at the current angle, the R/L ratio (flags when the small-angle approximation is no longer valid), the governing equations, and the extremes (max |v|, max |a|) over one revolution.

## Controls

| Control | Description |
|---|---|
| Crank **R** | Crank radius, in metres |
| Rod **L** | Connecting rod length, in metres |
| Speed **n** | Rotational speed, in rev/s |
| **θ** | Crank angle from ODC, in degrees (also settable by dragging the pin) |
| Run / Pause | Animate the mechanism at the chosen speed |
| Reset demo | Restores the defaults (R = 0.2 m, L = 0.5 m, n = 50 rev/s, θ = 60°) |

## Running locally

Just open `slider-crank-lab.html` in a browser — it's fully self-contained.

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. In **Settings → Pages**, set the source to the `main` branch, root folder.
3. Either rename `slider-crank-lab.html` to `index.html` (serves at the repo's root Pages URL), or leave the filename as-is and it'll be served at `https://<user>.github.io/<repo>/slider-crank-lab.html`.

## Credits

Designed with Claude Design and implemented as a standalone page by Claude Code.
