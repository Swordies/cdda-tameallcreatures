# Tame All Creatures

**Author:** Swordie
**Version:** 1.2.0
**Target:** Cataclysm: Dark Days Ahead 0.I

## Overview

This mod lets you tame and befriend every creature in CDDA; zombies, mi-go, robots, nether beings, all of them. It adds craftable taming treats, a corpse-to-treat conversion system, throwable pacification bombs that deploy visible gas clouds for crowd control, throwable healing incense for patching up your tamed creatures, command items for ordering pets around, and 8 new taming-focused professions. Vanilla faction relationships are preserved; untamed creatures still fight, flee, or coexist with each other as normal.

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

**Important:** The toolkit is a crafting tool, not an activatable item. You can't activate it directly; it works through the crafting menu. Think of it like a soldering iron or sewing kit.

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
Five themed command items that rally tamed creatures into a combat frenzy:

| Item | Theme |
|------|-------|
| Beast Commander's Horn | Animal bone horn |
| Insect Pheromone Vial | Synthetic pheromones |
| Tech Override Signal | EM pulse device |
| Eldritch Resonator | Dimensional crystal |
| Universal Tamer's Whistle | Multi-frequency whistle |

**Usage:** Activate to trigger an adrenaline spike in ALL nearby tamed creatures.  For about two minutes, affected creatures deal more damage and move faster; afterwards they suffer a brief crash with reduced stats as the rush wears off.  The adrenaline crash lasts about 90 seconds longer than the spike, so time your rallies carefully.

**Mechanical details:** Each command item casts a self-targeted AOE spell that applies both the Adrenaline Spike and Adrenaline Crash effects simultaneously.  The spike ends first, leaving the crash as a short vulnerability window.

### Flesh Rope
A craftable binding made from tanned hides, leather, and sinew.  Works as a standard rope for tying up creatures, restraining NPCs, or any other rope-based task.

**Crafting:** Requires the taming treat toolkit, sinew, leather, fur, and tanned hide.  Produces 2 flesh ropes per craft.  Survival 3.

### Creature Armor
Craftable armor for tamed creatures in two tiers:

| Tier | Material | Thickness | Skill | Time |
|------|----------|-----------|-------|------|
| Simple | Leather | 3 | Fabrication 3 | 60 min |
| Reinforced | Steel + Leather | 5 | Fabrication 5 | 120 min |

Armor is available for all 15 body types found in the mod's creature roster:

| Body Type | Label | Example Creatures |
|-----------|-------|-------------------|
| dog | canine | dogs, wolves, cats, coyotes |
| pig | stout | boars, large rodents |
| insect | arthropod | giant ants, centipedes |
| human | humanoid | zombies, feral humans |
| snake | serpentine | snakes, worms, grubs |
| flying insect | winged insect | wasps, bees, dragonflies |
| blob | amorphous | blobs, shoggoths |
| spider | arachnid | giant spiders |
| horse | equine | horses, deer, moose |
| migo | mi-go | mi-go and variants |
| crab | crustacean | crabs, lobsters |
| fish | aquatic | mutant fish |
| bear | ursine | bears, large mammals |
| bird | avian | birds, bats |
| kangaroo | macropod | large bipedal creatures |

**How to equip:** Walk up to a tamed creature, interact with it, and select "Equip with armor."  The game filters your inventory to show only armor that matches the creature's body type and size.

**Crafting:** All creature armor recipes require the taming treat toolkit.  Simple armor uses leather, sinew, and fur.  Reinforced armor adds steel chunks.

### Silent Tamed Creatures
All creature overrides include the `SILENTMOVES` flag, which eliminates footstep noise from tamed creatures entirely.  This means your tamed army won't keep you awake at night just by walking around.  All taming professions also start with a pair of attached ear plugs for additional noise protection against creature vocalizations that can't be silenced through JSON.

### Profession Morale Bonus
Each taming profession trait grants a passive morale bonus of +10 ("Bond with tamed [specialty]").  The bonus is processed via the Effect on Condition system; the trait's `processed_eocs` field fires every ~5 in-game minutes and refreshes a 20-minute morale buff with a 10-minute decay start.  This represents the tamer's deep satisfaction and confidence that comes from their expertise with their chosen creature type.

