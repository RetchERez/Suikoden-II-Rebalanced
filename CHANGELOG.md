# Changelog

By RetchERezzed

## v1.3 — 2026-11-27

- Added canonical CD-XA metadata repairs for Annallee Song, War Theme 1, War Theme 3 and Chant Song: 4,243 existing sectors receive duplicate file-number corrections and derived Form2 EDCs; audio samples and executable song filters remain unchanged
- Restored Meg’s Trick to 300% once per battle and Millie’s Groundhog to 200% once per battle, replacing v1.2’s weaker unlimited casts; retained their growth improvements and Millie’s head unlock at 30
- Retained Shin’s Spider Slay at repeatable 200%, Mayfly at 125% and Swallow at 150%
- Corrected the original Winup typo in all 60 Trick description copies to **3x DMG 1 time only**, matching the restored once-per-battle behavior
- Retained selected growth improvements for 22 characters; head unlocks for Tuta at 25, Millie at 30, Hai Yo at 45 and Hoi at 35; stronger coefficients for 14 Unite families and Cup of the Oath Bandit branches; and the existing Unite-description corrections
- Retained Clive’s five elapsed-time deadline removals, signed Kindness Penalty repair, two HQ exit-preload repairs, 64 Mercenary Soldier labels and reviewed spelling/rune-help/Potch/window fixes
- Verified deterministic patch encoding, exact decode and the complete guarded inventory of 1,215 logical edits plus 4,243 XA sector repairs; standalone layout and unlisted bytes remain unchanged
- Verified native Meg/Millie first-use damage, same-battle blocking and new-battle reset, plus Shin’s second execution/availability through victory and field return; later 60 Trick-text corrections were independently checked as text/checksum-only
- Verified Annallee’s first actual song with matching ordinary saves and 287-command native replays on candidate/retail, separately with SCPH-1001 and supplied actual SCPH-5501 firmware: a matched 30-second window contains song-correlated candidate PCM versus retail silence, with matched field/story/script witnesses and post-song dialogue
- Verified all four repaired streams by routing/EDC and complete nonzero decoding; the other three scenes have not received equivalent native scene replays
- **Full GS2 Bug Fix Patch v2.02.078 compatibility**: verified default Linux composition across 1,090 payloads, 17 disc-address tables and 35 PPFs while retaining all 1,215 Rebalanced logical edits; bounded overdue Radat/save checks are supplemented by cold reload, retained flags/party and normal field movement on the final corrected combined image
- Retained the external pack’s optional status and Kindness Penalty patch order; Windows installer execution, alternate options and every upstream fix remain unverified
- Added bounded encounter/resource and actual-selector diagnostics; no enemy or boss numerical data changed. Supplied level 4–5 Mist Shade save won in nine planned rounds using finite owned resources, including 19 Medicine charges and two L1MP, after a no-Medicine loss
- Verified Sword victory in eight rounds with six survivors, seven Medicine charges and finite MP, followed by story/field continuation and an ordinary save. The supplied legacy save has unknown prior history and retains retail cached growth profiles; its conservative policy is not a minimum-resource benchmark.
- Abomination was beaten in eight planned rounds with all six alive, using 16 Medicine charges and finite MP. Two survivors ended at 9 and 15 HP. Reward, post-boss dialogue and ordinary field movement were verified. An earlier policy lost; the retry differed in starting HP, resources and RNG, so this is not a controlled policy-only comparison. No extra training or equipment purchases were used. Four weapons were level 5; source gear, empty rune slots, legacy retail growth tables and conservative healing limit the difficulty assessment. These are observed costs, not minimum required resources or a whole-game balance certificate.
- Preserved the 16 photos/eight-photo collage as a clearly labeled v1.1 archive; no new images or GIFs

Current standalone patched BIN: `5a5d01a66dd4b105463ee63201c9b193ddcb9bb53d8fe591cab582dca5a33120`

Current xdelta: `41c1b33ab8a6e760402729e79dabe138764daa0a560420c3efcac19b8018e2b3`, 130,800 bytes

This release is a complete clean-source patch. The ZIP contains only the xdelta and two readmes. Existing saves keep earned stats and embedded growth/rune-slot data; already failed Clive flags are not reset. A full campaign, every party/loadout/quest, endings and real hardware remain unverified. Diagnostic models are not complete PS1 battles or win-rate certification.

## v1.2

