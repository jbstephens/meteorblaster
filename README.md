# Meteor Blaster

A single-file HTML space shooter for the family arcade. Fly the family ship, blast the falling meteors, and face **ZORG** at the end of the run.

Open `meteorblaster.html` in any modern browser (desktop, iPad Safari, etc.). No build step, no dependencies. Everything (graphics, sounds, voices, app icon) is generated at runtime — same pattern as Phaser Wars and Ninth Inning.

## Pilots

Ben, Luke, Mom, Dad — pick one. Each has their own ship colour, weapon colour, and victory voice (synthesized via the browser's speech engine).

## Controls

**Desktop**

- `← → ↑ ↓` or `WASD` — fly
- `Space` — fire (hold or mash; cooldown limits the rate)
- `B` — drop a bomb (clears the screen, chips Zorg)
- `P` or `Esc` — pause

**iPad / touch**

- 4-way D-pad (bottom-left) — fly
- **FIRE** button (bottom-right) — main weapon; mash it
- **BOMB** button (sits next to FIRE) — drop a bomb
- Drag anywhere on the canvas as an alternative to the D-pad
- Pause button (top-right) — same as Phaser Wars

## Run of play

Five waves, increasing difficulty: rocks, then ice rocks, then UFOs, then the **ZORG** boss with a figure-8 hover pattern, aimed bursts, and a meteor drop. Survive to win.

## Power-ups

Drop from destroyed meteors and UFOs (big rocks drop more often).

- **R** Rapid fire (10s)
- **S** Spread shot (10s)
- **◊** Shield (10s, absorbs hits)
- **B** Extra bomb
- **♥** Extra life (rare)

## Extras

- Three lives, two bombs to start
- Persistent high score saved per pilot (localStorage)
- Parallax starfield + drifting planets
- Synth sound effects + Zorg defeat speech — all generated, no audio files

## License

MIT
