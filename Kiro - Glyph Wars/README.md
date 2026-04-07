# Glyph Wars

An arcade browser game where you control an ancient glyph warrior in a cosmic arena. Absorb enemies that match your symbol — avoid the rest.

## Controls

| Input | Action |
|-------|--------|
| Mouse move | Move your glyph |
| Click | Dash toward cursor (brief invulnerability) |
| Space (hold) | Chrono Shift — slows all enemies to 35% speed |

## Gameplay

- Your glyph symbol changes every 5 kills — adapt your strategy on the fly
- Absorbing a matching enemy builds your combo multiplier (up to x20)
- Let the combo decay and it resets to x1
- Waves escalate: faster spawns, new enemy types, higher stakes
- Collect pickups to restore HP or recharge Chrono energy

## Features

- 8 glyph symbols with matching color palettes
- Mouse-following movement with smooth lerp
- Click-to-dash with cooldown and invulnerability frames
- Chrono Shift time-slow mechanic (drains/recharges energy bar)
- Combo system up to x20 multiplier
- Glyph rotation every 5 kills with "GLYPH SHIFT!" announcement
- Progressive wave system (spawn interval decreases each wave)
- Particle explosions on absorb, damage, and wave transitions
- Player trail rendering
- Screen shake on damage
- Starfield + grid background
- HUD: HP bar, Chrono bar, Score, High Score, Wave, Combo
- High scores persist via localStorage

## Enemy Types

| Type | Behavior | HP |
|------|----------|----|
| Normal | Straight path with wobble | 1 |
| Seeker | Homes toward player continuously (dashed border) | 1 |
| Splitter | Splits into 3 normals on death (thick border, larger) | 2 |

Seekers appear from wave 3. Splitters appear from wave 5.

## How to Run

Open `index.html` directly in any modern browser — no server or build step needed.

For live reload during development:
```
npx live-server --port=5500 --open=index.html
```
