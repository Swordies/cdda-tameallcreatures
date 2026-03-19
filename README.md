# Tame All Creatures

**Author:** Swordie
**Version:** 1.2.0
**License:** MIT

A mod for Cataclysm: Dark Days Ahead and its forks that lets you tame and befriend every creature in the game; zombies, mi-go, robots, nether beings, all of them. It adds craftable taming treats, a corpse-to-treat conversion system, throwable pacification bombs with visible gas clouds, throwable healing incense for patching up tamed creatures, command items for rallying pets, craftable creature armor, mountable creatures, custom starting scenarios, a questgiving NPC, and 8 new taming-focused professions.

## Supported Builds

| Build | Folder | Monsters | Silent Moves | Starting Pet Scenarios |
|-------|--------|----------|--------------|----------------------|
| **DDA 0.H** | `TameAllCreatures_0H` | 974 | No (ear plugs only) | Scenarios included; no starting pets |
| **DDA 0.I** | `TameAllCreatures` | 1,121 | Yes | Yes; 7 scenarios with pre-tamed pets |
| **Bright Nights** | `TameAllCreatures_BN` | 1,121 | No (ear plugs only) | No scenario support |
| **The Last Glyph** | `TameAllCreatures_TLG` | 1,121 | Yes | Yes; 7 scenarios with pre-tamed pets |

Download the ZIP that matches your game fork. Each build is independently tested and accounts for engine differences in item format, monster roster, and feature support.

## Installation

1. Download the ZIP for your fork from the [Releases](../../releases) page.
2. Extract the folder into your game's `data/mods/` directory.
3. Start a new game (or load an existing one) and enable "Tame All Creatures" in the mod list.

## Features

### Taming Treats
Five types of craftable treats, each used on a single creature to tame it:

| Treat | Target Creatures | Crafting Skill |
|-------|-----------------|----------------|
| Meaty Taming Treat | Zombies, animals, dinosaurs | Cooking 3 |
| Herbal Taming Treat | Insects, fungi, plants | Cooking 3 |
| Electronic Taming Module | Robots, cyborgs, turrets | Electronics 4 |
| Eldritch Taming Offering | Nether creatures, mi-go | Cooking 5 |
| Universal Taming Treat | ALL creatures | Cooking 6 |

Activate the treat while standing next to a creature to try taming it.

### Taming Treat Toolkit & Corpse Conversion
A reusable crafting tool that converts butchered creature remains into taming treats. Kill a creature, butcher it for parts, then open the crafting menu (`&`) and search for the treat you want. The toolkit is never consumed.

| Input Material | Output | Notes |
|---------------|--------|-------|
| Fresh meat | Meaty Taming Treat (x3) | From animals, humans, dinosaurs |
| Fresh vegetables | Herbal Taming Treat (x3) | From insects, fungi, plants |
| Electronic parts | Electronic Taming Module (x3) | From robots and cyborgs |
| Tainted flesh | Eldritch Taming Offering (x3) | From nether creatures, mutants, zombies |
| Any 2 specialty treats | Universal Taming Treat (x2) | Combines any two treat types |

All corpse-to-treat recipes require only the butchered remains and the toolkit; no extra ingredients needed.

**Zombie balance:** Zombie corpses yield tainted meat when butchered. This can't be turned into meaty treats; only eldritch offerings. Zombies can't become a free, infinite source of easy treats.

### Pacification Bombs
Five types of throwable devices that release a sustained pacification cloud. Wield, activate (pulls the pin), then throw. Creatures caught in the cloud get Pacified; dazed, slowed, and with reduced stats for 5-10 minutes. Walk up and use a regular taming treat to finish the tame.

The cloud spreads over time and the bomb emits gas for about 3 hours. Warning: the pacification effect hits you and friendly NPCs too.

### Healing Incense
Five types of throwable items that release a sustained healing cloud. Works the same way as pacification bombs: wield, activate, throw. Any creature standing in the cloud heals 2-4 HP every 10 turns. Burns for about 3 hours.

### Command Items
Five themed command items that rally tamed creatures into a combat frenzy. Activate to trigger an adrenaline spike in all nearby tamed creatures; they deal more damage and move faster for about two minutes, followed by a brief crash with reduced stats.

### Creature Armor
Craftable armor for tamed creatures in two tiers (simple leather and reinforced steel+leather) across all 15 body types: canine, stout, arthropod, humanoid, serpentine, winged insect, amorphous, arachnid, equine, mi-go, crustacean, aquatic, ursine, avian, and macropod. Equip by interacting with a tamed creature.

### Mounting
All creature overrides include `PET_MOUNTABLE`. Any tamed creature that's at least one size category larger than you and can support your weight (20% ratio) can be ridden. All taming professions start with Survival 4, which lets you ride without a saddle.

### Starting Scenarios
Seven custom scenarios, each paired with one taming profession and pre-tamed starting pets:

| Scenario | Profession | Starting Pets |
|----------|-----------|---------------|
| Beast Tamer's Menagerie | Beast Tamer | Dog + tabby cat |
| Insect Handler's Nest | Insect Tamer | 2 small bees + small ant |
| Dinosaur Wrangler's Camp | Dino Wrangler | Raptor |
| Demonologist's Sanctum | Demonologist | Kreck |
| Machine Whisperer's Workshop | Machine Whisperer | Manhack |
| Mycologist's Grove | Mycologist | Young fungaloid + 2 spores |
| Zombie Whisperer's Refuge | Zombie Whisperer | Zombie |

**Build notes:** 0.I and TLG include pre-tamed starting pets. 0.H includes the scenarios but the engine doesn't support the `pets` field, so you'll need to tame creatures with your starting treats. BN doesn't support scenarios at all.

### Wandering Tamer NPC
A unique NPC with two sequential quests:

