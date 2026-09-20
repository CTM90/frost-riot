# FROST RIOT

Arcade snowboarding. Two verbs. Real hills optional.

A playable browser / PWA in the spirit of early-2000s boarder games (SSX Tricky, Cool Boarders) — original characters, original mountain, original meter. Not an EA remake.

## Play

Needs a local server (service worker + fetch):

```bash
cd frost-riot
python3 -m http.server 8765
```

Open [http://localhost:8765](http://localhost:8765). On a phone: Add to Home Screen.

## How to ride

Two verbs: **steer** and **hold**.

- Desktop: `A`/`D` or arrows carve. Hold `Space` to charge. Flick while holding to spin.
- Phone: drag left to carve. Hold the JUMP pad. Flick on the pad to spin.
- Lean picks the grab. Warm RIOT + tuck auto-boosts. Full meter auto-Breakers at the apex.
- Follow the magenta **Echo** to keep FLOW alive.
- **Snap** spends RIOT to save an almost-slam.

That's the whole game.

## Local Line

Title screen → **Local Line**.

- Tap a packed hill (Wintergreen, Massanutten, Snowshoe, Canaan, Killington, Mammoth, Whistler)
- Search a place name (OpenSkiMap), or paste `lat, lon`
- Drop a GPX / GeoJSON / `.riot.json`

We sample a public DEM, trace high → low, exaggerate pitch so a real groomer rides like an arcade course, and plant kickers on slope breaks. Export saves a tiny `.riot.json`.

This is the elevation model LiDAR already became — not a raw LAS upload.

Terrain: public DEM (Open-Meteo / SRTM / NED-class). Search: [OpenSkiMap](https://openskimap.org) / OpenSkiData. Trails you drop are yours. OSM credit when a named run is used.

## The loop

1. Drop in on Razor Ridge or a Local Line.
2. Hold into the glowing lip.
3. Grab + spin. Stick the landing — or Snap.
4. Points fill **RIOT**. Four letters = RIOT MODE.
5. Stay on the Echo or FLOW dies.

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

- Razor Ridge showoff + Local Line importer
- 3 riders
- Echo Line, Snap, lip magnet, auto-style
- Keyboard + touch
- `.riot.json` export / import

## What's not

- AI racers / World Circuit
- Voice lines or licensed soundtrack
- Open-world roam of a whole resort
- Raw LiDAR point clouds
- Photoreal snow
