# Full GS2 Bug Fix Patch v2.02.078 compatibility

By RetchERezzed

This describes the default optional full-pack composition and bounded native checks. The standalone Rebalanced download does not bundle the full pack or a combined game image.

## Sources and exact images

Upstream: [Pyriel’s gs2-bugfixes](https://github.com/pyriell/gs2-bugfixes), pinned revision [`e657ecafebdad2ed4c8e9031a8ab982fd506bf58`](https://github.com/pyriell/gs2-bugfixes/tree/e657ecafebdad2ed4c8e9031a8ab982fd506bf58).

| Artifact | SHA-256 |
|---|---|
| Clean USA source BIN | `acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472` |
| Standalone v1.3 patched BIN | `5a5d01a66dd4b105463ee63201c9b193ddcb9bb53d8fe591cab582dca5a33120` |
| Standalone xdelta, 130,800 bytes | `41c1b33ab8a6e760402729e79dabe138764daa0a560420c3efcac19b8018e2b3` |
| Private final corrected combined BIN | `d2e9841892abf8687edb6cec51b505c30c7f37058c1af4a47b00844ab9cf17cb` |

The standalone patch preserves the original disc layout. Its 1,215 logical edits and 4,243 repaired XA sectors account for 4,856 changed raw sectors and 103,878 differing raw bytes, including derived checksums. Deterministic repeat encoding, exact decode and source preservation pass.

## Default Linux composition

The private combined image was built in Linux from the shipped default patch data: 32 selected options, 35 PPFs, Kindness Penalty and the Godspeed/Minotaur/Circlet text passes. Independent checks verify all 1,090 file payloads, all 17 disc-address tables with 1,090 entries each, retention of all 1,215 Rebalanced logical edits, normal raw-sector metadata/checksums and unchanged sectors outside the authorized writes.

Three logical files grow: `VF05.BIN` by 176 bytes within its allocation and `UWASA1.BIN`/`UWASA2.BIN` by 2,521 bytes each, relocated into verified trailing padding. The corresponding ISO records and internal tables are updated; extents do not overlap. Normal XA subheaders and terminal EOF/EOR metadata were checked on the final corrected image.

The canonical standalone music corrections match the corresponding shipped Music Fixes data and compose idempotently with it. The four requested file numbers are retained in the executable; duplicate XA subheader file numbers and derived Form2 EDCs are repaired. Audio samples are unchanged. The alternative four-byte executable-filter workaround must not be added to this canonical repair.

## Bounded native checks

A combined mechanics build completed overdue Radat progression and an ordinary post-event save. The final corrected combined image then cold-loaded that same save, retained quest flags and party, advanced the saved clock from 32:53:00 to 32:53:08 and allowed normal field movement. All campaign save blocks remained byte-identical; one reserved card-header byte normalized on mounting. The later 60-description correction is independently audited as text/checksum-only relative to the mechanics-tested image.

Inputs were normal controller actions, with read-only RAM/card observations, no save-state loads and no guest gameplay writes. The final cold-load test completed its observations and its exact owned process was deliberately stopped and reaped; its controlled exit is not a runtime crash. Earlier host-wrapper cleanup time limits from the longer Radat trial remain recorded as host limitations. No screenshot or new media claim is made.

Standalone rune tests separately observed Meg/Millie first-use damage, same-battle blocking and new-battle reset. Shin’s second execution/availability was observed; these v1.3 checks do not claim a measured second damage hit. Earlier v1.2 combined battle evidence remains historical and is not substituted for a new final-image battle.

## Music evidence and firmware identity

All four repaired streams pass complete routing/EDC and nonzero decode checks. Annallee’s first South Window song additionally passed an exact 287-command replay from the same ordinary pre-song save on the standalone candidate and retail. Both reached matching field/story/script witnesses and post-song dialogue. A matched 30-second no-input window had candidate RMS 3710.30, versus exact retail silence; the candidate waveform correlated 0.99036 with the decoded Annallee asset. Private PCM is not distributed.

The original paired replay used native Linux Beetle with an existing **SCPH-1001** BIOS, SHA-1 `10155d8d6e6e832d6ea66db9bc098321fb5e8ebf`, privately named `scph5501.bin`; the core’s checksum warning was retained. A separate, completed pair used the supplied actual **SCPH-5501 USA** BIOS, SHA-1 `0555c6fae8906f3f09baf5988f00e55f88e9f30b`, accepted without a firmware warning. That pair repeated the same checkpoint, 287 commands/17,736 frames, nine matched native witnesses, identical 30-second PCM results and post-song dialogue, then shut down cleanly. The original reports remain unchanged. These are named-core/firmware results, not console-hardware or all-emulator certification. The other three music scenes have not received equivalent native scene replays.

## Patch order and options

Use **clean original USA image → Rebalanced xdelta → optional upstream tool**. Keep the default **Kindness Penalty** to preserve Rebalanced’s intended signed negative-rating behavior. **No Penalty** intentionally overrides it. Both the Kindness Penalty repair and the corresponding canonical music writes are already present where documented; the full pack supplies its other repairs externally.

The Rebalanced xdelta strictly requires the clean original hash. It cannot be applied to a previously rebuilt or bugfix-patched image. No reverse-order patch is supplied. Keep source/card backups, restart the emulator and use normal saves. Existing saves retain their embedded growth/rune-slot table and earned stats; a disc patch does not migrate those tables or reset failed Clive flags.

Upstream PPF application does not guard each original target byte, and its table warning does not stop a write. Other revisions, layouts, unrelated patches and alternate option combinations therefore need their own audit. Byte-disjoint writes alone do not certify combined gameplay.

## Limits and retained history

The upstream Windows GUI/CD builder did not execute successfully in WSL. Linux data composition and bounded native routes do not certify that installer, its output layout, every external fix/option, all import behaviors, RetroAchievements, a full campaign or real hardware.

Enemy/boss numbers are unchanged. Mist’s finite-resource result and earlier selected encounters do not establish all-party difficulty or universal no-grind viability. Standalone Sword and Abomination victories are verified, with their finite-resource and source-party limits recorded in README.txt. These do not substitute for a final combined-image boss trial. Diagnostic AI/planner models retain documented targeting, status, acquisition and phase gaps.

[CHANGELOG.md](CHANGELOG.md) preserves v1.2 and earlier evidence as version-specific history. Its old 1,285-edit counts and previous combined hashes describe those earlier images, not this release. Full source/card provenance and raw test artifacts remain private QA material.
