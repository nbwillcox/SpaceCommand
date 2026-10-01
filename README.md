# SpaceCommand

A free, retro-flavored missile defense game with neon graphics and layered synthwave skylines, with a head nod to the classic arcade original. Aim with the mouse, launch interceptors, shield your cities, and spend credits on upgrades between waves.

**Play it in your browser:** https://nbwillcox.github.io/SpaceCommand/

Everything is generated in code: backdrops, buildings, weapons and effects are drawn on the fly, and all sound effects and music are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpaceCentiShooter](https://github.com/nbwillcox/SpaceCentiShooter), [SpaceVaderShooter](https://github.com/nbwillcox/SpaceVaderShooter) and [SpaceStroids](https://github.com/nbwillcox/SpaceStroids), with the same look and feel.

## Controls

| Action | Input |
| --- | --- |
| Aim | Mouse |
| Fire an interceptor (hold to repeat at your fire rate) | Left click |
| Pick a weapon | `1`-`4`, `Q` / `E` / `Tab`, or the mouse wheel |
| Fire the nuke (when charged) | `Space` or right click |
| Collect a pickup | Click it or let a blast touch it |
| Pause | `P` or `Esc` |

## Gameplay

- Defend **6 cities** and **3 launchers**. Click and the nearest launcher with ammo fires an interceptor that explodes where you aimed; the blast destroys anything it touches, and destroyed missiles explode too, so chain reactions score more. Each launcher holds a limited number of interceptors per wave.
- **Attackers:** ICBMs, **MIRVs** that split into several warheads, **smart bombs** that swerve around your blasts, **bombers** that drop missiles as they fly, and **laser UFOs** that lock on and burn a target unless you kill them first.
- **Damage persists.** A destroyed city or launcher stays down until you rebuild it in the shop (or earn a free **bonus city** every 10,000 points). Lose every city and it's game over.
- **Upgrade shop** between waves, paid with credits from kills and surviving cities:
  - Blast Radius, Missile Speed, Ammo Capacity, Fire Rate
  - **Cluster warheads** (burst into 3 / 5 / 7 blasts)
  - **Flak fields** (blasts that linger for seconds)
  - **Beam laser** (energy-powered sweeping beam, no ammo)
  - **Ultimate nuke** (charges as you score)
  - **Dome shields** that absorb hits, and **auto-turrets** that shoot on their own
- **Pickups** from carriers, UFOs and bombers: ammo refill, rapid fire, shields, instant nuke charge.
- Every 5th wave is the **Orbital Mothership**: knock out its shield generators, laser cannons and missile bays, then its core, while it rains missiles on your cities. Your launchers resupply during the fight.
- Five themed worlds with layered backdrops: Neon Sunset, Midnight Bay, Amber Dusk, Magenta Metropolis and Aurora Frost.
- Local top-10 high scores with arcade-style 3-letter initials (stored in your browser).

## Run locally

It is plain HTML/CSS/JS. Either open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

then visit http://localhost:8000. Desktop browsers with a mouse only for now.

## License and attribution

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix **non-commercially**, as long as you give credit and **link back to this repository**: https://github.com/nbwillcox/SpaceCommand

This is an original game inspired by classic arcade defense games. It uses no assets, names or code from any existing game.
