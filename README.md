# SpaceX IPO Simulation (SPCX)

Local day-1 trading sandbox. **No install, no server, no API.**

## Live demo

**[Open simulator →](https://npgreatest.github.io/SpaceXIPOSimulation/)**

Enable once: Repo → **Settings → Pages** → Branch **master**, folder **/ (root)** → Save.

## Open locally

```bash
git clone git@github.com:NPgreatest/SpaceXIPOSimulation.git
cd SpaceXIPOSimulation
open index.html
```

Or double-click `index.html`.

## Features

- Fixed: **SPCX**, IPO cost **$135**
- 4 scenarios: stop loss · TP1 · TP2 · moon trailing
- Sliders: fill E, stop, moon high H, optimism (expected P/L)
- EN / 中文 toggle (top right)
- P/L is **cumulative** within a path; scenarios are **mutually exclusive**

## Calculation

| Scenario | Path |
|----------|------|
| Stop loss | E → stop |
| TP1 | TP1 sell → remainder @ E |
| TP2 | TP1 + TP2 → remainder @ E |
| Moon | TP1 + TP2 → trailing exit |

## Disclaimer

Sandbox only. Not investment advice. No auto-trading.
