# Extraction and attribution notes

Source assets: user-supplied UnityFS bundle and Addressables `catalog.json`. The UnityFS LZ4 chunks decompress to a Unity serialized asset containing an English `Yarn_en` string table. The `Yarn_en` array has 2,607 entries, all with distinct 64-bit string IDs and valid UTF-8. Each entry in this table was extracted; no dialogue line was dropped for lacking a label.

Explicit `*_NAME_KEY:` labels: 1363. Untagged entries: 1244. Collector-tagged entries: 113 (107 Collector, 6 unknown-identity variants).

The same bundle also contains a separate `Strings_en` localization table of UI and other English text. It is not counted as Yarn dialogue. This extraction covers all `Yarn_en` entries from the **provided** bundle, not a promise to cover every update, DLC bundle, cutscene voiceover, journal entry, or text baked into other assets.

**Attribution rules:** Explicit source label = confirmed attribution as labelled by localization. Narrator, player choice/action, and system/editor categories are text-based inferences for unlabeled lines. Otherwise `Unattributed`; it is preferable to inventing a speaker. The `COLLECTOR_UNKNOWN_DOCK_NAME_KEY` / `COLLECTOR_UNKNOWN_HOUSE_NAME_KEY` strings are grouped separately from the regular Collector within the master character file; both are present in Collector-only file. Game runtime branching and exact conversational sequence cannot be recovered from this localization bundle and catalog alone.

**Counts by group:**

- Collector: 107
- Collector (unidentified in scene): 6
- Player: 5
- Narrator / scene text: 401
- Unattributed: 405
- Player (choice): 273
- Player (action choice): 158
- Travelling Merchant: 135
- Scientist: 96
- Foreman: 93
- Researcher: 84
- Soldier: 72
- Mayor: 63
- Fishmonger: 61
- Retired Whaler: 45
- Lighthouse Keeper: 43
- Engineer: 40
- Hermit: 40
- Photographer: 40
- Fanatic: 38
- Painter: 38
- Shipwright: 31
- Ingfell Resident: 27
- Dockworker: 26
- Builder: 24
- Executive: 22
- Trader: 22
- Founder: 19
- Grieving Father: 18
- Captain's Log: 17
- Dog: 16
- Courier: 15
- Old Mayor: 15
- Castaway: 13
- Leather Journal: 13
- Soul (Middle): 12
- Soul (South): 11
- Tattered Diary: 11
- Soul (East): 8
- Soul (West): 8
- System / editor: 7
- Founder (Undermarket): 6
- Hooded Figure 1: 5
- Hooded Figure 2: 5
- Hooded Figure 3: 5
- Hooded Figure 4: 4
- Hooded Figure 5: 4

**Source SHA-256:** `59241b655fe6fe76209b8de6413a57609ce0328dedac2a7a0695ec032cface14`.
