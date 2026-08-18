# QWEN 3.8 MARIO

A fully playable, Mario-style browser platformer. Single-file HTML/CSS/JS — zero
dependencies, works offline.

## Play

Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).

## Controls

| Key            | Action                      |
|----------------|-----------------------------|
| Arrows / A D   | Run                         |
| Space / Up / W | Jump (hold = higher)        |
| P              | Pause / resume              |
| M              | Mute / unmute               |
| R              | Restart level               |
| Enter          | Start game / restart after finish |

Touch controls appear automatically on mobile.

## Features

- Intro menu over a live animated game scene
- One handcrafted level: pipes, ?-blocks, breakable bricks, spike pits,
  stone staircases, flag pole, and the end castle
- Goombas and fast Zz-t enemies with enemy-on-enemy bounce AI
- Stomping with chain multipliers, coin pops from ?-blocks, 1-UP at 10,000
- Coyote time, jump buffering, variable jump height
- Flag slide → auto-walk → COURSE CLEAR → fireworks → stats
- 3 lives, 300s timer, best score persistence (localStorage)
- Procedural chiptune (WebAudio) + SFX, no audio assets
- Parallax background, particles, screen shake

No build step, no framework — one `index.html`.
