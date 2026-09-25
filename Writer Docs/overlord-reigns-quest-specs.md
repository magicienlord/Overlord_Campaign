# Overlord Reigns: quest specs (triggers, objectives)

A Twine link only means one quest is a prerequisite for another. The TRIGGER is what actually makes a quest appear once its prerequisites are done. All IDs below were checked against the pack's jars. Unless noted, a chain quest's trigger is simply "the previous quest in the chain is done".

**Rewards: none anywhere.** Neither quests nor Ramblings give rewards. (This replaces the earlier "milestones only" answer.)

## Ramblings (a separate content type, not quests)
Ramblings are a set of achievements that aren't used by any quest objective. Each adds a fun lore entry to the log: a TRIGGER POPUP + a fuller log entry, with NO completion popup and NO completion entry. Not every achievement qualifies: only those that mark a particular feat or completion, or are tied to a mod that matters to the campaign. Selection happens PER MOD, but only AFTER the campaign structure is finished (so no advancement already used as an objective becomes a Rambling).

## Prologue
- **Our New Overlord**: Trigger: first login. Objective: read the entry.
- **A New Master** (Browns): Trigger: Our New Overlord done. Objectives: obtain the Master Staff (`minionsremastered:masters_staff`), summon a Brown.
- **Seat of the Overlord**: the throne room, the FIRST room restoration, which unlocks the other rooms. Trigger: A New Master done. Objective: place a Necrolord chair (`fantasyfurniture:necrolord/chair`).
- **A Reign Unfolds**: the start of the exploration route. Trigger: A New Master done, unlocking together with the restoration route so Gnarl can speak to both of the player's wants at the start of the game. Completes when the player leaves the Dark Tower biome.

## Hives
- **Restore the Reds**: Trigger: A New Master done. Objective: obtain a blaze rod.
- **Restore the Greens**: Objectives: have Poison, then kill a witch.
- **Restore the Blues**: Objective: kill an Elder Guardian.
- **A Complete Horde**: Objective: read. Celebration.

## Tower rooms
Trigger for every room: Seat of the Overlord done. Objective: place the listed block.
- **Fire & Iron**: `hot_iron:smithing_anvil` (Smithing Anvil)
- **A Place for Everything**: `storagedrawers:controller` (Drawer Controller)
- **An Armory Worth Seeing**: `display_case:display_case`
- **The Tower Heart?**: any Waystone (tag `waystones:waystones`, or any `waystones:*waystone`)
- **The Alchemy Den**: `elixirum:glass_cauldron`
- **The Theurgy Lab**: `theurgy:pyromantic_brazier`
- **Gristle's Kitchen**: `farmersdelight:cooking_pot`
- **The Spell Study**: `irons_spellbooks:inscription_table`
- **The Eidolons Chamber**: `eidolon:worktable` (Magic Workbench)
- **Gnarl's Secret Project**: a lore buffer before the Biomancy chain. Objective: read the entry.
- **Enchantment Room**: `minecraft:enchanting_table`
- **Your Chambers, Sire**: `fantasyfurniture:necrolord/bed_double`
- **A Golden Start**: `iceandfire:gold_pile` (Pile of Gold)
- **The Arena**: `domesticationinnovation:drum` (Command Drum)
- **Behind the Bars**: `supplementaries:cage`
- **Beasts Pen**: `domesticationinnovation:pet_bed_*` (any colour)
- **A Tower Complete**: automatic once all 16 rooms are restored.

## Room chains (voiced mod tutorials)
### Theurgy (after The Theurgy Lab), following the Hermetica's chapters
- **Three Principles**: obtain one each of `#theurgy:alchemical_sulfurs`, `#theurgy:alchemical_salts`, `theurgy:mercury_shard`.
- **Reassembling Matter**: place `theurgy:incubator` (incubation).
- **Laws of Repetition**: place `theurgy:reformation_source_pedestal`, `theurgy:reformation_target_pedestal`, `theurgy:reformation_result_pedestal` (replication by reformation).
- **Crossing the Boundary**: place `theurgy:fermentation_vat` (replication by transmutation).

### Eidolon (after The Eidolons Chamber)
- **A Ritual that Works**: advancement `eidolon:soul_shard` (Crystallization Ritual at the Brazier).
- **Prepare the Offering**: advancement `eidolon:incense` (burn Offering Incense on an Altar).
- **Words that Answer**: advancement `eidolon:flame_spell` (learn the Chant of Flames by researching a Blaze).
- **Sacred or Wicked**: a REAL fork, decided by PERFORMING the path's ritual (learning a Sign alone doesn't lock the other path). OR gate: Sacred = advancement `eidolon:holy_symbol` (transfigure a Gold Inlay into the Holy Symbol); Wicked = advancement `eidolon:unholy_symbol` (transfigure a Pewter Inlay into the Unholy Symbol). Whichever comes first completes the quest. CODER NOTE: tag the path so Gnarl can react.

