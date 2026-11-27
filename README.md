# Suikoden II: Rebalanced v1.3

By RetchERezzed

[Download v1.3](https://github.com/RetchERez/Suikoden-II-Rebalanced/releases/download/v1.3/Suikoden-II-Rebalanced-v1.3.zip)

A combat rebalance for the original USA PlayStation release, intended to make more party choices useful while keeping resource management relevant.

## New in v1.3

- Repairs missing Annallee Song, War Theme 1, War Theme 3 and Chant Song playback using canonical CD-XA metadata corrections. The existing audio samples and executable song filters are unchanged
- Returns Meg’s Trick to **300% once per battle** and Millie’s Groundhog to **200% once per battle**. These stronger opening attacks trade away v1.2’s unlimited weaker casts; they are not a universal sustained-damage increase
- Keeps Shin’s Spider Slay **repeatable at 200%**, Meg/Millie’s growth improvements and Millie’s head rune slot at level 30
- Corrects the original **Winup** typo in all 60 Trick description copies, now reading **3x DMG 1 time only**

Enemy and boss numbers are unchanged. The encounter review remains a bounded evidence pass, not a completed whole-game difficulty rebalance.

## Included changes

- Selected growth improvements for 22 characters; earlier head rune slots for Tuta at 25, Millie at 30, Hai Yo at 45 and Hoi at 35
- Mayfly at 125%, Swallow at 150%, stronger coefficients for 14 Unite families and the Cup of the Oath Bandit branches, with matching descriptions
- Clive’s five elapsed-playtime deadlines removed at Lakewest, Forest Village, Rockaxe, Radat and Sajah. The clock, initial Muse encounter, story prerequisites and one-time flags remain; already failed quest flags are not reset
- The signed negative-Kindness repair, retaining its normal attack penalty; two Headquarters exit-preload repairs; 64 Mercenary Soldier label corrections
- Reviewed spelling, rune help, Potch capitalization/spacing and money-window clipping repairs. This is not a full retranslation

[CHANGELOG.md](CHANGELOG.md) preserves earlier release history. The packaged `README_EVERY_CHANGE.txt` lists every exact vanilla-to-v1.3 edit.

## Install and saves

Use your own legally sourced, untouched USA **SLUS-00958**, single-track **MODE2/2352 BIN/CUE**. The source BIN must be **513,907,296 bytes**, with SHA-256:

`acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472`

Apply the complete v1.3 xdelta to that clean original, including when upgrading from an earlier Rebalanced release. Use a new output BIN; copy the original CUE, change only its `FILE` filename to the new BIN, retain its `TRACK`/`INDEX` lines and launch the copied CUE. Keep the original and save backups. Other regions/revisions, prepatched images and CHDs are unsupported patch inputs. The packaged `README.txt` contains the xdelta commands.

The release ZIP contains exactly `Suikoden-II-Rebalanced-v1.3.xdelta`, `README.txt` and `README_EVERY_CHANGE.txt`. No ROM, BIOS, emulator, save or game audio is distributed.

A new game is recommended for the complete rebalance. Vanilla saves keep their embedded growth/rune-slot table and already earned stats; patching the disc does not migrate either. Correctly migrated Rebalanced saves need no new table migration in v1.3. Migration tools are not included. Restart the emulator and use normal saves rather than carrying save states across versions.

## Verification and limits

The patch encodes deterministically and decodes to the exact patched BIN. All **1,215 logical edits** and **4,243 XA sector repairs** are guarded; whole-disc checks verify checksums, unchanged standalone layout and every unlisted raw byte.

Native Linux tests observed Meg/Millie’s first-use damage, same-battle blocking and new-battle reset, plus Shin’s repeat availability through victory and field return. Annallee’s first song passed the same-save 287-command native comparison with both SCPH-1001 and the supplied actual SCPH-5501 firmware: a matched 30-second wait contains song-correlated PCM on v1.3 and exact silence on vanilla. The other three tracks have routing and decoded-asset verification, rather than native scene replays.

Mist Shade was beaten from a supplied level 4–5 save after nine planned rounds using finite owned resources, including 19 Medicine **charges**, following a no-Medicine loss. Sword was beaten in eight rounds with all six alive, using seven Medicine **charges** and finite MP. Its conservative policy is not a minimum-resource benchmark.

Abomination was beaten in eight planned rounds with all six alive, using 16 Medicine charges and finite MP. Two survivors ended at 9 and 15 HP. Reward, post-boss dialogue and ordinary field movement were verified. An earlier policy lost; the retry differed in starting HP, resources and RNG, so this is not a controlled policy-only comparison. No extra training or equipment purchases were used. Four weapons were level 5; source gear, empty rune slots, legacy retail growth tables and conservative healing limit the difficulty assessment. These are observed costs, not minimum required resources or a whole-game balance certificate.

Earlier selected boss, Suikoden I import and Gremio/Tir Banner-introduction checks remain qualified evidence. Supplied saves have unknown prior training/editing history.

Diagnostics and resource-planning comparisons have documented AI, targeting, status, acquisition and phase limits. They do not establish battle win rates or a full PS1 simulation. A full campaign, every party/loadout/Unite variant, all quests, endings and real hardware remain unverified.

## Full GS2 Bug Fix Patch v2.02.078 compatibility

The optional default profile passed Linux data composition across **1,090 file payloads, 17 disc-address tables and 35 PPFs**, retaining all 1,215 Rebalanced edits. A combined mechanics build completed overdue Radat and an ordinary save; the final corrected combined image cold-loaded that save, retained flags/party and allowed field movement.

Apply **clean original → Rebalanced → optional upstream tool**, keeping **Kindness Penalty**. The full pack remains external; standalone Rebalanced includes only its documented Kindness repair and four canonical music repairs. Windows installer execution, alternate options and every upstream fix are not certified. See [COMPATIBILITY.md](COMPATIBILITY.md) for exact evidence and limits.

## Screenshots

The existing [16-photo gallery](media/README.md) and **eight-photo 9:16 collage** are a **v1.1 archive**, captured in Linux with normal controller input. They may contain location spoilers and older rune values; use the v1.3 values above. No new images or GIFs accompany this release.

![Eight-photo portrait collage — v1.1 archive](media/Suikoden-II-Rebalanced-v1.1-Photo-Collage.png)

## Credits and feedback

[Pyriel’s gs2-bugfixes project](https://github.com/pyriell/gs2-bugfixes) supplies the original signed-penalty Kindness fix and canonical Music Fixes reference. Additional thanks: Cloudstrife7894, Dyne and community save authors whose checkpoints enabled the documented bounded tests.

For a bug report, include emulator/version, location, party/levels, equipment/runes, save origin, patched BIN hash and reproduction steps.

The representative save-based review covers Mist Shade, Sword and Abomination, alongside qualified earlier encounter evidence. The target remains moderate challenge, varied parties and no extra grinding. No enemy or boss numerical/AI changes were made. Abomination was a difficult, healing-intensive win; source equipment, empty rune slots, legacy growth tables and a conservative player policy limit the inference. These results support retaining the current numbers for public testing; they do not certify moderate difficulty across the whole game or every party.