**Technical note:** The morale bonus is tied to having the profession trait, not to proximity of tamed creatures.  The CDDA engine doesn't expose a JSON-accessible way to count nearby friendly monsters; the bonus is designed as a passive reward for choosing a taming profession.

### Mounting
All creature overrides include the `PET_MOUNTABLE` flag, which lets you ride any tamed creature that meets the engine's size and weight requirements.  The game checks three things: the creature must be at least one size category larger than you, it must be friendly (tamed), and your weight must not exceed 20% of the creature's weight.  In practice, this means most large and huge creatures can be ridden, while smaller or lighter ones can't.  Heavier creatures like moose, bears, and hulks make reliable mounts; lighter ones like the antlered horror may reject riders who carry too much gear.  All taming professions start with Survival 4, which lets you ride without a saddle.

### Starting Scenarios
Seven custom scenarios, each paired with one taming profession, that spawn you alongside tamed creatures from your specialty:

| Scenario | Profession | Starting Pets |
|----------|-----------|---------------|
| Beast Tamer's Menagerie | Beast Tamer | Dog + tabby cat |
| Insect Handler's Nest | Insect Tamer | 2 small bees + small ant |
| Dinosaur Wrangler's Camp | Dino Wrangler | Raptor |
| Demonologist's Sanctum | Demonologist | Kreck |
| Machine Whisperer's Workshop | Machine Whisperer | Manhack |
| Mycologist's Grove | Mycologist | Young fungaloid + 2 spores |
| Zombie Whisperer's Refuge | Zombie Whisperer | Zombie |

Each scenario restricts profession selection to its paired profession and costs -2 to -3 character points.  Pets spawn pre-tamed and follow you from the first turn.

**Note:** Scenarios aren't available in the Bright Nights build; BN doesn't support the scenario `pets` field.

### Wandering Tamer NPC
A unique NPC who appears in the game world and offers two sequential quests:

**Quest 1: A Tamer's Errand**
- Bring the tamer 5 pieces of cooked meat
- Reward: a taming treat toolkit + the recipe to craft your own

**Quest 2: The Universal Formula**
- Bring the tamer 3 meaty taming treats
- Reward: the universal taming treat recipe (the only way to learn it)

The Wandering Tamer has a full dialogue tree that recognizes whether you have a taming profession trait.  Their dialogue covers the basics of taming; treat types, toolkit usage, and creature handling.

**Important:** The universal taming treat and toolkit recipes are no longer autolearned.  You must complete the NPC quests to learn them, or play a taming profession that starts with both items already in your inventory.

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

Each profession has a unique trait with a passive morale bonus, themed gear, a generous supply of taming treats (including 2 universal treats), medical supplies, and a pair of attached ear plugs for sleeping near tamed creatures.

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
| `0_spells.json` | 2 spells (adrenaline spike + crash for command items) |
| `converter_recipes.json` | 15 converter recipes (6 treat + 4 bomb + 4 incense + 1 flesh rope) |
| `pet_armor_items.json` | 30 creature armor items (15 bodytypes x 2 tiers) |
| `pet_armor_recipes.json` | 30 creature armor crafting recipes |
| `scenarios.json` | 7 custom starting scenarios with tamed pets |
| `npc_tamer.json` | Wandering Tamer NPC class, item groups, and template |
| `npc_tamer_dialogue.json` | 3 talk topics for the Wandering Tamer dialogue tree |
| `npc_tamer_missions.json` | 2 mission definitions (toolkit quest + universal recipe quest) |
| `item_extensions.json` | 13 vanilla item petfood extensions |
| `morale_types.json` | 7 custom morale type definitions |
| `morale_eocs.json` | 7 Effect on Condition definitions for morale processing |
| `monster_overrides_1-6.json` | 1,121 monster overrides (petfood taming data) |
| `professions.json` | 7 traits (with morale EOCs) + 8 professions (each starts with rope and ear plugs) |

