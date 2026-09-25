# Overlord Reigns: Ramblings (APPROVED)

Approved by the Archivist, mod group by mod group, all "as drafted". **338 Ramblings** (313 modded + 25 vanilla). Quaver 87 · Gnarl 76 · Gristle 51 · Giblet VI 41 · Mortis 22 · Collector 20 · Blister 15 · Lestat 14 · Grubbison Jr 12.

## Rules
- **What a Rambling is:** an advancement that no quest uses as a trigger or objective. When it fires: a TRIGGER POPUP (1–2 sentences, speaker portrait, emotion) + a fuller LOG ENTRY. No completion popup, no completion entry, no reward. Questlog chapter: Ramblings.
- **Selection:** a real feat or completion (boss kill, challenge, full collection, a notable evil act), or a mod the campaign leans on. Roots, auto-ticks and tutorial steps are dropped. Anything a quest uses is excluded (listed per mod below).
- **Speakers:** Giblet VI (forge, armory, weapons, armour sets) · Gristle (kitchen, food, farming) · Blister (alchemy, potions, plague) · Grubbison Jr (travel, digging, mining, exploration) · Quaver (music, and heralding TITLED FEATS: boss kills, no-hit kills, challenges, full collections) · Mortis (death, graves, undead) · Lestat (vampires, blood) · **the Collector, whose name is the Historian** (Fathoms, plus relics and antiquities) · Gnarl (everything else).
- **Writer template per Rambling:** SPEAKER · EMOTION · POPUP (trigger) · LOG ENTRY · CODER NOTES. The in-game advancement name is shown in brackets; the Rambling's own title comes in the Gnarl-jab title pass.
- **IDs:** modded IDs read from the pack's jars; vanilla IDs from the official 1.20.1 data (vanilla isn't in the jars). Full per-advancement descriptions: see each mod's in-game advancement screen.
- **Gnarl's Suspicions I–V** remain separate count-based Rambling-style entries (narrative beats doc).

## Speaker availability: held Ramblings (Archivist's ruling)
100 Ramblings belong to speakers who aren't present from the start. Each is HELD until its speaker appears:
- **Gristle (51) and Blister (15):** held until *Sit, Sire. Brood.* (Seat of the Overlord) is COMPLETED, when the room restorations wake them.
- **The Collector (20):** held until *That Is Not a Fish* (An Aberration on the Line) has UNLOCKED, his first appearance.
- **Lestat (14):** held until *Pale Suits You, Sire* (First Blood) has UNLOCKED, his first appearance. All 14 wait, including the vampire-hunting and garlic ones; a player who never turns vampire never sees them.
- **Release:** a Rambling whose advancement was earned before its speaker appeared fires on release as a **catch-up: log entry + toast only, no popup**. One earned after the speaker's arrival behaves normally (popup + log).
- CODER: implement as a Questlog prerequisite on the speaker's introduction quest; each affected Twine passage states its hold in CODER NOTES.
- Always available: Gnarl, Quaver, Giblet the Sixth, Grubbison Jr (Browns) and Mortis.

