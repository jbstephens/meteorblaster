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

Seven waves, each one introducing something new:

1. **METEOR FIELD** — basic rocks
2. **ICE STORM** — ice meteors join in (lighter, glint)
3. **ENEMY CONTACT** — UFOs + first kamikaze swarm
4. **MOTHERSHIP** — red-domed mini-boss that drops kamikaze pods
5. **GUN BELT** — turret asteroids dock in and shoot at you
6. **CHAOS** — everything mixed, faster, with random meteor showers
7. **ZORG** — the green-domed boss with a figure-8 hover and meteor drops

Survive all seven to win. Take zero damage during a regular wave and you'll bank a +500 **PERFECT!** bonus when the next one starts.

## Enemies

- **Rocks** — fall, 1 hit (big rocks: 3 hits)
- **Ice rocks** — same but blue, glinty
- **Splitter rocks** — green, crack into 3 fast fragments when destroyed (great combo feeders)
- **UFOs** — drift across, fire aimed bolts
- **Kamikaze drones** — purple, dive in pods aimed at you
- **Turret asteroids** — dock at altitude, fire orange bolts, take 4 hits
- **Mothership** — wave-4 mini-boss
- **Zorg** — wave-7 boss

## Power-ups (ten kinds!)

Drop from destroyed meteors, UFOs, kamikazes, and turrets.

- **R** Rapid fire (10s)
- **S** Spread shot (10s, 5-way)
- **◊** Shield (10s, absorbs hits)
- **H** Homing shots (10s, bullets curve into the nearest enemy)
- **L** Laser (6s, continuous vertical beam)
- **W** Wingmen (12s, two escort ships auto-fire alongside you)
- **M** Magnet (15s, all power-up crates fly into you)
- **T** Slow-mo (6s, everything except you slows to a crawl)
- **B** Extra bomb
- **♥** Extra life (rare)

## Combos

Kills made within ~2 seconds of each other stack a combo. Every 3 hits raises the multiplier (1x → 2x → 3x → … up to 8x), the score popups change colour, and the announcer calls out milestones — **DOUBLE!**, **TRIPLE!**, **RAMPAGE!**, **INSANE!**, **GODLIKE!**. Taking a hit resets the combo.

## Extras

- Three lives, two bombs to start
- Persistent high score saved per pilot (localStorage)
- Parallax starfield + drifting planets + background streaking comets
- Random **METEOR SHOWER** set pieces
- Hit-pause on big kills (Zorg, mini-boss, turret)
- Synth sound effects + Zorg defeat speech + combo announcer — all generated, no audio files

## License

MIT