## Known Limitations

- **Taming is single-target.** Engine limitations mean treats have to be used one creature at a time. The pacification cloud workaround lets you daze groups first for easier sequential taming.
- **Tamed zombies attack friendly NPCs.** This is a hardcoded engine limitation ([GitHub #78467](https://github.com/CleverRaven/Cataclysm-DDA/issues/78467)). The CDDA engine explicitly prevents zombie-species monsters from being friendly to NPCs, even when tamed. Only the ~86 monsters with the ZOMBIE species are affected; the other ~1,095 creatures (animals, insects, robots, mi-go, nether beings, mutants, etc.) behave correctly when tamed and won't attack friendly NPCs.
- **Healing is area-based.** There's no way to heal one specific tamed monster. The healing cloud affects everything in the area, including wild creatures and you. Monster healing uses the REGEN_HP enchantment system; the cloud adds ~2 HP/turn to any creature standing in it.
- **Pacification hits everyone.** The pacification cloud doesn't pick sides. You, your NPCs, and your tamed creatures all get affected if they walk into it.
- **Clouds fade faster outdoors.** The `outdoor_age_speedup` mechanic means clouds last longest indoors.
- **Toolkit is a crafting tool.** The toolkit can't be activated directly on a corpse. You must first butcher the corpse for parts, then use the crafting menu (`&`) to make treats.
- **Morale bonus is passive.** The profession morale bonus is tied to having the trait, not to proximity of tamed creatures.  The CDDA engine doesn't provide a JSON-accessible way to detect nearby friendly monsters.

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

### v1.1.0
- Command items reworked: now trigger an adrenaline spike AOE instead of toggling docility; affected creatures get +30 speed, +3 STR, +2 DEX, and bonus melee damage for ~2 minutes, followed by a ~90-second crash with reduced stats
- 8 new toolkit converter recipes: 4 corpse-to-bomb and 4 corpse-to-incense, using butchered remains and the toolkit (no extra ingredients)
- Added flesh rope: a craftable binding item made from sinew, leather, fur, and tanned hide via the toolkit (yields 2 per craft)
- All 8 professions now start with 3 lengths of rope
- All creature overrides now include PET_MOUNTABLE; tamed creatures large enough to ride can be mounted
- 30 new craftable creature armor items: simple (leather) and reinforced (steel+leather) for all 15 body types; crafted with the taming treat toolkit and equipped via the pet interaction menu
- Each profession trait now grants a passive morale bonus (+10) via the EOC system; refreshes every ~5 in-game minutes with a 20-minute duration
- Added 7 custom morale types (one per specialty) and 7 Effect on Condition definitions for morale processing
- All creature overrides include the `SILENTMOVES` flag; tamed creatures no longer make footstep sounds
- All taming professions start with attached ear plugs for additional noise protection against creature vocalizations
- Added 0_spells.json for adrenaline spike/crash spell definitions
- Replaced "animal" with "creature" throughout mod text where appropriate

### v1.2.0
- 7 custom starting scenarios (one per specialty profession); spawn alongside tamed creatures from the start
- Wandering Tamer NPC with a full dialogue tree and two sequential quests:
  - "A Tamer's Errand": bring 5 cooked meat to earn a taming treat toolkit and learn the toolkit crafting recipe
  - "The Universal Formula": bring 3 meaty taming treats to learn the universal taming treat recipe
- Universal taming treat and toolkit recipes changed from autolearn to NPC-taught
- Profession balance pass: all 8 professions now start with equivalent medical supplies (3 bandages + 5 adhesive bandages) and 2 universal taming treats alongside their specialty treats
- All taming professions now require Survival 4 (ride without a saddle from the start)
- All creature overrides include `SILENTMOVES` for silent movement; tamed creatures no longer generate footstep noise
- Fixed flavor text mismatches: fowler toad/tadpole no longer described with feathers; coyote-shark mutant no longer described with antennae; cellar spider moved to spider message group
- Fixed "burrows through the food" phrasing on burrowing creatures
- Minor punctuation, spacing, and code style cleanup across all files
