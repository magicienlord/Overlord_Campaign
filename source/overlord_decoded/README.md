# Overlord canon scripts, decoded (for the writer)

Readable text of the Overlord I, Raising Hell and Overlord II script files in `source/overlord1` and `source/Overlord_2_Language` (decoded from `.8ld` with `tools/decode_8ld.py`). UI-only files (config, launcher, interface, credits, system) are left out.

**The Archivist wants the writer to lean heavily on these lines**: reuse canon catchphrases, echo canon lines, and rework a canon line whenever it fits the moment (see the writing rules in `Writer Docs/overlord-reigns-answers-log.md`).

## Files
- `gnarl_o1_lines.md`: every line the OI / Raising Hell scripts attribute to GNARL (911), grouped by script, each with its reference. **Start here for Gnarl's voice.**
- `minions_and_titles.md`: Minion speech, the Jester / Minstrel title announcements, Giblet at the Forge, canon Minion names and causes of death (for Quaver, Giblet the Sixth, Gristle, Blister, Grubbison Jr, Mortis).
- `o1/*.txt`, `o2/*.txt`: every script in full, one line per entry: `[scene.line] SPEAKER: text   <<trigger / dev note>>`.
- `overlord_all_lines.csv`: every line in one sheet (game, file, ref, speaker, text, trigger_or_notes), for searching and filtering.

## Speakers
- Overlord I / Raising Hell scripts name their speakers (GNARL, ROSE, VELVET, the FORGOTTEN GOD, etc.).
- **Overlord II scripts carry no speaker field**, so their lines are marked `(unattributed)`. Most O2 story lines are Gnarl (Prelude, NW_*, Wastelands, Nordberg_*, Everlight_*, Empire_*, End_Scene); read them in context. Nobody guessed speakers from wording.

## Citation codes used in `overlord-canon-bible.md`
`[FILE scene.line]` points into these files. Short codes: **MK** = `o1/D1_SD3_MelvinsKitchen` · **Boss** / **EXP Boss** = `o1/EXP_Endboss_Abyss` · **End** = `o1/End_Tower_Battle_Narrative` · **D1/D2/D3 (O1)** = `o1/D1_MAIN`, `o1/D2_MAIN`, `o1/D3_MAIN` · **NT4** = `o2/Nordberg_Town_Chunk_4` · **MT** = `o2/Minstrel_Titles` · **NW_TR** = `o2/NW_TR` · **Wastelands** = `o2/Wastelands` · **Nordberg_Sanctuary** = `o2/Nordberg_Sanctuary` · **SQ** = `o2/System_Quests`. Example: `[O1 D1_MAIN 412.10]` is line `[412.10]` in `o1/D1_MAIN.txt` (Gnarl on Evil energy).

## Fourth-wall rule
These are game scripts; they mention buttons, cameras and triggers in the `<<...>>` notes. Borrow the voice and lines, never the game mechanics wording.
