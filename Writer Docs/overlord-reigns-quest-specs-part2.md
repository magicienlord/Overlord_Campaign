# Overlord Reigns: quest specs, part 2 (main plot and faction intros)

Continues `overlord-reigns-quest-specs.md`. Where the two disagree, this file wins (e.g. it settles A Tainted Essence vs The Great Chalice).

## Faction introductions: objective
Each of the 11 faction intros (Spree, Again · The Bastille · The Successor Hold · The Gnumu Settlement · The Goblin Camp · The Den Below · The Ribbit Village · The Village beneath · Gold in the Netherworld · The Grove and its God · **The Mound-Dwellers** (formerly "The Chosen Colony")) completes when the player places ANY banner inside that settlement's structure bounds (the coder checks the position). For the three factions with no structure ID (Gnumus, Mermorphs, Myrmex), the banner must be placed within 16 blocks of one of that faction's mobs.

## Essence / Great Chalice line (Knight Quest)
- **A Tainted Essence** (starts the main plot): Trigger: first `knightquest:small_essence` obtained (A Reign Unfolds done). Objective: read. It unlocks We Need a Bigger Sword, Cataclysm, An Aberration on the Line and The Great Chalice.
- **The Great Chalice**: Trigger: A Tainted Essence done. Objective: place `knightquest:great_chalice`.
- **The Great Essences**: obtain `knightquest:great_essence` and `knightquest:filled_goblet` (charge the Chalice).
- **Radiance for the Vessel**: obtain `knightquest:radiant_essence`.
- **The Architect of Chaos**: kill `knightquest:netherman`.

## We Need a Bigger Sword and the five gates (Bosses'Rise, `block_factorys_bosses`)
- **We Need a Bigger Sword**: Trigger: A Tainted Essence done + enter any Bosses'Rise structure. Objective: read.
- Each gate has 3 steps. Step 1 = enter the lair (the trigger/objective of the first quest). Step 2 = a boss-specific clue. Step 3 = kill the boss.

| Gate chain | Step 1: enter | Step 2 | Step 3: kill |
|---|---|---|---|
| A Hunger in the Frozen North > What the Frost Made > Silence the North | `block_factorys_bosses:yeti_hideout` | kill 5 `frozen_skeleton` | `yeti` (Skor) |
| Movement Beneath the Ruborian Sands > Blood Beneath the Armor > Empty the Desert | `sandworm_nest` | find the corpse in the nest: right-click `block_factorys_bosses:corpse`, then read | `sandworm` (Sirok) |
| A Dead Dragon Flies > Heraldry of the Raised > Undo the Resurrection | `dragon_tower` | find the `dragon_skull` block | `infernal_dragon` (Ashlord) |
| A Familiar Weight Below > The Door to an Old Reign > One Reign Must End | `underworld_arena` | obtain `underworld_arena_key` | `underworld_knight` (Helvar, the 3rd Overlord) |
| The Sea Has Been Keeping Something > Part of the Sea > Cut the Ocean's Threat | `kraken_ship` | kill `pirate_captain` | `kraken` (Nerakyss) |

All five step-3 quests are prerequisites for **A Single Wound** (fix: link Silence the North > A Single Wound).

## Finale
- **A Single Wound**: Trigger: all 5 gates done. Objective: read. (Plants the idea of one origin; doesn't reveal the End.)
- **The Wound Beyond the World**: enter the End (`minecraft:the_end`). The reveal.
- **Sever the Anchor**: kill `minecraft:ender_dragon`. Gnarl senses the lost Tower Heart at the rift's heart.
- **A Seed of the Heart** (NEW passage, add to the Twine after Sever the Anchor; working title, the jab pass renames it): Trigger: Sever the Anchor done. Objective: obtain `minecraft:dragon_egg` (holding it is enough; no placement step). Checking vanilla advancement `minecraft:end/dragon_egg` is equivalent.
  - **Lore (Archivist's ruling):** the Dragon Egg is a SEED OF THE TOWER HEART, the fragment the Anchor crystallised around. Most of the Heart is still lost in the rift. The seed CALLS TO THE REST, pulling toward the missing Heart deeper in the Wound. That pull is why the postgame pushes outward into the rift.
  - The egg is optional for the credits: the quest stays open afterwards if the player leaves without it.
- **End Credits**: fires when the player enters the End exit portal after the dragon dies (vanilla timing), whether or not the egg was taken. Objective: read. The single ending in canon End_Scene style, built from stat tags. CODER: it replaces Minecraft's End Poem / credits at that same portal moment; no new gates or blockers are added.
  - **Stat tags read by the ending:** each faction's fate (P/S/D) · Sacred or Wicked path · whether he turned vampire · how many side lines he finished · **whether he held the Heart's seed** (A Seed of the Heart done before entering the exit portal). With the seed, Gnarl closes on the Heart coming home and calling to the rest; without it, on the Heart left behind in the rift.

## Postgame ("the Wasteland" = the End)
The seed's pull toward the rest of the Heart is the thread that leads the Overlord outward (writer: weave it into these entries).
- **Return to the Wasteland**: advancement `minecraft:end/enter_end_gateway`.
- **A Thriving Wound**: visit any Outer End biome (`outer_end:azure_forest` / `outer_end:crystal_crag` / `outer_end:primordial_pools`).
- **Cities at the Edge**: enter `minecraft:end_city` (reworked by Better End Cities).
- **Far Edge of the Reign**: enter `outer_end:catacombs` AND `outer_end:end_tower`.

## Cataclysm (L_Ender's Cataclysm, optional scars of the Wound)
- **Cataclysm** hub: Trigger: A Tainted Essence done + enter any Cataclysm boss structure. Objective: read.
- Each dungeon: Trigger = enter its structure. Objective = kill its boss.

| Quest | Structure | Boss |
|---|---|---|
| The Ancient Factory | `cataclysm:ancient_factory` | `the_harbinger` |
| The Cursed Pyramid | `cataclysm:cursed_pyramid` | `ancient_remnant` |
| The Frosted Prison | `cataclysm:frosted_prison` | `maledictus` |
| The Soul Forge | `cataclysm:soul_black_smith` | `netherite_monstrosity` |
| The Sunken City | `cataclysm:sunken_city` | `the_leviathan` |
| The Burning Arena | `cataclysm:burning_arena` | `ignis` |
| The Acropolips | `cataclysm:acropolis` | `scylla` |
| The Ruined Citadel | `cataclysm:ruined_citadel` | `ender_guardian` |
