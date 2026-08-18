# QWEN 3.8 MARIO

A fully playable, Mario-style browser platformer. Single-file HTML/CSS/JS —
zero dependencies, works offline.

## Play

**Live (any device, any network):**
https://saadharis.github.io/qwen38-mario/

Or open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).
No build step, no server needed.

## Controls

| Key            | Action                            |
|----------------|-----------------------------------|
| Arrows / A D   | Run                               |
| Space / Up / W | Jump (hold = higher, release = pop) |
| P / Esc        | Pause / resume                    |
| M              | Mute / unmute                     |
| R              | Restart level                     |
| Enter          | Start / replay after finish       |
| Click / tap    | Start; during play = jump (mobile) |

Touch controls appear automatically on mobile.

## Features

- Animated title menu, intro card, pause, game over, and COURSE CLEAR screens
- One hand-tuned 224-tile level: 8 pipes, ?-blocks, breakable bricks, a row-of-4
  coin arch, stone plateau with stair risers, death pits, spike strips,
  end staircase, flag pole, and the castle
- 22 Goombas + 3 fast Zz-t runters with enemy-on-enemy bounce AI
- Stomping with chain multipliers (100/200/400/800/1600), brick breaks,
  coin pops, 1-UP every 100 coins
- Coyote time, jump buffering, variable jump height, skid on turnarounds
- Flag slide → auto-walk out → fireworks → stats (score, coins, time, best)
- 3 lives, 300s timer, best score persisted in localStorage
- ICONIC Super Mario BROS. 1-1 overworld theme (WebAudio, synthesized — no
  audio files): the full A-A-B-B-C loop with lead, bass, and a drum groove
  that joins at bar 9, just like the original. The music is
  MOVEMENT-REACTIVE: sprinting speeds the tempo up and chirps the lead
  higher (a la 2-1), and the lead ducks while you're airborne so SFX speak.
  Title screen uses the same loop; a one-shot classic game-over song
  (E-C-G dropping to E) plays on losing. Plus 10 synthesized SFX.
- Parallax sky/hills, dust & sparkle particles, screen shake, camera lookahead

Verified by an automated 60-check browser test suite (headless Chrome):
full level completion, all hazard/enemy/coin interactions, state machine,
audio channels, persistence, and a 60-second soak with zero JS errors.

## Sharing with friends
- **Best:** send the live link — `https://saadharis.github.io/qwen38-mario/`.
  Permanent, works on phones, tablets, PCs, any network. Pushes to `main`
  auto-redeploy it (GitHub Pages, ~1 min).
- **Offline:** send `QWEN38-MARIO.html` (or the zip) in any chat/email/AirDrop.
  It's one 55 KB self-contained file — opens offline, no server, no internet needed.
  On iPhone: Files → tap → Share → "Open in Safari". iOS starts audio after the first tap.
- **Temp ports/tunnels** (ngrok, cloudflared, LAN IP) work too, but the Pages
  link above is the one that outlives your machine.
