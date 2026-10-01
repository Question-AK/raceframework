# Changelog

## 1.1.0-halfgiant.2 - local test build, 1 October 2026

- Removes the Half-Giant swim speed −75% and sinking penalties, which kept it from
  reaching the surface. Its height already makes surfacing about four times slower than
  a human's, and holding Space alone does not lift it out of deep water: swim up with
  Space plus forward, or by looking up and swimming forward.
- Everything else is unchanged from 1.1.0-halfgiant.1.

Local test only; not for the Khorvaire server or ModDB.

## 1.1.0-halfgiant.1 - local test build, 1 October 2026

- Adds the Half-Giant as a sixth playable model: the Racial Equality Human at 2.1× size,
  cloned by JSON patch so no Racial Equality files are copied.
- Half-Giant traits: +100% melee, +30 max health, stomach and hunger ×5.31, walk and
  sprint +25%, +7 °C warmth; frost, heat, starvation, drowning and fire damage ×3, fall
  damage ×6.3, +50% animal detection, swim speed −75%, sinks.
- Model step height 2.1. RF Mechanics 1.1.2 overrides step height for races it does not
  recognise, so expect 1.0 until RF Mechanics knows the Half-Giant.
- Built on 1.0.0; the unshipped dwarf-subrace removal (D18) is not included.

Local test only; not for the Khorvaire server or ModDB.

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
