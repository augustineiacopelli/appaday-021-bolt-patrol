# 021 · Bolt Patrol

A Sonic-inspired side-scrolling runner built for one player (hi, Simon). Roll through 8 zones, stomp enemies, collect rings, and survive long enough to destroy the Death Egg.

## How to Play

- **Tap / Click / Space** — Jump. Bolt curls into a spin ball the moment he leaves the ground.
- **Tap again in the air** — Double jump for extra height and distance.
- **Land on top of an enemy** — Stomp kill. Bounce off and keep going.
- **Hit an enemy from the side or below** — Lose a life.
- **Fall into a pit** — Lose a life. Watch the edges of platforms.
- **Collect rings** — 50 rings earns an extra life.

## Zones

8 unique zones with escalating speed and difficulty:

1. Green Hill Zone
2. Marble Zone
3. Spring Yard Zone
4. Labyrinth Zone
5. Starlight Zone
6. Scrap Brain Zone
7. Final Zone
8. Death Egg Zone

Clear all 8 to beat the game.

## Technical Notes

- Vanilla HTML/CSS/JS — no frameworks, no dependencies.
- Single `index.html`.
- Platform landing uses a two-pass per-frame support check to correctly handle walk-off edges.
- Pit fall-through is physics-based: ground support is removed when the player's center crosses a gap, gravity takes over naturally.
- Stomp detection uses overlap-entry direction (vy > 0 + small top-entry threshold) rather than simple bounding box comparison.

## Definition of Complete

- [x] Character runs, jumps, double-jumps, and curls into spin ball
- [x] Stomp enemies from above; take damage from sides/below
- [x] Pits with varied widths; character falls through rather than bumping
- [x] Floating platforms with correct walk-off physics
- [x] Ring collection with 50-ring extra life threshold
- [x] 8 unique zones with distinct color palettes and escalating difficulty
- [x] Win screen after clearing all 8 zones
- [x] Mobile-friendly single-tap controls
- [x] Lives system with game over and high score tracking
