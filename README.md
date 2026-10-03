# Race Framework

Release **1.1.0** for Vintage Story **1.22.6**. Adds the Half-Giant, retunes Orc and Elf hunger and removes the dwarf subraces; see CHANGELOG.md. Live multiplayer testing is still limited; expect bugs and balance changes.

**Summary:** Racial strengths, drawbacks and class choices for humans, dwarves, elves, orcs, goblins and half-giants.

### Development and AI use

**I've been a developer for about five years, and for the last two years I've worked closely with advanced AI models.** C# is a language I have much less experience with, so I use LLM coding tools to supplement my knowledge of the language and Vintage Story's modding API.

That includes generating and explaining code and data, researching implementation options, investigating errors and helping with documentation. AI has a substantial role in this project's development. I choose what goes into the mod, playtest as development progresses, and handle release decisions and maintenance. That does not mean every situation has been tested. The source is available for anyone who wants to inspect it, contribute or make their own version.

### What it does

Race Framework makes race a meaningful part of your character. Humans, dwarves, elves, orcs, goblins and half-giants have different strengths and limitations, affecting gathering, movement, combat and food capacity.

Your race and class remain separate choices, with available classes configured for each race. Character models and customization are supplied by **Racial Equality** and **Player Model Library**. Race Framework provides the traits and class setup around those projects.

### Companion mods

- **RF Mechanics** adds the active abilities and ongoing mechanics: elven climbing, dwarven Ore-Song, Orc Thew and scent, and goblin scavenging with spit.
- **Diet Setup** provides configurable food preferences and nutrition profiles, with optional bindings to these races.

Both companions are separate downloads. Install the parts you want to use.

### Installation

Install Racial Equality, Player Model Library and the dependencies required by their chosen versions, then add Race Framework. Multiplayer servers and clients should use matching mod versions.

If you also install Diet Setup, follow its instructions to enable the example race bindings. Installing both mods does not automatically activate race diets.

### Existing worlds — untested

I have not tested adding this mod to an existing world. No new-world requirement is currently known, but compatibility is not guaranteed.

**Installing on an existing save is at your own risk. I am not responsible for problems, lost progress or save damage resulting from doing so.** Make a full backup and test on a separate copy first. Keep the original backup: removing the mod does not necessarily undo saved changes.

Existing characters may need race/class reselection. Removing Race Framework can leave characters assigned to classes that are no longer available.

### No dwarf subraces

Race Framework 1.1.0 removes the dwarf subraces; no race has subraces. Dwarves now choose the six vanilla classes: commoner, hunter, malefactor, clockmaker, blackguard and tailor. Race Framework defines no dwarf subrace classes or marker traits.

Existing worlds with Mountain or Hill Dwarf characters need RF Mechanics 1.2.0, which resets the retired class to `commoner` at login. Without it, Player Model Library's trait application raises an `ArgumentException` for the missing class when those characters load.

### Planned races

I plan to keep developing the existing races and expand the roster with **Halflings, Gnomes, Giants, Frogs, Merpeople, Bugs, Dragon-kin and Cows**.

These are working names for future additions. They are not included in the current roster, and there is no fixed release order or timetable. Each should bring its own way of living in the world, with distinct capabilities, limitations and food preferences.

### Source, permissions and credits

Original work is MIT-licensed. You are welcome to fork it, tweak the balance and redistribute your changes without asking. Keep the included copyright and license notices. Third-party material remains under its applicable terms.

Thanks to **Tomoyuki** for Racial Equality and **Caliber** for work on Player Model Library. These projects supply the models and model system used here.

[Source code](https://github.com/Question-AK/raceframework) · [Report a problem](https://github.com/Question-AK/raceframework/issues)


## Build and contribute

Use `Build.ps1` to build/package locally without installing. See [RELEASING.md](RELEASING.md) for development branches, clean candidate builds, testing and the explicit publication gate. Original work is MIT; retain the [third-party notices](THIRD_PARTY_NOTICES.md).
