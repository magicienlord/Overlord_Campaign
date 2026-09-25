# Overlord Reigns: quest specs, part 3 (side stories)

Continues parts 1 and 2. A chain quest's trigger is "the previous quest is done" unless noted. Discovery triggers for the first quest of each line are listed in part 1 ("Side-story hooks").

## Graveyard / Lich (the Lich is a rival dark lord)
- **Places the Dead Keep** (trigger: enter any `graveyard:*` structure): kill 5 Graveyard undead (`graveyard:acolyte` / `ghoul` / `revenant` / `reaper` / `nightmare` / `wraith`).
- **The Bone Staff**: obtain any `graveyard:*_bone_staff`.
- **An Invitation to the Lich**: enter `graveyard:lich_prison`.
- **The Corrupted Champion**: kill `graveyard:lich`.

## Bumblezone (Gnarl's disgust at anything sweet)
- **A Hive Without End** (trigger: enter the Bumblezone): read.
- **The Queen's Domain**: within 8 blocks of `the_bumblezone:bee_queen`.
- **Essence of the Hive**: obtain `the_bumblezone:essence_of_the_bees`.

## Rats / Ratlantis (comedy; Ratlantis is where Gnarl draws the line)
- **A Workforce with Tails** (trigger: within 16 blocks of `rats:rat`): tame a `rats:rat`.
- **An Empire of Cheese**: obtain `rats:cheese`.
- **The Gem of Ratlantis**: obtain `rats:gem_of_ratlantis`.
- **The Rat Baron**: kill `rats:rat_baron`.
- **Back from Ratlantis**: return to the Overworld after visiting the Ratlantis dimension.

## Orchid Altar (Bosses Oddities)
- **Where the Orchids Gather** (trigger: enter `oddities:orchid_shrine`): right-click `oddities:orchid_altar`.
- **A Heart for the Altar**: obtain `oddities:orchid_heart` and use it on the altar.
- **Cut Down the Queen**: kill `oddities:queen_of_orchid`.

## Vampire (Nycto; presented by Lestat)
- **First Blood**: Trigger: advancement `nycto:nycto/become_vampire` (drink Vampire Blood). No coder hook needed. Objective: `nycto:nycto/extract_blood_bottle`.
- **The Hunter**: kill a `nycto:hunter`.
- **The Price of Power**: advancement `nycto:nycto/obtain_vampire_power` (use a Vampire Altar to pick a first power).

## Pet Cemetery (bittersweet; presented by Mortis)
- **A Collar Left Behind**: Trigger: obtain `pet_cemetery:pet_collar` (dropped when a pet dies). No coder hook needed. Objective: read.
- **The Grave Gives Something Back**: OR `pet_cemetery:nether/respawn_pet` / `pet_cemetery:nether/respawn_zombie_pet`.
- **A Death Reversed**: `pet_cemetery:nether/cured_zombie_pet`.

## Aberrations (Fathoms, jar `overlord-depths`; presented by the Collector)
The Twine titles match Fathoms' own advancements.
- **An Aberration on the Line** (trigger: `fathoms:nautical/catch_aberration`): `fathoms:nautical/cut_aberration`.
- **Lost in Translation**: `fathoms:nautical/open_message_in_a_bottle`.
- **The Sunken Record**: `fathoms:nautical/obtain_all_sunken_scrawls`.
- **Rocky Waters**: `fathoms:nautical/enter_rocky_waters`.
- **Weight of the World**: `fathoms:nautical/perform_ritual`.

## The Lost Castle (`tlc`; the mod adds no mobs or items)
- **A Castle Off the Map** (trigger: enter `tlc:lost_castle`): read.
- **Break the Lost Court**: kill 10 hostile mobs inside the castle's bounds.
- **What the Castle Kept**: open the throne-room treasure chest (coder hook on loot table `tlc:chests/treasure`).

## Dragon (Ice and Fire), leading into A Forge for Dragons
- **A Shadow with Wings** (trigger: within 48 blocks of an Ice and Fire dragon): read.
- **Take the Measure**: advancement `iceandfire:iceandfire/bestiary`.
- **Steal the Future**: advancement `iceandfire:iceandfire/dragon_egg`.
- **The Master Takes Wing**: tame an Ice and Fire dragon (`questlog:entity_tame` on fire/ice/lightning dragon) and ride it (coder check).

## Twilight Forest (refuge of Queen Fay's Sanctuary elves)
- **Old Forest, New Master**: Trigger: when the Ribbit OR the Grove (Umvuthi) questline unlocks. Gnarl senses elven magic and traces it to the Twilight Forest. Objective: ENTER the Twilight Forest. (It unlocks once, whichever comes first.)
- **The Forest's First Keepers** (NEW passage, to add to the Twine between Old Forest, New Master and Maze & Fire): `twilightforest:progress_naga` + `twilightforest:progress_lich`.
- **Maze & Fire**: `twilightforest:progress_labyrinth` + `twilightforest:progress_hydra`.
- **Towers in the Gloom**: `twilightforest:progress_knights` + `twilightforest:progress_ur_ghast`.
- **The Frozen Queen**: `twilightforest:progress_yeti` + `twilightforest:progress_glacier`.
- **Giants Above**: `twilightforest:progress_troll`.
