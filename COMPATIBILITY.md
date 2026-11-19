# Pyriell bugfix compatibility audit for Rebalanced v1.2

Audited v1.2 BIN: `6202e1b7ace94d75f2cce162e5391bbf8ccc6720c484fe98df3b6984904cfabc`

Source: [Pyriell gs2-bugfixes 2.02.078](https://github.com/pyriell/gs2-bugfixes/blob/e657ecafebdad2ed4c8e9031a8ab982fd506bf58/patcher.lua), revision `e657ecafebdad2ed4c8e9031a8ab982fd506bf58`. Local repository was clean and `git ls-remote origin HEAD` matched that revision.

This is a byte-level and private in-memory per-file composition audit. No upstream fixes were applied to our image, no combined ISO was built, and no combined-image gameplay is certified.

## Result

- All 1,285 Rebalanced manifest spans survive the actual default PPF selection followed by Godspeed, Minotaur and Circlet text passes in the installer order
- The NA release contains 36 PPF files and 34 selectable options, of which 32 are selected by default. PPF40 is the custom format name, not a count of 40 patches
- Default Kindness Penalty writes four bytes already identical in Rebalanced. No other default PPF overlaps any Rebalanced guarded span
- Across both mutually exclusive Kindness alternatives, seven per-patch overlap bytes comprise six equal values and one different value. There are only four distinct overlapped addresses; these alternative counts must not be mistaken for a single default combination
- No Penalty overlaps three Rebalanced bytes: two equal, one different at SLUS file offset `0x1E177` (`02` becomes `00`). It intentionally overrides the retained negative-Kindness penalty rather than silently preserving our balance choice
- The other 34 PPF files have zero overlap with Rebalanced spans, including the five Clive branches
- All 1,090 hardcoded FileList paths exist and exactly match the original and Rebalanced ISO inventories. File locations, sizes and directory layout are unchanged before running the upstream tool
- All 17 LBA-table writes span 8,720 bytes each (1,090 entries). Their original and current bytes match, their first words pass the upstream sanity condition, and they overlap zero Rebalanced spans

## Selectable-option matrix

“Disjoint” means no byte conflict was found; it is not full combined-gameplay validation. All optional upstream fixes remain external.

| Upstream option | Default | Byte compatibility |
|---|---|---|
| Armor Attribute Fixes | Yes | Disjoint PPF writes |
| Badeaux Appears | Yes | Disjoint PPF writes |
| Castle Armory Fix | Yes | Disjoint PPF writes |
| Castle Farm Fix | Yes | Disjoint PPF writes |
| Chaco Bug Fix | Yes | Disjoint PPF writes |
| Circlet Name Correction | Yes | Disjoint text replacement; no protected-byte overlap |
| Collectibles Fix | Yes | Disjoint PPF writes |
| Emilia Dialogue Fix | Yes | Disjoint PPF writes |
| Forgiver Sign Fix | Yes | Disjoint PPF writes |
| Godspeed Rune Name Correction | Yes | Disjoint text replacement; no protected-byte overlap |
| Gozz Rune Renamed Minotaur Rune | Yes | Disjoint text replacement; no protected-byte overlap |
| Gozz Rune Renamed Gozu Rune | No | Disjoint text replacement; no protected-byte overlap |
| Gregminster Rune Shop Fix | Yes | Disjoint PPF writes |
| Gremio Text Fix | Yes | Disjoint PPF writes |
| GS1 Load - Names Fix | Yes | Disjoint PPF writes |
| GS1 Load - Tai Ho Import | Yes | Disjoint PPF writes |
| GS1 Load - Rune Import | Yes | Disjoint PPF writes |
| Inns Fix | Yes | Disjoint PPF writes |
| Join At 99 Fix | Yes | Disjoint PPF writes |
| Kindness Rune Fix (No Penalty) | No | Intentional Kindness behavior override: 1 different byte; 2 equal |
| Kindness Rune Fix (Penalty) | Yes | Already present: 4 identical bytes; idempotent |
| Knife-thrower Fix | Yes | Disjoint PPF writes |
| Lamb Fix (Unicorn Woods) | Yes | Disjoint PPF writes |
| Luca Battle Party-change Fix | Yes | Disjoint PPF writes |
| Matilda Gate Fix | Yes | Disjoint PPF writes |
| Music Fixes | Yes | Disjoint PPF writes |
| North Sparrow Escape Talisman Fix | Yes | Disjoint PPF writes |
| Rope Climb - Turtle Plans #4 | Yes | Disjoint PPF writes |
| Rune Speed Fix | Yes | Disjoint PPF writes |
| Rune Unite Fix | Yes | Disjoint PPF writes |
| Scroll Shop Display Fix | Yes | Disjoint PPF writes |
| Tenzan Pass Enemies Fix | Yes | Disjoint PPF writes |
| Tinto Glitch Fix | Yes | Disjoint PPF writes |
| Trade Gossip Translation | Yes | Disjoint PPF writes |

## Text replacements and growth

| Pass | Eligible files | Matches in original and v1.2 | Protected-byte overlap |
|---|---:|---:|---:|
| circlet | 60 | 61 | 0 |
| godspeed | 60 | 60 | 0 |
| gozu | 61 | 60 | 0 |
| minotaur | 61 | 60 | 0 |

The Minotaur variant replaces the five-byte `Gozz\0` slot with nine bytes. In all 60 actual v1.2 matches the following four bytes are zero padding, so this audited candidate has no new-data overwrite there. Godspeed and Circlet preserve the remaining string by shifting it one byte left and adding a terminator, matching the Lua code.

Only these PPFs append bytes:

| PPF / file | Before | After | Growth |
|---|---:|---:|---:|
| gremiotext.ppf / VF05.BIN | 324340 | 324516 | 176 |
| uwasa_1.ppf / UWASA1.BIN | 5232 | 7753 | 2521 |
| uwasa_2.ppf / UWASA2.BIN | 5232 | 7753 | 2521 |

The checked G1LOAD, knife-thrower and Tenzan PPFs do not grow their logical files. The shipped Gremio PPF appends 176 bytes; the source assembly alone must not substitute for the actual PPF.

## Patch order and limitations

For this audited v1.2 candidate, the supported composition direction is: **clean original USA image → Rebalanced xdelta → upstream bugfix tool**, selecting the desired external fixes. Keep the default Kindness Penalty option to preserve Rebalanced’s existing Kindness behavior. The No Penalty choice is an explicit behavior override.

Our xdelta is built against the clean original source hash. It is not a generic per-file merger and must not be applied to an image already rebuilt or modified by the bugfix tool. Reversing the order needs a separately constructed and tested patch for that exact source; none is provided.

The upstream PPF format checks its header, offsets and bounds but has no original-byte validation. It will blindly overwrite target offsets. The LBA sanity warning also does not stop its table write. Applying it to another revision, reordered layout or unrelated patch combination is outside this audit. Upstream fixes can intentionally change gameplay on their own even where their bytes are disjoint from ours.

The upstream rebuild changes file locations and regenerates internal LBA tables after selected files grow. This audit confirms those writes do not cover our edits; it does not execute the upstream ISO builder or certify every new scene, import behavior, combat/minigame fix, emulator or RetroAchievements use.

## Implementation notes

- The whole SLUS and SYSTEM.CNF files do not have to remain untouched: the installer checks their paths/existence, and this candidate safely changes SLUS at disjoint offsets. Our clean-source xdelta requirement remains strict
- A numeric same-file/range warning is insufficient: actual writes are mostly disjoint even in armor, Rune Speed, Rune Unite, Forgiver Sign, inns and armory resources
- The actual NA count is 36 PPFs / 34 options; the exact file list has 1,090 files
- Actual append effects are three PPFs, not speculative growth of G1LOAD/VB18/VA11
- The clean source and v1.2 both start BGM.XA at LBA343, and its entire 123,301,248-byte raw sector span is identical. LBA344 is mentioned in the installer comment, but the padding-sector creation call in that loop is commented out; the comment does not establish a forced rebuilt LBA
- “Both patch orders work” is not supported for a clean-source raw-image xdelta
- Download counts, ratings and RetroAchievements compatibility claims were not needed for this audit and are not certified

## Evidence

- [Pinned installer](https://github.com/pyriell/gs2-bugfixes/blob/e657ecafebdad2ed4c8e9031a8ab982fd506bf58/patcher.lua#L6696): LBA rewrite and warning behavior
- [Pinned text passes](https://github.com/pyriell/gs2-bugfixes/blob/e657ecafebdad2ed4c8e9031a8ab982fd506bf58/patcher.lua#L6862): Godspeed/Gozz/Circlet behavior
- [Pinned rebuild](https://github.com/pyriell/gs2-bugfixes/blob/e657ecafebdad2ed4c8e9031a8ab982fd506bf58/patcher.lua#L6995): source extraction and rebuild ordering
- [Pinned PPF parser](https://github.com/pyriell/gs2-bugfixes/blob/e657ecafebdad2ed4c8e9031a8ab982fd506bf58/patcher.lua#L7288): no source-byte validation