### Biomancy (after Gnarl's Secret Project)
- **A Fleshy Core**: obtain `biomancy:primordial_core`.
- **A Cradle for Flesh**: place `biomancy:primordial_cradle`.
- **Flesh Reborn... Almost**: obtain `biomancy:living_flesh`.
- **No Mouth, Must Work**: place `biomancy:decomposer`.
- **Directed Life**: advancement `biomancy:biomancy/bio_injector`.

### Spell Study (after The Spell Study)
- **Practical Spellcraft**: write a scroll into a spellbook (inscribe a spell at the Inscription Table).
- **Shape the Mana**: advancement `irons_spellbooks:make_scroll_forge`.
- **More than a Weapon**: advancement `irons_spellbooks:make_arcane_anvil`.
- **A New Power Balance**: OR gate: cast a level 10 Blood spell / cast a level 10 Holy spell.

### Gristle's Kitchen (after Gristle's Kitchen; presented by Gristle)
- **Start with Dinner**: craft a Farmer's Delight meal (`#farmersdelight:meals`).
- **Food Shaman**: craft a feast.
- **An Estate Worth Feeding**: place `farmersdelight:rich_soil_farmland`.
- **Small Hands for Small Work**: create a Crop Critter (Crop Critters).
- **A Harvest Worth Automating**: create a Hay Golem (Golem Overhaul).
- **The Assisted Estate**: 20 crops harvested by Crop Critters (needs a coder hook / counter).

### Alchemy Den (after The Alchemy Den; presented by Blister)
- **Knowledge of the Earth**: obtain `elixirum:extract` (draw an essence from an ingredient with Honey Solvent).
- **A Deliberate Formula**: brew a potion WITH INTENT, i.e. from a known recipe or known essence (not a random Suspicious Mixture).
- **Evil's Formula**: master one potion (Elixirum recipe mastery).

### Forge (presented by Giblet the Sixth)
- **A Forge for Dragons** (needs Fire & Iron AND The Master Takes Wing): place any `iceandfire:dragonforge_*_core`.
- **DragonSteel**: obtain any `iceandfire:dragonsteel_*_ingot`.

### Quaver's Band (presented by Quaver). These are real quests Quaver asks for, with objectives.
- **A Band for the Dark Tower** (Quaver's Request): obtain 4 different Immersive Melodies instruments.
- **A Whole Orchestra**: obtain all 11 instruments (bagpipe, didgeridoo, flute, lute, piano, triangle, trumpet, tiny drum, vielle, ender bass, handpan).

## Exploration hooks (unlocked by A Reign Unfolds; each needs A Reign Unfolds done)
TRIGGERS approved. OBJECTIVES of the faction introductions are still to be defined.

### Faction introductions
- **Spree, Again**: enter any village (`#minecraft:village`).
- **The Bastille**: enter `takesapillage:bastille`.
- **The Successor Hold**: enter `dwarven_forge:dwarven_village`.
- **The Gnumu Settlement**: within 16 blocks of any Gnumus (`gnumus:gnumus_worker` / `_merchant` / `_hunter` / `_shaman`). The mod has no structure ID.
- **The Goblin Camp**: enter `goblins_tyranny:goblinscamp`.
- **The Den Below**: enter `kobolds:kobold_den` or `kobolds:kobold_den_pirate`.
- **The Ribbit Village**: enter `ribbits:ribbit_village`.
- **The Village beneath**: within 16 blocks of any Mermorph (`seadwellers:mermorph*`). No structure ID in the jar.
- **Gold in the Netherworld**: enter `nether_villages:nether_village`.
- **The Grove and its God**: enter `mowziesmobs:umvuthana_grove`.
- **The Chosen Colony**: within 24 blocks of any Myrmex (`iceandfire:myrmex_*`); hives aren't structures.

### Side-story hooks
- **Places the Dead Keep**: enter ANY structure from The Graveyard mod (`graveyard:*`).
- **A Hive Without End**: enter the Bumblezone dimension (`the_bumblezone:the_bumblezone`).
- **The Great Chalice**: obtain `knightquest:small_essence`.
- **A Castle Off the Map**: enter `tlc:lost_castle`.
- **A Workforce with Tails**: within 16 blocks of `rats:rat`.
- **Where the Orchids Gather**: enter `oddities:orchid_shrine`.
- **A Shadow with Wings**: within 48 blocks of any Ice and Fire fire/ice/lightning dragon.
- **An Aberration on the Line**: advancement `fathoms:nautical/catch_aberration`.
- **A Collar Left Behind**: a tamed pet dies (coder hook).
- **First Blood**: the player becomes a vampire in Nycto (coder hook).
- **A Tainted Essence** (starts the main plot): also triggered by a Knight Quest small essence (`knightquest:small_essence`). How it's told apart from The Great Chalice's trigger is still to be settled.
