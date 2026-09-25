# Overlord Reigns: quest specs, part 4 (faction paths)

Rules (all factions): the 3 path quests trigger when that faction's intro (banner) is done. Completing Peaceful or Submission locks the other of the two; Destruction stays available afterwards (escalation, never the reverse). Each path quest's narrative is DEFINED here.

**Title changes:** "The Chosen Colony" becomes **"The Mound-Dwellers"** (no reference to choosing or the banner). "Break the Golden Order" becomes **"Break the Pig Pride"** (there's no Golden Order).

## Humans of Spree
- **The Full Larder (P)**: the Overlord becomes Spree's best customer and supplier until its granaries depend on the tower. Objective: trade with villagers 10 times (stat `minecraft:traded_with_villager`).
- **Overlord's Watch (S)**: Spree's guards now answer to him; its watchtowers fly his banner. Objective: advancement `guardvillagers:adventure/recruit_guard`.
- **Break the Civic Spine (D)**: kill the guards and the golem, and Spree learns the bedtime story was true. Objective: kill 5 `guardvillagers:guard` + 1 iron golem inside the village.

## Pillagers of the Bastille
- **An Armed Boundary (P)**: a border pact where the raiders keep their Bastille and raid only where he points. Objective: win a raid against another village while carrying the Bastille's banner (coder hook: raid won).
- **Bastille as a Weapon (S)**: they bow to force; their beasts become his. Objective: obtain `takesapillage:ravager_horn`.
- **What Bows After Fear (D)**: break the Bastille. Objective: kill 10 `takesapillage:legioner` / `skirmisher` / `archer` + a `takesapillage:clay_golem`.

## Dwarves of the Successor Hold (`dwarven_forge`, no advancements)
- **Two Claims (P)**: the Overlord backs the Dwarves' ancestral claim, in writing, in exchange for their forge. Objective: trade with a dwarf until you obtain `dwarven_forge:rune`.
- **The Weight of Continuity (S)**: the Hold "continues", but as his vassal forge. Objective: obtain `dwarven_forge:dwarven_metal_ingot` and wear a full dwarven armour set.
- **A Forge Owes Its Fire (D)**: he takes their fire for his own forge. Objective: kill 3 Dwarven Warriors and the Dwarven Forger (`dwarven_forge:dwarf`, by profession).

## Kobolds of the Den Below
- **Supply the Captain (P)**: he keeps the Den's Captain in supplies, so the salvage flows to the tower. Objective: trade with a Kobold (coder hook: any kobold trade).
- **Engineer the Den (S)**: the Den's engineers work for him now. Objective: obtain `kobolds:kobold_template`.
- **A Den Worth Razing (D)**: the salvagers get salvaged. Objective: kill the `kobolds:kobold_captain` + 10 Kobolds.

## An Old Conflict (Dwarves vs Kobolds, flavour only)
- **An Old Conflict**: Trigger: both The Successor Hold and The Den Below intros done. Objective: read (Gnarl lays out the tunnel feud: the Dwarves call it theft, the Kobolds call it salvage).
- 4 options; the first one done wins and closes the others:
  - **Weight the Scales** (Dwarf-favoured): kill 5 Kobolds.
  - **Arm the Den** (Kobold-favoured): kill 3 Dwarven Warriors.
  - **Make them Work** (peace): trade with both a dwarf and a kobold.
  - **Peace, What is it good for?** (war): kill 3 of each.

## Gnumus
- **Vintage Work Restored (P)**: he helps the Gnumus revive their lost "vintage" craft; their workshops now make his wares. Objective: advancement `gnumus:vintage_improvement`.
- **Vintage on Credit (S)**: he bankrolls them, and a debt never repaid is a leash. Objective: `gnumus:business_approach`.
- **End the Gnumus (D)**: gluttony meets the grave. Objective: kill 10 Gnumus including a `gnumus:gnumus_shaman`.

## Goblins (the Minion/Goblin "cousins" joke runs through all three)
- **Business Without Tribute (P)**: a trade deal where neither side pays tribute, and each cheats the other politely. Objective: `goblins_tyranny:merchant_success`.
- **Arms by Patronage (S)**: he becomes their patron; their engineers now arm his reign. Objective: `goblins_tyranny:engineer_success`.
- **Profit & Ruin (D)**: he takes the profit and leaves the ruin. Objective: `goblins_tyranny:goblins_slayer_success`.

## Ribbits
- **Prosperity in Ribbit (P)**: he funds their gardens; their harvest flows to his table. Objective: trade with a Ribbit (coder hook).
- **Quiet Village under Shadow (S)**: the village lives on, but its music plays only at his command. Objective: obtain `ribbits:maraca` (their instrument, given in tribute).
- **Silent Garden, At Last (D)**: no more croaking; Gnarl is delighted. Objective: kill 10 `ribbits:ribbit`.

## Sea People (Mermorphs, `seadwellers`)
- **Terms Below the Surface (P)**: an undersea trade treaty in aquamarine. Objective: `seadwellers:adv_barter_aquamarine`.
- **Depth Metal on Call (S)**: their Depth Metal forges now serve him. Objective: `seadwellers:adv_depth_ingot`.
- **Extinguish the Light (D)**: snuff out the last elven light. Objectives: `seadwellers:adv_break_sea_lantern` AND kill Mermorphs (count: 10, to confirm).

## Piglins
- **Gold without Theft (P)**: honest barter, which Gnarl finds shameful for different reasons. Objective: `minecraft:nether/distract_piglin`.
- **Who Owns the Gold (S)**: he takes their treasury, and they learn who owns it. Objective: `minecraft:nether/loot_bastion`.
- **Break the Pig Pride (D)**: the family shame is erased. Objective: kill 10 piglins + 2 piglin brutes in a Nether Village.

## The Grove (Umvuthi, Mowzie's Mobs)
- **Patron of the Grove (P)**: he trades offerings to Umvuthi and receives the Sun's Blessing: a god on retainer. Objective: `mowziesmobs:suns_blessing`.
- **A God Beneath a Master (S)**: he wears their masks, and the Umvuthana follow him instead of their god. Objective: obtain any `mowziesmobs:umvuthana_mask_*`.
- **Not a Phoenix (D)**: the sun-bird doesn't rise again. Objective: `mowziesmobs:kill_umvuthi`.

## The Mound-Dwellers (Myrmex, Ice and Fire)
- **A Hive Left its Own (P)**: he leaves the hive alone in exchange for its resin. Objective: obtain `iceandfire:myrmex_desert_resin` or `iceandfire:myrmex_jungle_resin`.
- **Command of the Resin (S)**: a staff that makes the colony obey. Objective: obtain `iceandfire:myrmex_desert_staff` or `iceandfire:myrmex_jungle_staff`.
- **Cut Off the Crown (D)**: kill the Queen and the hive dies. Objective: kill `iceandfire:myrmex_queen`.
