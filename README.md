# Tame All Creatures

**Author:** Swordie
**Version:** 1.0.0 
**Target:** Cataclysm: Dark Days Ahead 0.H (Herbert)

## Overview

This mod lets you tame and befriend every creature in CDDA: zombies, mi-go, robots, nether beings, all of them! It adds craftable taming treats, a corpse-to-treat conversion system, throwable pacification bombs that deploy visible gas clouds for crowd control, throwable healing incense for patching up your tamed creatures, command items for ordering pets around, and 8 new taming-focused professions. Vanilla faction relationships are preserved; untamed creatures still fight, flee, or coexist with each other as normal.

## Features

### Taming Treats (Basic)
Five types of craftable treats, each used on a single creature to tame it:

| Treat | Target Creatures | Crafting Skill |
|-------|-----------------|----------------|
| Meaty Taming Treat | Zombies, animals, dinosaurs | Cooking 3 |
| Herbal Taming Treat | Insects, fungi, plants | Cooking 3 |
| Electronic Taming Module | Robots, cyborgs, turrets | Electronics 4 |
| Eldritch Taming Offering | Nether creatures, mi-go | Cooking 5 |
| Universal Taming Treat | ALL creatures | Cooking 6 |

**Usage:** Activate the treat while standing next to a creature to try taming it.

### Taming Treat Toolkit & Corpse Conversion
A reusable crafting tool that converts butchered creature remains into taming treats.

**How to use the toolkit (step by step):**
1. Kill a creature.
2. Butcher the corpse (press `B` or use your butchery menu) to collect meat, tainted flesh, vegetables, or electronic scrap.
3. Open the **crafting menu** (press `&`).
4. Search for the treat you want to make (e.g. "meaty taming treat" or "eldritch taming offering").
5. The recipe will appear as long as you have the toolkit in your inventory and the required ingredients.
6. Craft the treats. The toolkit is never consumed; you keep it forever.

**Important:** The toolkit is a crafting tool, not an activatable item. You cannot activate it directly; it works through the crafting menu. Think of it like a soldering iron or sewing kit.

| Input Material | Output Treat | Notes |
|---------------|-------------|-------|
| Fresh meat (`meat`, `meat_cooked`, `fish_cooked`, `meat_smoked`, `human_flesh`) | Meaty Taming Treat (x3) | From animals, humans, dinosaurs. Zombies only drop tainted meat; use eldritch recipe for those. |
| Fresh vegetables (`veggy`, `veggy_cooked`, `dry_fruit`, `birdfood`, `cattlefodder`, `wild_herbs`) | Herbal Taming Treat (x3) | From insects, fungi, plants, and herbivores. |
| Electronic parts (`e_scrap`, `processor`) | Electronic Taming Module (x3) | From robots and cyborgs. Requires soldering iron. |
| Tainted flesh (`meat_tainted`, `veggy_tainted`) | Eldritch Taming Offering (x3) | From nether creatures, mutants, and zombies. The only treat path for zombie remains. |
| Any 2 specialty treats | Universal Taming Treat (x2) | Combines any two treat types into universal ones. |

**Zombie balance:** Zombie corpses yield `meat_tainted` when butchered. This can't be turned into meaty treats; only eldritch offerings. This keeps zombies from becoming a free, infinite source of easy meaty treats while still giving their remains a use through the eldritch recipe. Eldritch treats work on nether creatures, mi-go, and other horrors.

**Simplified recipes:** All corpse-to-treat conversion recipes require only the butchered remains and the toolkit. No extra ingredients like salt or water needed.

**Toolkit crafting:** The toolkit is craftable from steel, plastic, duct tape, a knife, and a pot (Fabrication 3). All taming professions start with one.

### Fragrant Pacification Bombs
Five types of throwable devices that release a sustained pacification cloud:

| Bomb | Cloud Type | Crafting Skill |
|------|-----------|----------------|
| Fragrant Meaty Pacification Bomb | Meaty haze | Cooking 5 |
| Fragrant Herbal Pacification Bomb | Herbal haze | Cooking 5 |
| Fragrant Electronic Pacification Bomb | EM field | Electronics 6 |
| Fragrant Eldritch Pacification Bomb | Eldritch miasma | Cooking 7 |
| Fragrant Universal Pacification Bomb | Universal cloud | Cooking 8 |

**How to use pacification bombs (step by step):**
1. **Wield** the bomb (press `w` and select it).
2. **Activate** it (press `a`). This "pulls the pin" and transforms it into an active bomb.
3. **Throw** it where you want the cloud (press `t`). The bomb lands on the ground and starts emitting gas.
4. The cloud builds up over the following turns, spreading outward.
5. Any creature that steps into the cloud gets Pacified; dazed, slowed (-40 speed), and with reduced perception and dexterity for 5-10 minutes.
6. While a creature is pacified, walk up and use a regular taming treat to finish the tame.

The active bomb sits on the ground and continuously emits gas for about 3 hours before burning out. The cloud spreads over time and fades faster outdoors.

**Intended workflow for group taming:** Throw a pacification bomb into a group of monsters, wait for the cloud to spread, then walk through and feed treats to the dazed creatures one at a time.

**Warning:** The pacification effect hits YOU and friendly NPCs too. Throw the bomb away from yourself, or deal with the speed and perception penalties.

### Healing Incense
Five types of throwable items that release a sustained healing cloud:

