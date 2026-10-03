# Changelog

## 1.1.0 - 4 October 2026

- Adds the Half-Giant, a sixth playable race: the Racial Equality Human at 2.1× size, cloned by JSON patch so no
  Racial Equality files are copied.
- Half-Giant traits: +100% melee damage, +30 max health, +25% walk and sprint speed, +7 °C warmth and +50% animal
  detection. Frost, heat, starvation, drowning and fire damage ×3; fall damage ×6.3. Model step height 2.1.
- Half-Giant hunger rate ×5.31 and stomach +630%: it eats like five Humans, and a full meal lasts about 1.4× a
  Human's.
- Orc: +40% hunger rate, stomach unchanged (+150%). A full stomach lasts about 1.8× a Human's, down from 2.5×.
- Elf: −47.5% hunger rate, stomach unchanged (−30%). A full stomach lasts about 1.33× a Human's, up from 0.7×.
- Removes the dwarf subraces; no race has subraces. Dwarves choose the six vanilla classes: commoner, hunter,
  malefactor, clockmaker, blackguard and tailor.

Known limitations:

- Existing worlds with Mountain or Hill Dwarf characters need RF Mechanics 1.2.0, which resets the retired class to
  `commoner` at login. Without it, Player Model Library's trait application raises an `ArgumentException` for the
  missing class when those characters load.
- The Half-Giant's stepping, wading and camera need RF Mechanics 1.2.0. RF Mechanics 1.1.2 does not recognise the
  Half-Giant and overrides its step height to 1.0.
- After a race change, the new stomach size applies once the world is reloaded.
- Racial diets in Diet Setup stay opt-in and need explicit bindings.

For Vintage Story 1.22.6. Half-Giant multiplayer testing remains limited.

## 1.0.0 - initial baseline, 7 September 2026

- Race traits and class choices for humans, dwarves, elves, orcs and goblins.
- Uses separately installed Player Model Library 1.23.8 and Racial Equality 0.1.28.
- RF Mechanics and Diet Setup remain optional; race diets require explicit bindings.
- Includes original-work MIT licensing, third-party notices and source/build identity.

Prepared for client/server deployment before the first ModDB release. Live gameplay and existing-world installation/removal acceptance remain unverified.

## 0.0.2-rc.1 ? candidate, unpublished

- Snapshot of current development for gameplay acceptance; not an approved stable release.
- Include MIT licensing for original work, credits and applicable third-party notices in packages.
- Add safe build/package commands, full source identity and immutable Release ZIPs.
- Document AI-assisted development, existing-save limitations and the development/stable release workflow.
