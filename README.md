# Suikoden II: Rebalanced v1.1

A combat rebalance and spelling cleanup for the original USA PlayStation release, by RetchERezzed

**[Download v1.1](https://github.com/RetchERez/Suikoden-II-Rebalanced/releases/download/v1.1/Suikoden-II-Rebalanced-v1.1.zip)** Â· [Installation](README.txt) Â· [Every change](README_EVERY_CHANGE.txt) Â· [Screenshots and capture notes](media/README.md)

![Eight Linux captures in a 9:16 portrait collage](media/Suikoden-II-Rebalanced-v1.1-Photo-Collage.png)

The rebalance gives more of the roster a useful role through selected growth improvements, earlier rune access, repeatable personal runes, and stronger underused Unites

## Main changes

- Selected growth improvements for 22 characters
- Earlier head rune slots for Tuta, Millie, Hai Yo, and Hoi
- Repeat use of Trick, Groundhog, and Spider Slay, with adjusted damage coefficients
- Damage adjustments for Mayfly and Swallow
- Coefficient increases for 14 named Unite families
- The signed negative-Kindness fix, preserving its ordinary attack penalty
- Two Headquarters exit-preload boundary repairs
- Corrected Mercenary Soldier labels and reviewed spelling fixes throughout readable dialogue, descriptions, labels, and menus
- Consistent Potch capitalization and spacing in currency text, with verified money-window width repairs

## New in v1.1

The combat configuration stays the same as v1.0

The text cleanup fixes 177 duplicated rune descriptions and ten separate battle-help descriptions, then adds reviewed spelling, contraction, and text-fit corrections. The pass covers 1,071 readable resources using the observed English game font and ASCII, with independent review of punctuation and false positives. Character names, dialect, singing, and stammering are preserved

Longer corrections sometimes use minor nearby wording or redundant spacing to retain the original text-slot size. The complete change list includes readable before-and-after passages and exact bytes for all 1280 guarded edits

## Install

Use your own legally sourced, untouched USA **SLUS-00958** single-track **MODE2/2352 BIN/CUE**. Follow [README.txt](README.txt) to verify the original hash, apply the xdelta patch to a separate BIN, update a copied CUE, and verify the result

The download ZIP contains exactly three files

- `Suikoden-II-Rebalanced-v1.1.xdelta`
- `README.txt`
- `README_EVERY_CHANGE.txt`

No game image, BIOS, emulator, memory card, or save state is included

## Existing saves

A new game is recommended for the complete rebalance. Vanilla saves retain their own growth/rune-slot table, and the patch does not retroactively increase earned stats. Save-migration tools are not part of this three-file package

Correctly migrated v0.99/v1.0 saves need no further table migration for v1.1. Use normal in-game saves and restart the emulator on the v1.1 CUE; older emulator save states can retain cached code or menu text

Apply v1.1 to a clean original, including when upgrading from v1.0. No previous patch is required

## Verification

The patch has deterministic encoding, an exact decode round-trip, source-preservation checks, and a byte audit confirming that the changes since v1.0 are confined to the documented text/UI-layout fields and CD checksums

The existing Linux tooling suite passes 96 tests, and twelve new regression checks cover text, spelling, pointer layouts, opaque controls, and unchanged resources. An independent review checked the text changes and remaining dictionary matches

The gallery contains 16 varied photos and an eight-picture 9:16 portrait collage, freshly captured in native Linux PCSX-Redux on the exact v1.1 image. Private copies of downloaded cards and normal controller inputs cover menus, battles, dialogue, and early-to-late locations. These checkpoint visits include possible spoilers; capture notes distinguish visible scenes from measured action effects

This release is ready for public testing. A full campaign, every legal recruitment/loadout/Unite combination, endings, and real hardware remain unverified. The spelling review is not a claim of a complete retranslation or universal grammatical perfection

## Credits and feedback

Rebalance by RetchERezzed. The negative-Kindness repair incorporates [Pyriel's published signed-penalty fix](https://github.com/pyriell/gs2-bugfixes), rather than the complete upstream collection

For a bug report, include your emulator/version, location, party and levels, equipment, runes, patched BIN hash, save origin, and reproduction steps. Screenshots of remaining text issues are welcome

v1.0 remains available as the earlier release. v1.1 is the latest version and adds the menu and spelling corrections documented in [CHANGELOG.md](CHANGELOG.md)
