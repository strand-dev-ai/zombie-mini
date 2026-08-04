# Zombie Mini — spec (2026-07-06)

Single-file 2.5D canvas arcade survival game. `index.html`, zero dependencies.

- **Goal:** impossible to win, fun to survive. Infinite waves, exponential difficulty vs linear upgrades. High score = best wave (localStorage).
- **Player:** walk only (WASD/arrows), machine gun auto-fires toward mouse. Cartoon guy: bob walk, squash on hit, muzzle flash, shell casings.
- **Camera/look:** slight-angle top-down, ellipse shadows, y-sorting, subtle depth scaling. Thick-outline cartoon style.
- **Zombies:** shambler, runner, tank, exploder; boss every 5th wave. Wobbly cartoon animation, blood particles, death pops.
- **Coins:** drop on kill, coin magnet auto-pulls (upgradeable radius).
- **Shop between waves (DOM overlay), 5 lines:** machine gun (rate/dmg/+bullets), turret (max 4, then upgrades all), explosions (auto-grenade), magnet radius, max HP. Costs scale ~1.6×/level. Everything resets on death.
- **In-game powerups (temporary drops only):** nuke, freeze, rapid fire, shield, coin rain.
- **Juice:** screenshake, particles, floating damage numbers, combo counter, WebAudio synth SFX (no files).
- **Out of scope:** mobile/touch, persistence beyond high score, multiplayer.

## v2 additions (2026-07-06)
- Auto-aim nearest zombie (no mouse), cursor hidden.
- Weapons: shotgun, bazooka (rockets explode), freeze gun (slows) — bought once in shop, Q cycles. Gun-upgrade line boosts all weapons.
- Perk cards: XP from kills, pick 1 of 3 on level-up (pierce, ricochet, vampire, fire trail, speed, crit, greed, tough).
- Map: 7 rocks (block movement + bullets), explodable barrels each wave (chain reactions, damage scales with wave).
- Elite zombies from wave 4: sprint / split-on-death / shielded, double coins, glowing ring.
- Clone shooters: shop item, max 4, ~doubles firepower per clone but zombie count ×1.3 per clone.