- Removed Clive's five local elapsed-playtime deadline checks at Lakewest, Forest Village, Rockaxe, Radat and Sajah
- Kept the normal game clock, story prerequisites, one-time flags and all v1.1 combat/text/UI edits unchanged
- Verified all five callback machine-code paths in controlled Linux CPU tests and a native same-save overtime Radat comparison
- Verified ordinary post-event save and cold-reload persistence
- **Full GS2 Bug Fix Patch v2.02.078 compatibility**: verified the combined default profile in Linux, including overdue Radat, post-event save/cold reload and repeat Spider Slay through victory
- Independently verified all combined file payloads, disc-address tables, checksums and retention of all 1285 Rebalanced edits
- The combined test uses a Linux builder with upstream patch data; Windows GUI/CD-builder execution, all upstream fixes and alternate options are not certified
- Documentation and v1.2 ZIP readmes refreshed after compatibility testing; the standalone xdelta patch is unchanged
- Retained the existing standalone Kindness Penalty fix; the optional external No Penalty variant intentionally overrides it
- Updated the full 1285-edit ledger, save caveats and both compact BBCode posts

Existing failed quest flags are not reset. The rest of the Gremio/Tir quest remains deferred. A full v1.2 campaign remains unverified

## v1.1

- Project title updated to Suikoden II: Rebalanced with the tested game patch unchanged
- Added bounded Linux checks for a 108-star Suikoden I import and, on a separate late-game save, living Gremio and Tir's Banner fishing encounter
- Replaced the captioned collage with an eight-photo 9:16 mosaic and supplied both spoiler-tag and open BBCode posts with paired screenshots

The combat configuration is unchanged from v1.0

- Fixed 177 stale Trick, Groundhog, and Spider Slay descriptions across 59 resources, covering field, shop, and post-battle menu copies
- Fixed the separate personal-rune battle-help strings in both battle layouts, including Mayfly and Swallow damage information
- Added a dictionary and contextual spelling pass across 1,071 readable resources in the observed English game-font and ASCII encodings
- Corrected 59 additional spelling forms across 365 reviewed text spans, including detach, targeted, questions, soldiers, mustn't, haven't, and misplaced apostrophes
- Corrected three copies of “suprised” to “surprised”
- Reverified all 64 existing Mercenary Soldier label corrections
- Standardized 380 lowercase currency references to Potch and retained 27 already capitalized references
- Added spacing to 25 standalone currency labels and repaired verified money-window widths to fit the maximum amount
- Shifted two Chinchirorin money windows eight pixels left to preserve the gap between neighbouring frames
- Preserved proper names, deliberate dialect, singing, and stammering after reviewing the dictionary matches
- Used minor nearby wording, punctuation, or redundant spacing where longer corrections needed to fit the original text slot
- Retained the original resource lengths, text-pointer layouts, combat program logic, combat values, and growth/rune-slot configuration
- Added 16 varied photos, an eight-picture 9:16 portrait collage, capture provenance, and fresh Linux battle replays on the exact v1.1 image
- Added twelve text/currency/layout regression checks alongside the existing 96-test Linux tooling suite

The complete vanilla-to-v1.1 ledger contains 1280 guarded edits across 217 game files. Its readable passages and exact bytes document the text-fit adjustments

v1.1 is a complete patch for the clean USA SLUS-00958 original. Do not apply it over v1.0. Existing correctly migrated v0.99/v1.0 cards need no further growth-table migration; restart the emulator and use ordinary in-game saves

The text review does not certify a full retranslation, every dialogue rendering, or universal grammatical perfection. Full campaign and real-hardware testing remain outstanding

## v1.0

The earlier release remains available

- Selected growth improvements for 22 characters and earlier head rune slots for Tuta, Millie, Hai Yo, and Hoi
- Personal-rune damage adjustments and repeat use for Trick, Groundhog, and Spider Slay
- Coefficient increases for 14 named Unite families, with matching Unite description updates
- The signed negative-Kindness repair, preserving its ordinary attack penalty
- 64 equal-length Mercenary Solider to Mercenary Soldier label corrections
- Two Headquarters exit-preload boundary repairs
- Patch reconstruction, numerical/native-engine checks, and selected downloaded-save routes

The original v1.0 package is retained unchanged. Some separate rune-menu descriptions still display vanilla wording in that version; v1.1 repairs those sources and adds the broader spelling cleanup