## Coder notes
- A Rambling can fire in the same tick as a quest trigger (e.g. `graveyard:graveyard/haunted_house` if it's the first Graveyard structure entered). Queue the Rambling popup AFTER the quest popup.
- Advancements whose JSON trigger is `impossible` (Born in Chaos, Gnumus, Goblins, Fathoms, Bosses'Rise no-hit, Sea Dwellers…) are granted by the mod's own code; Questlog still sees them.
- Hidden advancements stay hidden in the vanilla screen; the popup is the player's first sight of them.

## Tower mods

### biomancy (16)
- **Gnarl:** `biomancy:biomancy/bio_forge` (Organic Smithing), `biomancy:biomancy/malignant_growth` (Malignant Growth), `biomancy:biomancy/nether_star_sacrifice` (Superior Sacrifice), `biomancy:biomancy/organ_trader` (Organ Trader), `biomancy:biomancy/primal_orifice` (Trypophobia?)
- **Quaver:** `biomancy:biomancy/cat_killer` (Kitty Cat Killer), `biomancy:biomancy/poacher` (Rare Animal Poacher), `biomancy:biomancy/predator_killer` (Predator Killer)
- **Giblet VI:** `biomancy:biomancy/greedy_butcher` (Greedy Butcher)
- **Gristle:** `biomancy:biomancy/cooked_meat_sacrifice` (Cooked Meat Disrelish), `biomancy:biomancy/digester` (Yummy Paste), `biomancy:biomancy/raw_meat_collection` (Collector of Raw Meats)
- **Blister:** `biomancy:biomancy/bio_lab` (Is this still Alchemy?), `biomancy:biomancy/exotic_compounds` (Exotic Bio-Alchemy), `biomancy:biomancy/genetic_compounds` (Genetic Bio-Alchemy), `biomancy:biomancy/organic_compounds` (Organic Bio-Alchemy)
- *Excluded (quest):* `biomancy/bio_injector`, `biomancy/cradle`, `biomancy/craft_primal_core`, `biomancy/decomposer`, `biomancy/living_flesh`, `biomancy/primal_vision`

### eidolon (12)
- **Gnarl:** `eidolon:cure_zombie` (Curse Lifted), `eidolon:frost_spell` (Call of Winter), `eidolon:lay_on_hands` (Healing Touch), `eidolon:sacred_path` (The Sacred Path), `eidolon:sacrifice` (Blood for the Dark One), `eidolon:smite_undead` (The light's Fury), `eidolon:villager_sacrifice` (A Greater Sacrifice), `eidolon:wicked_path` (The Wicked Path)
- **Blister:** `eidolon:crucible` (Alchemical Soup)
- **Mortis:** `eidolon:enthrall_undead` (A New Servant), `eidolon:reaper_scythe` (Reaping Time), `eidolon:zombify` (A New Recruit for the Dark)
- *Excluded (quest):* `flame_spell`, `holy_symbol`, `incense`, `soul_shard`, `unholy_symbol`, `worktable`

### irons_spellbooks (13)
- **Gnarl:** `irons_spellbooks:irons_spellbooks/enter_catacombs` (Dungeon Delving), `irons_spellbooks:irons_spellbooks/ink_legendary` (Premium!), `irons_spellbooks:irons_spellbooks/make_wayward_compass` (And so a Quest Begins!), `irons_spellbooks:irons_spellbooks/spell_book_dead_king` (Necronomicon), `irons_spellbooks:irons_spellbooks/spell_book_dragon` (Elder Power), `irons_spellbooks:irons_spellbooks/spell_book_evoker` (Grimoire of Evokation), `irons_spellbooks:irons_spellbooks/spell_book_villager` (Enlightenment), `irons_spellbooks:irons_spellbooks/steal_from_wizard` (A Fool's Folly)
- **Giblet VI:** `irons_spellbooks:irons_spellbooks/staff_pyrium` (Ancient Beckonings)
- **Mortis:** `irons_spellbooks:irons_spellbooks/spell_book_rotten` (How long's this been here?)
- **Lestat:** `irons_spellbooks:irons_spellbooks/spell_book_blood` (A piece of Yourself), `irons_spellbooks:irons_spellbooks/staff_blood_staff` (Staff of Blood)
- **Collector:** `irons_spellbooks:irons_spellbooks/spell_book_netherite` (Ancient Knowledge)
- *Excluded (quest):* `irons_spellbooks/make_arcane_anvil`, `irons_spellbooks/make_inscription_table`, `irons_spellbooks/make_scroll_forge`, `make_inscription_table`

### farmersdelight (7)
- **Gnarl:** `farmersdelight:main/hit_raider_with_rotten_tomato` (Boo! Hiss!)
- **Giblet VI:** `farmersdelight:main/obtain_netherite_knife` (If You Can't Take the Heat...)
- **Gristle:** `farmersdelight:main/eat_nourishing_food` (Nourishing!), `farmersdelight:main/get_ham` (Wild Butcher), `farmersdelight:main/get_mushroom_colony` (Fungus Among Us), `farmersdelight:main/master_chef` (Master Chef), `farmersdelight:main/plant_all_crops` (Crop Rotation)
- *Excluded (quest):* `main/get_rich_soil`, `main/place_cooking_pot`, `main/place_feast`

### farmers_spell (5)
- **Gristle:** `farmers_spell:alchemist_pot` (Brimming with Mana), `farmers_spell:blood_tofu` (Coagulated Blood...), `farmers_spell:catacombs_wine` (Vintage Bloodline), `farmers_spell:chef_ratatouille` (Chef Ratatouille), `farmers_spell:icebreaker_bread` (Titantic Bread)
- *Excluded:* `food_shaman` (same name as the quest Food Shaman)

### dungeonsdelight (12)
- **Quaver:** `dungeonsdelight:main/all_knife_mob_drops` (Gastrocryptozoologist), `dungeonsdelight:main/all_monster_effects` (Monsters Smashed), `dungeonsdelight:main/eat_horse` (How Hungry...?), `dungeonsdelight:main/use_gunk_arrow_on_monster_yam` (Septic Tank)
- **Giblet VI:** `dungeonsdelight:main/get_netherite_cleaver` (Cutlery of Apostasy), `dungeonsdelight:main/get_stained_scrap` (Heavy Metal), `dungeonsdelight:main/get_stained_weapon` (A Slice of Life)
- **Gristle:** `dungeonsdelight:main/all_dungeonsdelight_foods` (Meal of Champions), `dungeonsdelight:main/all_monster_foods` (The Privilege of The Living), `dungeonsdelight:main/eat_bloody_mary` (Bloody Mary Challenge), `dungeonsdelight:main/eat_monster_food` (Ah, Dungeon Food), `dungeonsdelight:main/place_monster_pot` (Delicious in a Dungeon)

### display_case (2)
- **Giblet VI:** `display_case:collapse` (The collapse), `display_case:infinity_case` (To infinity and beyond)
- *Excluded (quest):* `display_item`

## Main plot

### block_factorys_bosses (7)
- **Gnarl:** `block_factorys_bosses:no_hit_underworld_knight` (Beyond Death)
- **Quaver:** `block_factorys_bosses:kill_boss_under_minute` (Overclocker), `block_factorys_bosses:no_hit_dragon` (Dragon Hunter), `block_factorys_bosses:no_hit_kraken` (Wraith of the Tide), `block_factorys_bosses:no_hit_sandworm` (Desert Power), `block_factorys_bosses:no_hit_yeti` (King of the Hill)
- **Mortis:** `block_factorys_bosses:die_boss` (Bosses' Rise)
- *Excluded (quest):* `kill_all_bosses` (= all 5 gates done, A Single Wound's trigger), `kill_dragon`, `kill_kraken`, `kill_sandworm`, `kill_underworld_knight`, `kill_yeti`

### cataclysm (4)
- **Gnarl:** `cataclysm:kill_clawdian` (Not so Shrimple Now), `cataclysm:kill_ender_golem` (Palette Swap), `cataclysm:kill_revenant` (Imperfect thing)
- **Quaver:** `cataclysm:kill_all_bosses` (The Cataclysmfarer)
- *Excluded (quest):* all 8 `find_*` and the 8 dungeon boss kills (`kill_ender_guardian`, `kill_harbinger`, `kill_ignis`, `kill_leviathan`, `kill_maledictus`, `kill_monstrosity`, `kill_remnant`, `kill_scylla`)

## Side stories

### graveyard (11)
- **Gnarl:** `graveyard:graveyard/corruption` (Source of Evil), `graveyard:graveyard/giant_mushroom` (Corrupting the Paradise), `graveyard:graveyard/haunted_house` (Invitation to the Tea Party)
- **Quaver:** `graveyard:graveyard/kill_while_blinded` (Peekaboo, I (still) see you!)
- **Giblet VI:** `graveyard:graveyard/dark_iron` (Iron, but dark)
- **Mortis:** `graveyard:graveyard/dead_tree` (Hanging Tree), `graveyard:graveyard/equip_ghouling_coffin` (The dead shall serve), `graveyard:graveyard/kill_acolyte_bone_dagger` (Turning the tables), `graveyard:graveyard/kill_horde` (Walking Dead), `graveyard:graveyard/kill_wraith` (Taking from the Dead)
- **Lestat:** `graveyard:graveyard/vial_of_blood` (Blood "Donation")
- *Excluded (quest):* every `*_bone_staff` (black, cyan, purple, red, white, lower, middle, upper), `lich_prison`, `summon_lich`, `root`, `crypt`, `desert_graveyard`, `medium_graveyard`, `large_graveyard`, `kill_graveyard_mob`

### the_bumblezone (37)
- **Gnarl:** `the_bumblezone:beehemoth/queen_beehemoth` (Regal Friends Till The Very End!), `the_bumblezone:beehemoth/tamed_beehemoth` (Bee Movie But It's 300% Larger), `the_bumblezone:effects/bee_hit_wrath_of_the_hive` (NOT THE BEEEEEES!!!), `the_bumblezone:essence/bee_essence_infusion` (Hope, Love, Dreams, and BEES!!!), `the_bumblezone:structures/enter_sempiternal_sanctum` (Ancient Origins), `the_bumblezone:the_queens_desire/the_beginning` (The Queen's Desire)
- **Quaver:** `the_bumblezone:essence/essence_calming` (Peace and Love), `the_bumblezone:essence/essence_continuity` (Reality Glitch), `the_bumblezone:essence/essence_knowing` (The All-Seeing), `the_bumblezone:essence/essence_life` (Blessings of Life), `the_bumblezone:essence/essence_radiance` (Solar Powered), `the_bumblezone:essence/essence_raging` (Unstoppable Anger), `the_bumblezone:music_discs/obtain_all_music_discs` (Gotta Hive a Dance!), `the_bumblezone:stinger_spear/stinger_spear_paralyze_boss` (Getting Favorable Odds), `the_bumblezone:the_queens_desire/back_in_action` (Back in Action), `the_bumblezone:the_queens_desire/crazy_trader` (Crazy Trader), `the_bumblezone:the_queens_desire/fighting_the_swarm` (Fighting the Swarm), `the_bumblezone:the_queens_desire/flooding_the_housing_market` (Flooding the Housing Market), `the_bumblezone:the_queens_desire/love_bees` (Love bees), `the_bumblezone:the_queens_desire/otherworldly_mites` (Otherworldly Mites), `the_bumblezone:the_queens_desire/peak_inefficiency` (Peak Inefficiency), `the_bumblezone:the_queens_desire/poison_warfare` (Poison Warfare), `the_bumblezone:the_queens_desire/pollen_fight` (Pollen Fight), `the_bumblezone:the_queens_desire/terror_fangs` (Terror Fangs), `the_bumblezone:the_queens_desire/the_crazy_florist` (The Crazy Florist), `the_bumblezone:the_queens_desire/the_great_dragon_slayer` (The Great Dragon Slayer), `the_bumblezone:the_queens_desire/too_many_legs` (Too Many Legs)
- **Giblet VI:** `the_bumblezone:armor/warrior_bee` (The Bee Warrior Rises!), `the_bumblezone:honey_crystal_shield/obtain_maxed_honey_crystal_shield` (Grand Hive Defender)
- **Gristle:** `the_bumblezone:honey_bucket/drink_royal_jelly_bottle` (Gaining Royal Powers), `the_bumblezone:honey_bucket/obtain_royal_jelly_bucket` (Masterful Collector), `the_bumblezone:the_queens_desire/honey_drunk` (Honey Drunk), `the_bumblezone:the_queens_desire/hungry_hungry_bees` (Hungry Hungry Bees), `the_bumblezone:the_queens_desire/slimy_mitosis` (Slimy Mitosis), `the_bumblezone:tools/fish_rare_loot` (Beesistent Fishing)
- **Grubbison Jr:** `the_bumblezone:biomes/discover_all_biomes` (Beeography), `the_bumblezone:structures/enter_all_structures` (Sightbee-er)
- *Excluded (quest):* `teleportation/teleport_to_bumblezone_pearl`, `teleportation/teleport_to_bumblezone_piston` (A Hive Without End), `the_queens_desire/journeys_end` (hands over the Essence = Essence of the Hive)

### rats (22)
- **Gnarl:** `rats:ball_of_filth` (Cleanliness is Close to Godliness!), `rats:rat_crafting_table` (Rat Auto-Crafting), `rats:rat_upgrade_demon` (I Seen This Before...), `rats:rat_upgrade_flight` (Essentially Pigeons), `rats:rat_upgrade_god` (Whats a Man to a King?), `rats:rat_upgrade_idol` (False Prophet), `rats:rat_upgrade_pickpocket` (Talk of the Town)
- **Quaver:** `rats:all_hats` (Grand Hat Collector), `rats:defeat_black_death` (Do Not Go Quietly Into the Night), `rats:defeat_rat_king` (King of the World!), `rats:piper` (Pay the Piper), `rats:rat_music_disc` (Rat Tunes)
- **Giblet VI:** `rats:rat_upgrade_warrior` (Rat Warrior Clan)
- **Gristle:** `rats:contaminated_food` (Stop that Health Inspector!), `rats:nether_cheese` (Spicy Pepper Jack), `rats:rat_cooking` (Anyone Can Cook), `rats:rat_upgrade_chef` (The Rat is the Cook!)
- **Blister:** `rats:plague` (Down with the Sickness!), `rats:plague_cure` (The Medieval Treatment), `rats:plague_doctor` (I AM THE CURE!)
- **Mortis:** `rats:black_death` (Dance Macabre!), `rats:rat_upgrade_sculked` (One with the Souls)
- *Excluded (quest):* `cheese`, `tame_rat`

### nycto (10)
- **Lestat:** `nycto:nycto/brew_garlic_brew` (Holy Water), `nycto:nycto/buy_hunter_contract` (Contract Killer), `nycto:nycto/complete_vampire` (Taste of Eternity), `nycto:nycto/kill_vampire` (Not So Immortal), `nycto:nycto/kill_vampire_with_wooden_stake` (Shot Through The Heart), `nycto:nycto/obtain_garlic_coated_halberd` (Seasoned Warrior), `nycto:nycto/obtain_garlic_wreath` (It's Called Aura), `nycto:nycto/sleep_in_coffin` (Rest in Peace), `nycto:nycto/use_garlic_brew_on_vampire` (Night of the Living), `nycto:nycto/wear_vampire_hunter_armor` (Van Helsing)
- *Excluded (quest):* `nycto/become_vampire`, `nycto/extract_blood_bottle`, `nycto/obtain_vampire_power`

### fathoms (18)
- **Giblet VI:** `fathoms:nautical/upgrade_ornate_tool` (Former Glory)
- **Collector:** `fathoms:nautical/activate_conduit` (Moskstraumen), `fathoms:nautical/all_max_level_rituals` (Gargantua's Devout), `fathoms:nautical/apply_jinx` (The Monkey's Paw), `fathoms:nautical/calcify_augur` (Rapid Calcification), `fathoms:nautical/catch_all_fish` (Ol' Mariner), `fathoms:nautical/create_kelpie` (Transmogrification), `fathoms:nautical/dredging_apparatus` (Dredge the Depths), `fathoms:nautical/enter_ancient_reservoir` (Buried Alive), `fathoms:nautical/full_tell_tale_heart_trim_material` (Oilman), `fathoms:nautical/make_a_bad_decision` (Heart of Oil), `fathoms:nautical/obtain_nautilus_shell` (Extinct Enigma), `fathoms:nautical/obtain_pylon` (Bomb Squad), `fathoms:nautical/obtain_turtle_shell` (Turtle Power), `fathoms:nautical/open_coffer` (You Are a Pirate), `fathoms:nautical/perform_enhanced_ritual` (Return to Nature), `fathoms:nautical/thaw_wishing_well` (Frozen in Time), `fathoms:nautical/whiplash_lightning` (System Overload)
- *Excluded (quest):* `nautical/catch_aberration`, `nautical/cut_aberration`, `nautical/enter_rocky_waters`, `nautical/obtain_all_sunken_scrawls`, `nautical/open_message_in_a_bottle`, `nautical/perform_ritual`

### iceandfire (18)
- **Gnarl:** `iceandfire:iceandfire/dragon_staff` (Dragon Commander), `iceandfire:iceandfire/tame_amphithere` (Jungle Fliers), `iceandfire:iceandfire/tame_cockatrice` (Stay Out of my Peripheral!), `iceandfire:iceandfire/tame_hippogryph` (Buck Beak)
- **Quaver:** `iceandfire:iceandfire/gorgon_head` (Clash of the Titans), `iceandfire:iceandfire/kill_cyclops` (My Name is Nobody), `iceandfire:iceandfire/kill_deathworm` (The Desert Swimmers), `iceandfire:iceandfire/kill_ghost` (Who You Gonna Call?), `iceandfire:iceandfire/kill_hydra` (The Twelve Labors of Hercules), `iceandfire:iceandfire/kill_if_dragon` (Dragonslayer), `iceandfire:iceandfire/kill_sea_serpent` (Sea? Not a Problem), `iceandfire:iceandfire/kill_siren` (Tie me to the Mast), `iceandfire:iceandfire/kill_stymphalian_bird` (Herc was on a Roll!)
- **Giblet VI:** `iceandfire:iceandfire/dragonarmor` (Suit Up), `iceandfire:iceandfire/dragonbone_flaming_sword` (A Flaming Sword), `iceandfire:iceandfire/dragonsteel_weapon` (Draconic Evolution), `iceandfire:iceandfire/pixie_wand` (Where Is My Mind?)
- **Gristle:** `iceandfire:iceandfire/dragon_meal` (Dragon Growth Hormone)
- *Excluded (quest):* `iceandfire/bestiary`, `iceandfire/dragon_egg`, `iceandfire/dragon_forge_core`, `iceandfire/dragonsteel`, `iceandfire/myrmex_resin`

### twilightforest (20)
- **Gnarl:** `twilightforest:arborist` (Maniacal Dendrologist), `twilightforest:beanstalk` (Jack and the Beanstalk), `twilightforest:ghast_trap` (Something Strange in Towerwood), `twilightforest:quest_ram` (Consummate Baaahs), `twilightforest:uncraft_uncrafting_table` (A Step too Far)
- **Quaver:** `twilightforest:giants` (I'm on Cloud Nine), `twilightforest:lich_scepters` (By Our Powers Combined!), `twilightforest:progress_merge` (Ultimate Showdown), `twilightforest:progress_trophy_pedestal` (Trophied Champion)
- **Giblet VI:** `twilightforest:break_glass_sword` (One Hit Wonder), `twilightforest:fiery_set` (Gallons of Blood and Tears), `twilightforest:naga_armors` (Naga Armorer)
- **Gristle:** `twilightforest:experiment_115` (Mystery Meat?), `twilightforest:experiment_115_115` (Eating 115 Everyday, 115 Years, Forever), `twilightforest:experiment_115_self_replenishing` (Making a note: Huge Success!), `twilightforest:hydra_chop` (Hydra Chop, Baby!), `twilightforest:twilight_dinner` (We Dine At Eternal Sundown)
- **Blister:** `twilightforest:full_mettle_alchemist` (Full Mettle Alchemist)
- **Grubbison Jr:** `twilightforest:mazebreaker` (Breaking the Maze), `twilightforest:ore_map` (How Can That Be Worth It?)
- *Excluded (quest):* the 9 `progress_*` (naga, lich, labyrinth, hydra, knights, ur_ghast, yeti, glacier, troll), `root`

## Factions

### gnumus (8)
- **Gnarl:** `gnumus:weight_loss_protection` (Weight Loss Protection), `gnumus:worthy_traders_hat` (Worthy Trader's Hat)
- **Quaver:** `gnumus:plan_boar` (Plan "Boar"), `gnumus:sack_collector` (Pouch Collector)
- **Giblet VI:** `gnumus:vintage_rifleman` (Vintage Rifleman), `gnumus:vintage_technology` (Vintage Technology), `gnumus:wellfed_warrior` (Well-fed Warrior)
- **Gristle:** `gnumus:hearty_dish` (Hearty Dish)
- *Excluded (quest):* `business_approach`, `fatty_demon`, `vintage_improvement`

### goblins_tyranny (12)
- **Gnarl:** `goblins_tyranny:barrel_success` (Kinda Sus), `goblins_tyranny:droblin_success` (Best Slave Forever), `goblins_tyranny:glitteron_success` (A Bug's Life), `goblins_tyranny:goblins_disguise_success` (Hiding Among Fools), `goblins_tyranny:wake_up_success` (Do Not Disturb)
- **Giblet VI:** `goblins_tyranny:prototype_success` (This is Mine Now), `goblins_tyranny:skybound_success` (To the Sky), `goblins_tyranny:upgrade_success` (Upgrades, People. Upgrades.)
- **Gristle:** `goblins_tyranny:blazing_liquor_success` (This is Fine !), `goblins_tyranny:deadly_liquor_success` (I Don't Feel so Good...), `goblins_tyranny:goblins_meat_success` (Goblin Eater), `goblins_tyranny:mushroom_success` (Seeing a Rainbow Road ?)
- *Excluded (quest):* `engineer_success`, `goblins_encounter_success`, `goblins_slayer_success`, `merchant_success`

### seadwellers (1)
- **Gnarl:** `seadwellers:adv_turn_villager_into_mermorph` (Reverse Evolution)
- *Excluded (quest):* `adv_barter_aquamarine`, `adv_break_sea_lantern`, `adv_depth_ingot`

### mowziesmobs (9)
- **Gnarl:** `mowziesmobs:sneak_grove` (Birds of a Feather), `mowziesmobs:steal_ice_crystal` (Big Brain™ Time)
- **Quaver:** `mowziesmobs:kill_ferrous_wroughtnaut` (Just a Flesh Wound), `mowziesmobs:kill_frostmaw` (Rude Awakening), `mowziesmobs:kill_naga` (Wingin' It), `mowziesmobs:sculptor_challenge` (You Must Believe)
- **Grubbison Jr:** `mowziesmobs:kill_grottol_fortune` (Double Or Nothing!), `mowziesmobs:kill_grottol_silk_touch` (You're Coming With Me)
- **Mortis:** `mowziesmobs:sculptor_failure` (No One Jumps for the Beef)
- *Excluded (quest):* `kill_umvuthi`, `suns_blessing`

## Other mods (feats only)

### artifacts (3)
- **Quaver:** `artifacts:chest_slayer` (Chest Slayer)
- **Gristle:** `artifacts:adventurous_eater` (Adventurous Eater)
- **Collector:** `artifacts:amateur_archaeologist` (Amateur Archaeologist)

### betterdungeons (1)
- **Grubbison Jr:** `betterdungeons:all_dungeons` (Professional Dungeoneer)

### born_in_chaos_v1 (36)
- **Gnarl:** `born_in_chaos_v1:naughty_child` (Naughty Child), `born_in_chaos_v1:trickor_treat` (Trick or Treat)
- **Quaver:** `born_in_chaos_v1:arachnophobes_nightmare` (Arachnophobe's Nightmare), `born_in_chaos_v1:big_boy` (Big Boy), `born_in_chaos_v1:charm_collector` (Charm Collector), `born_in_chaos_v1:dark_creator` (Dark Creator), `born_in_chaos_v1:dismantledto_bones` (Senior Summoner), `born_in_chaos_v1:excessive_fly_swatter` (Excessive Fly Swatter), `born_in_chaos_v1:exorcism` (Exorcism), `born_in_chaos_v1:fighting_nightmares` (Fighting Nightmares), `born_in_chaos_v1:hatman` (Hatman), `born_in_chaos_v1:horror_underthe_mantle` (Horror Under the Mantle), `born_in_chaos_v1:horrorofthe_depths` (Horror of the Depths), `born_in_chaos_v1:pumpkin_lord` (Last Night), `born_in_chaos_v1:pumpkin_sir` (Pumpkin Sir), `born_in_chaos_v1:rampage` (RAMPAGE!), `born_in_chaos_v1:spruce_cowboyinthe_moonlight` (Spruce Cowboy In The Moonlight), `born_in_chaos_v1:symphonyof_chaos` (Symphony of Chaos), `born_in_chaos_v1:wrong_santa` (Wrong Santa)
- **Giblet VI:** `born_in_chaos_v1:chaos_knight` (Chaos Knight), `born_in_chaos_v1:dark_blacksmith` (Dark Blacksmith), `born_in_chaos_v1:my_size` (My Size!), `born_in_chaos_v1:protectedby_darkness` (Protected by Darkness), `born_in_chaos_v1:shell_warrior` (Shell Warrior), `born_in_chaos_v1:spider_warlord` (Spider Warlord), `born_in_chaos_v1:squireofthe_dark_lord` (Squire of the Dark Lord), `born_in_chaos_v1:unitywith_darknessachievement` (Unity with Darkness)
- **Gristle:** `born_in_chaos_v1:yoursatietywillbe_eternal` (Your satiety will be Eternal!)
- **Blister:** `born_in_chaos_v1:infernal_medicine` (Infernal Medicine), `born_in_chaos_v1:transmutalogy` (Transmutalogy)
- **Mortis:** `born_in_chaos_v1:bury_them_all` (Bury Them All), `born_in_chaos_v1:compact_necromancy` (Compact Necromancy), `born_in_chaos_v1:grave_ravager` (Grave Ravager), `born_in_chaos_v1:guidetothenextworld` (The day of the Dead), `born_in_chaos_v1:soul_eater` (Soul Eater)
- **Lestat:** `born_in_chaos_v1:heart_thief` (Heart Thief)

### conjurer_illager (1)
- **Quaver:** `conjurer_illager:kill_conjurer` (What a Performance!)

### darkerdepths (3)
- **Mortis:** `darkerdepths:activities/bottle_void_soul` (Bottle O'Void Souls), `darkerdepths:activities/insert_diamond_into_crystal_husk` (Back From the Dead!), `darkerdepths:activities/set_death_anchor` (Soul Pact)

### ice_and_fire_delight (5)
- **Quaver:** `ice_and_fire_delight:kill_pixie` (You are a monster!)
- **Gristle:** `ice_and_fire_delight:dragon_minced_meat_adv` (Not so great beast), `ice_and_fire_delight:power_of_three_dragons_adv` (The Power of Three Dragons), `ice_and_fire_delight:rip_dragon_adv` (Rest in peace Dragon), `ice_and_fire_delight:too_much_power` (Too Much Power)

### netherdepthsupgrade (2)
- **Gristle:** `netherdepthsupgrade:main/abyssal_flora_expert` (Abyssal Flora Expert), `netherdepthsupgrade:main/lava_fishing_master` (Lava Fishing Master)

### rottencreatures (3)
- **Quaver:** `rottencreatures:he_is_a_pirate` (He's a Pirate!), `rottencreatures:kill_all_rot` (Purification!), `rottencreatures:shocking_encounter` (High Tension)

### savage_and_ravage (3)
- **Gnarl:** `savage_and_ravage:adventure/mask_of_dishonesty` (A Little Tricking)
- **Giblet VI:** `savage_and_ravage:adventure/griefer_armor` (Dynamite with a Laser Beam)
- **Collector:** `savage_and_ravage:adventure/relic_collector` (Relic Collector)

### shieldexp (1)
- **Giblet VI:** `shieldexp:get_netherite_shield` (Immovable Object)

### supplementaries (3)
- **Gnarl:** `supplementaries:story/unenchanter` (Why Would You do That!?)
- **Gristle:** `supplementaries:husbandry/soap` (Tide Pod Challenge)
- **Blister:** `supplementaries:nether/goblet` (Consume the Concoction Chalice)

### tameablebeasts (8)
- **Gnarl:** `tameablebeasts:big_iron_hoe` (It's Not For Gardening), `tameablebeasts:grapteranodon` (Hey Just Like In Ark), `tameablebeasts:ice_armor` (Bring Me A Warden!), `tameablebeasts:quetzalcoatlus` (Is That A Cloud?)
- **Giblet VI:** `tameablebeasts:beetle_armor` (Giving Netherite A Run For Its Money), `tameablebeasts:beetle_elytra` (Why Not Have Both?), `tameablebeasts:metal_beetle` (Chrome Beetle)
- **Grubbison Jr:** `tameablebeasts:quetzal_stand` (Public Transport)

### Mods with no Ramblings
- `hot_iron` (local_smithery = the Fire & Iron room), `outer_end` (both used by Far Edge of the Reign), `knightquest` (essence line), `pet_cemetery` (all three used), `takesapillage` (bastille = intro; pillager_camp dropped). `guardvillagers`' `minecraft:adventure/recruit_guard` = Overlord's Watch (S).

## Vanilla (Minecraft 1.20.1) (25)
- **Gnarl:** `minecraft:adventure/hero_of_the_village` (Hero of the Village), `minecraft:adventure/voluntary_exile` (Voluntary Exile), `minecraft:end/respawn_dragon` (The End... Again...), `minecraft:nether/create_full_beacon` (Beaconator), `minecraft:nether/summon_wither` (Withering Heights), `minecraft:nether/uneasy_alliance` (Uneasy Alliance), `minecraft:story/cure_zombie_villager` (Zombie Doctor)
- **Quaver:** `minecraft:adventure/arbalistic` (Arbalistic), `minecraft:adventure/kill_all_mobs` (Monsters Hunted), `minecraft:adventure/sniper_duel` (Sniper Duel), `minecraft:adventure/two_birds_one_arrow` (Two Birds, One Arrow), `minecraft:nether/return_to_sender` (Return to Sender)
- **Giblet VI:** `minecraft:adventure/trim_with_all_exclusive_armor_patterns` (Smithing with Style), `minecraft:nether/netherite_armor` (Cover Me in Debris)
- **Gristle:** `minecraft:husbandry/balanced_diet` (A Balanced Diet), `minecraft:husbandry/bred_all_animals` (Two by Two), `minecraft:husbandry/obtain_netherite_hoe` (Serious Dedication)
- **Blister:** `minecraft:end/dragon_breath` (You Need a Mint), `minecraft:nether/all_effects` (How Did We Get Here?), `minecraft:nether/all_potions` (A Furious Cocktail)
- **Grubbison Jr:** `minecraft:adventure/adventuring_time` (Adventuring Time), `minecraft:end/elytra` (Sky's the Limit), `minecraft:nether/explore_nether` (Hot Tourist Destinations), `minecraft:nether/fast_travel` (Subspace Bubble)
- **Mortis:** `minecraft:adventure/totem_of_undying` (Postmortal)
- *Excluded (quest):* `minecraft:end/dragon_egg` (A Seed of the Heart); `minecraft:nether/obtain_blaze_rod` (Restore the Reds); `minecraft:end/kill_dragon` (Sever the Anchor); `minecraft:story/enter_the_end` (The Wound Beyond the World); `minecraft:end/enter_end_gateway` (Return to the Wasteland); `minecraft:end/find_end_city` (Cities at the Edge); `minecraft:nether/distract_piglin` (Gold without Theft); `minecraft:nether/loot_bastion` (Who Owns the Gold)
