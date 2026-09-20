# FROST RIOT

Arcade snowboarding. Tricks fill the tank. The tank is the mountain.

A playable browser / PWA slice in the spirit of early-2000s boarder games (SSX Tricky, Cool Boarders) — original characters, original mountain, original meter. Not an EA remake.

## Play

Open `index.html` from a local server (the PWA service worker needs http):

```bash
cd frost-riot
python3 -m http.server 8765
```

Then go to [http://localhost:8765](http://localhost:8765).

On a phone: open that URL and **Add to Home Screen**. The app launches fullscreen.

Enable GitHub Pages on this repo (Settings → Pages → Deploy from main) to play at `https://ctm90.github.io/frost-riot/`.

## How to ride

**Desktop**
- `A` / `D` or arrows — carve
- Hold `S` — tuck and pre-wind
- `Space` — ollie (release at the lip for big air)
- In air: `W`/`S` flip, `A`/`D` spin
- `J` Mute · `K` Indy · `L` Melon · `I` Method
- `Shift` — boost (spends the RIOT meter)
- `F` — Breaker when the meter is full
- `P` / `Esc` — pause

**Phone**
- Left side drag — carve
- Hold JUMP to pre-wind, release to ollie
- BOOST spends the meter
- Grab pads appear in the air
- BREAKER when the bar is lit

Land clean. Repeat grabs pay less. Keep flowing or the multiplier dies.

## The loop

1. Carve Razor Ridge.
2. Pre-wind into kickers.
3. Grab + spin + flip. Stick the landing.
4. Points fill the **RIOT** meter.
5. Spend it on boost, or dump a **Breaker** (character signature).
6. Chain unique tricks to climb the FLOW multiplier (cap 8x).
7. Fill four letters — **RIOT MODE** — infinite boost.

Medals: FROST 40k · RIOT 120k · LEGEND 250k · UNHOLY 400k

## Riders

| Rider | Role | Breaker |
|---|---|---|
| Jett Harrow | Speed | Redline Helix |
| Nix Vale | Tricks | Glass Orchid |
| Kizzy Rowan | Edge | Switchblade Sermon |

## Stack

Vanilla HTML / CSS / JS + Three.js r128. No build step. Works as a PWA.

Later path if you want App Store / Play: wrap with Capacitor, or rebuild the same systems in Godot 4.

## What's in v0

- One mountain (Razor Ridge), showoff score attack
- 3 riders with different speed / trick / edge
- Kickers, two rails, air multiplier rings
- Combo, RIOT meter, Breakers, landing check
- Keyboard + touch

## What's not

- AI racers / World Circuit
- Voice lines or licensed soundtrack
- Open mountain (this is a spline course, on purpose)
- Photoreal snow
