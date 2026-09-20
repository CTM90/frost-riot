# FROST RIOT

Arcade snowboarding. Two verbs. Real hills optional. Something in the snow if you ask for it.

A playable browser / PWA in the spirit of early-2000s boarder games (SSX Tricky, Cool Boarders) — original characters, original mountain, original meter. Not an EA remake.

## Play

```bash
cd frost-riot
python3 -m http.server 8765
```

Open [http://localhost:8765](http://localhost:8765). Phone: Add to Home Screen.

## How to ride

Two verbs: **steer** and **hold**.

- Desktop: `A`/`D` carve. Hold `Space` to charge. Flick to spin.
- Phone: drag left to carve. Hold JUMP. Flick on the pad to spin.
- Lean picks the grab. Warm RIOT + tuck auto-boosts. Full meter auto-Breakers at the apex.
- Follow the magenta **Echo**. **Snap** spends RIOT to save an almost-slam.

## Modes

- **Drop In** — Razor Ridge showoff. Score attack.
- **Local Line** — real hill from OpenSkiMap / DEM / GPX.
- **Whiteout** — same two verbs, a thing in the snow closing, avalanche wall, trees that hit. ESCAPED or HUNTED.

## Language

Title chips. Detects the browser. Remembers `frost-riot-lang`.
Brand stays English: RIOT, BREAKER, SNAP, Echo, FLOW, Local Line, Whiteout.

## Riders

| Rider | Role | Breaker |
|---|---|---|
| Jett Harrow | Speed | Redline Helix |
| Nix Vale | Tricks | Glass Orchid |
| Kizzy Rowan | Edge | Switchblade Sermon |

## Stack

Vanilla HTML / CSS / JS + Three.js r128. No build step. PWA.

Clone needs `js/game.js` and `js/i18n.js` from this repo. If a clone 404s those, copy them from the playable artifacts folder.