1. **A Tamer's Errand:** Bring 5 cooked meat. Reward: a taming treat toolkit + the crafting recipe.
2. **The Universal Formula:** Bring 3 meaty taming treats. Reward: the universal taming treat recipe (the only way to learn it outside of taming professions).

### Professions
Eight new professions, each starting with themed taming treats, a command item, a pacification bomb, healing incense, a toolkit, medical supplies, rope, and ear plugs:

| Profession | Specialty | Starting Treat Type |
|-----------|-----------|---------------------|
| Beast Tamer | Carnivores, animals | Meat |
| Insect Tamer | Arthropods, insects | Veggie |
| Dino Wrangler | Dinosaurs, large beasts | Meat |
| Demonologist | Nether, eldritch | Eldritch |
| Machine Whisperer | Robots, cyborgs | Tech |
| Mycologist | Fungi, plants | Veggie |
| Zombie Whisperer | Undead | Meat |
| Universal Tamer | All creatures | Universal |

Each profession has a unique trait with a passive morale bonus (+10) that refreshes via the EOC system.

### Other Features
- **Flesh Rope:** A craftable binding made from sinew, leather, fur, and tanned hide via the toolkit.
- **Silent Tamed Creatures (0.I/TLG only):** All creature overrides include `SILENTMOVES`, eliminating footstep noise from tamed creatures. The 0.H and BN builds rely on ear plugs for noise management instead.
- **Profession Morale Bonus:** Each taming profession trait grants a passive +10 morale bonus.
- **Vanilla Faction Preservation:** Untamed creatures still fight, flee, or coexist with each other as normal.

## Known Limitations

- **Taming is single-target.** Treats must be used one creature at a time. Pacification bombs are the crowd-control workaround.
- **Tamed zombies attack friendly NPCs.** This is a hardcoded engine limitation ([GitHub #78467](https://github.com/CleverRaven/Cataclysm-DDA/issues/78467)). Only the ~86 monsters with the ZOMBIE species are affected; the other 1,000+ creatures behave correctly.
- **Healing is area-based.** The healing cloud affects everything in the area, including wild creatures and you.
- **Pacification hits everyone.** The cloud doesn't pick sides. You, your NPCs, and your tamed creatures all get affected.
- **Clouds fade faster outdoors.** The `outdoor_age_speedup` mechanic means clouds last longest indoors.
- **Toolkit is a crafting tool.** It can't be activated directly on a corpse. Butcher first, then use the crafting menu.
- **Morale bonus is passive.** It's tied to having the profession trait, not to proximity of tamed creatures.

## Changelog

### v1.2.0
- 7 custom starting scenarios (one per specialty profession); spawn alongside tamed creatures from the start
- Wandering Tamer NPC with a full dialogue tree and two sequential quests:
  - "A Tamer's Errand": bring 5 cooked meat to earn a taming treat toolkit and learn the toolkit crafting recipe
  - "The Universal Formula": bring 3 meaty taming treats to learn the universal taming treat recipe
- Universal taming treat and toolkit recipes changed from autolearn to NPC-taught
- Profession balance pass: all 8 professions now start with equivalent medical supplies (3 bandages + 5 adhesive bandages) and 2 universal taming treats alongside their specialty treats
- All taming professions now require Survival 4 (ride without a saddle from the start)
- All creature overrides include `SILENTMOVES` for silent movement (0.I/TLG builds)
- Fixed flavor text mismatches: fowler toad/tadpole no longer described with feathers; coyote-shark mutant no longer described with antennae; cellar spider moved to spider message group
- Fixed "burrows through the food" phrasing on burrowing creatures
- Minor punctuation, spacing, and code style cleanup across all files

### v1.1.0
- Command items reworked: now trigger an adrenaline spike AOE instead of toggling docility; affected creatures get +30 speed, +3 STR, +2 DEX, and bonus melee damage for ~2 minutes, followed by a ~90-second crash with reduced stats
- 8 new toolkit converter recipes: 4 corpse-to-bomb and 4 corpse-to-incense, using butchered remains and the toolkit (no extra ingredients)
- Added flesh rope: a craftable binding item made from sinew, leather, fur, and tanned hide via the toolkit (yields 2 per craft)
- All 8 professions now start with 3 lengths of rope
- All creature overrides now include PET_MOUNTABLE; tamed creatures large enough to ride can be mounted
- 30 new craftable creature armor items: simple (leather) and reinforced (steel+leather) for all 15 body types; crafted with the taming treat toolkit and equipped via the pet interaction menu
- Each profession trait now grants a passive morale bonus (+10) via the EOC system; refreshes every ~5 in-game minutes with a 20-minute duration
- Added 7 custom morale types (one per specialty) and 7 Effect on Condition definitions for morale processing
- All taming professions start with attached ear plugs for noise protection against creature vocalizations
- Added 0_spells.json for adrenaline spike/crash spell definitions
- Replaced "animal" with "creature" throughout mod text where appropriate

### v1.0.0
- Initial public release
- 5 petfood categories: meat, veggie, tech, eldritch, universal
- 5 basic taming treats with crafting recipes; 13 vanilla item petfood extensions
- 5 throwable pacification bombs that deploy visible gas clouds for crowd-control taming
- 5 throwable healing incenses that deploy restorative clouds (2-4 HP per 10 turns)
- 5 themed command items for toggling tamed creatures between passive and aggressive
- Taming Treat Toolkit; a reusable crafting tool that converts butchered remains into treats (simplified recipes; no extra ingredients needed)
- 8 new taming-focused professions, each with specialty treats, a toolkit, bombs, incense, and command items
- 2 custom effects (Pacified, Soothing Vapors); 10 custom field types; 20 emitters
- Vanilla faction relationships preserved; untamed creatures behave naturally