| Incense | Cloud Type | Crafting Skill |
|---------|-----------|----------------|
| Meaty Healing Incense | Meaty restorative vapor | Cooking 5 + First Aid 3 |
| Herbal Healing Incense | Herbal restorative vapor | Cooking 5 + First Aid 3 |
| Nanite Repair Canister | Nanite repair cloud | Electronics 6 + First Aid 3 |
| Eldritch Mending Censer | Eldritch mending miasma | Cooking 7 + First Aid 3 |
| Universal Healing Incense | Universal restorative mist | Cooking 8 + First Aid 4 |

**How to use healing incense (step by step):**
1. **Wield** the incense (press `w` and select it).
2. **Activate** it (press `a`). This lights it and transforms it into an active incense.
3. **Throw** it where you want the healing zone (press `t`), or just drop it at your feet.
4. The incense sits on the ground and continuously emits healing vapor.
5. Any creature standing in the cloud gets the Soothing Vapors effect, healing 2-4 HP every 10 turns.
6. The incense burns for about 3 hours before going out.

**Tip:** The healing cloud works on you too. Throw one at your base and you can recover alongside your pets.

### Command Items
Five themed command items that toggle tamed creatures between passive and aggressive:

| Item | Theme |
|------|-------|
| Beast Commander's Horn | Animal bone horn |
| Insect Pheromone Vial | Synthetic pheromones |
| Tech Override Signal | EM pulse device |
| Eldritch Resonator | Dimensional crystal |
| Universal Tamer's Whistle | Multi-frequency whistle |

**Usage:** Activate to switch nearby tamed creatures between passive/aggressive behavior.

### Professions
Eight new professions, each starting with themed taming treats, a command item, a pacification bomb, healing incense, and a toolkit:

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

Each profession has a unique trait, themed gear, and a generous supply of taming treats (10+ of their specialty type).

## Installation

1. Copy the `TameAllCreatures` folder into your CDDA `data/mods/` directory.
2. Start a new game (or load an existing one) and enable "Tame All Creatures" in the mod list.

## File Structure

| File | Contents |
|------|----------|
| `modinfo.json` | Mod metadata |
| `taming_items.json` | 5 basic taming treat items |
| `fragrant_items.json` | 10 items (5 inactive + 5 active pacification bombs) |
| `healing_items.json` | 10 items (5 inactive + 5 active healing incenses) |
| `command_items.json` | 5 command items |
| `effects.json` | Custom effects (Pacified, Soothing Vapors) |
| `field_types.json` | 10 custom field types (5 pacification + 5 healing) |
| `emitters.json` | 20 emitters (10 burst + 10 stream for continuous emission) |
| `recipes.json` | 5 basic treat recipes |
| `fragrant_recipes.json` | 5 pacification bomb recipes |
| `healing_recipes.json` | 5 healing incense recipes |
| `command_recipes.json` | 5 command item recipes |
| `converter_items.json` | Taming treat toolkit item |
| `converter_recipes.json` | 6 corpse-to-treat conversion recipes |
| `item_extensions.json` | 13 vanilla item petfood extensions |
| `monster_overrides_1-6.json` | 1,121 monster overrides (petfood taming data) |
| `professions.json` | 7 traits + 8 professions |

## Known Limitations

- **Taming is single-target.** Engine limitations mean treats have to be used one creature at a time. The pacification cloud workaround lets you daze groups first for easier sequential taming.
- **Tamed zombies attack friendly NPCs.** This is a hardcoded engine limitation ([GitHub #78467](https://github.com/CleverRaven/Cataclysm-DDA/issues/78467)). The CDDA engine explicitly prevents zombie-species monsters from being friendly to NPCs, even when tamed. Only the ~86 monsters with the ZOMBIE species are affected; the other ~1,095 creatures (animals, insects, robots, mi-go, nether beings, mutants, etc.) behave correctly when tamed and will not attack friendly NPCs.
- **Healing is area-based.** There's no way to heal one specific tamed monster. The healing cloud affects everything in the area, including wild creatures and you. In the 0.I version, the engine does not support enchantment-based regeneration; healing incense only heals the player character, not tamed monsters.
- **Pacification hits everyone.** The pacification cloud doesn't pick sides. You, your NPCs, and your tamed creatures all get affected if they walk into it.
- **Clouds fade faster outdoors.** The `outdoor_age_speedup` mechanic means clouds last longest indoors.
- **Toolkit is a crafting tool.** The toolkit cannot be activated directly on a corpse. You must first butcher the corpse for parts, then use the crafting menu (`&`) to make treats.

## Changelog

### v1.0.0
- Initial public release
- 1,121 monster overrides across all vanilla creature types
- 5 petfood categories: meat, veggie, tech, eldritch, universal
- 5 basic taming treats with crafting recipes; 13 vanilla item petfood extensions
- 5 throwable pacification bombs that deploy visible gas clouds for crowd-control taming
- 5 throwable healing incenses that deploy restorative clouds (2-4 HP per 10 turns)
- 5 themed command items for toggling tamed creatures between passive and aggressive
- Taming Treat Toolkit; a reusable crafting tool that converts butchered remains into treats (simplified recipes; no extra ingredients needed)
- 8 new taming-focused professions, each with specialty treats, a toolkit, bombs, incense, and command items
- 2 custom effects (Pacified, Soothing Vapors); 10 custom field types; 20 emitters
- Vanilla faction relationships preserved; untamed creatures behave naturally
- 21 files (20 JSON + README) — 0.H backport
