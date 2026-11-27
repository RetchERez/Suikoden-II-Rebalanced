# Suikoden II: Rebalanced v1.3

By RetchERezzed

v1.3 repairs four missing music streams and restores stronger once-per-battle opening attacks for Meg and Millie, while retaining the growth, rune access, Unite, Clive and text improvements from earlier releases.

- **Music:** canonical XA metadata repairs for Annallee Song, War Theme 1, War Theme 3 and Chant Song; existing samples and executable song filters are unchanged
- **Meg:** Trick returns to 300% once per battle, with all 60 description copies correcting the original Winup typo to **3x DMG 1 time only**
- **Millie:** Groundhog returns to 200% once per battle; her growth improvements and head slot at level 30 remain
- **Shin:** Spider Slay stays repeatable at 200%
- **Retained:** 22-character growth improvements, four earlier head rune unlocks, Mayfly/Swallow adjustments, stronger coefficients for 14 Unite families and Cup of the Oath Bandit branches, Clive’s five removed elapsed-time deadlines, signed Kindness Penalty repair, two HQ preload repairs, reviewed spelling/rune help/Potch/window fixes

Meg and Millie trade v1.2’s unlimited weaker casts for stronger first-use bursts. Enemy and boss numbers are unchanged; the encounter review is not a completed whole-game balance pass.

## Evidence and limits

The 130,800-byte xdelta encodes deterministically and round-trips to the exact patched BIN. The audited change inventory is **1,215 logical edits plus 4,243 XA sector repairs**.

Native Linux checks cover Meg/Millie’s first use, same-battle blocking and new-battle reset, Shin’s repeat availability, victory/rewards/field return, and Annallee’s first actual song. The exact same ordinary checkpoint and 287-command replay produced song-correlated candidate PCM versus retail silence in a matched 30-second wait. Separate paired tests passed with disclosed SCPH-1001 and supplied actual SCPH-5501 firmware. The other three music tracks have routing and decoded-asset evidence only.

Mist Shade was beaten from a supplied level 4–5 save in nine planned rounds using finite owned resources, including 19 Medicine **charges** and two L1MP; the first no-Medicine policy lost. Sword was beaten in eight rounds with six survivors, seven Medicine **charges** and finite MP, followed by an ordinary save. Its conservative policy is not a minimum-resource benchmark.

Abomination was beaten in eight planned rounds with all six alive, using 16 Medicine charges and finite MP. Two survivors ended at 9 and 15 HP. Reward, post-boss dialogue and ordinary field movement were verified. An earlier policy lost; the retry differed in starting HP, resources and RNG, so this is not a controlled policy-only comparison. No extra training or equipment purchases were used. Four weapons were level 5; source gear, empty rune slots, legacy retail growth tables and conservative healing limit the difficulty assessment. These are observed costs, not minimum required resources or a whole-game balance certificate.

Supplied save history is unknown, and these observations are not win rates or a complete campaign assessment. Full campaign, every party/loadout/Unite variant, all quests, endings and real hardware remain unverified.

## Full GS2 Bug Fix Patch v2.02.078 compatibility

The optional default profile passed Linux composition across **1,090 file payloads, 17 tables and 35 PPFs**, retaining all Rebalanced edits. Bounded overdue Radat/ordinary-save checks pass; the final corrected combined image cold-loaded that save with flags/party intact and working field movement. The Windows installer, alternate options, every upstream fix and full campaign remain unverified. See [COMPATIBILITY.md](COMPATIBILITY.md).

The pack remains optional and external. Apply **clean original → Rebalanced → upstream tool**, retaining **Kindness Penalty**. Standalone Rebalanced includes only the documented Kindness and four canonical music repairs from that project.

## Installation and package

Patch the untouched USA SLUS-00958 single-track MODE2/2352 original, including when upgrading. Use a new output BIN and copied CUE; do not patch an earlier Rebalanced image. The ZIP contains exactly:

- `Suikoden-II-Rebalanced-v1.3.xdelta`
- `README.txt`
- `README_EVERY_CHANGE.txt`

No ROM, BIOS, emulator, save, game audio or private QA material is included. Vanilla saves keep their embedded growth/rune-slot table and earned stats. Correctly migrated Rebalanced saves need no additional table migration; restart the emulator and use normal saves.

| Artifact | SHA-256 |
|---|---|
| Required source BIN, 513,907,296 bytes | `acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472` |
| Patched BIN | `5a5d01a66dd4b105463ee63201c9b193ddcb9bb53d8fe591cab582dca5a33120` |
| xdelta, 130,800 bytes | `41c1b33ab8a6e760402729e79dabe138764daa0a560420c3efcac19b8018e2b3` |

The existing 16 photos and eight-photo collage are explicitly a **v1.1 archive**, with possible spoilers and older rune values. No new images or GIFs are supplied.

Credits: [Pyriel’s gs2-bugfixes](https://github.com/pyriell/gs2-bugfixes) for the original Kindness repair and canonical music reference; Cloudstrife7894, Dyne and community save authors. Earlier release history is preserved in [CHANGELOG.md](CHANGELOG.md).
