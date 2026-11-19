SUIKODEN II: REBALANCED v1.1
By RetchERezzed

ABOUT THE PATCH

A focused combat rebalance for the original USA PlayStation game. It adjusts
growth for 22 characters, four head-rune unlock levels, personal runes and
14 named Unite families, and includes the documented Kindness, spelling
and Headquarters preload fixes. README_EVERY_CHANGE.txt lists every edit.

NEW IN v1.1

Corrected 177 stale descriptions for Trick, Groundhog and Spider Slay across
59 resource files, plus ten separate FST/SEC battle-help descriptions.
A dictionary and contextual review also corrects spelling across readable
dialogue, labels, rune/weapon/war descriptions and menus, including additional
soldiers spellings, contractions and surprised. All 64 Mercenary Soldier
label fixes are verified. Character names and intentional dialect remain.
Currency references now consistently use Potch in menus, prices, spending,
rewards and dialogue: 380 lowercase occurrences corrected and 27 retained.
25 standalone labels gain a space before Potch within existing slot padding.
30 verified money-window widths expand one text cell to fit the added space.
Two Chinchirorin windows shift eight pixels left to avoid overlapping frames.
44 later shop resize calls retain the expanded width instead of clipping Potch.
The v1.0 combat configuration is unchanged.

This ZIP contains exactly:
  Suikoden-II-Rebalanced-v1.1.xdelta
  README.txt
  README_EVERY_CHANGE.txt

REQUIRED ORIGINAL

Use your own legally sourced, untouched USA SLUS-00958 single-track
MODE2/2352 BIN/CUE. The BIN must be exactly 513907296 bytes.

Original BIN SHA-256:
acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472

Other regions, revisions, prepatched images, compressed CHDs and combinations
with other hacks are unsupported inputs. Keep your original and saves backed up.

HOW TO APPLY

Extract the ZIP and obtain xdelta3 from its upstream project:
https://github.com/jmacd/xdelta/releases
The recorded Linux checks used xdelta3 version 3.0.11.

Check your original's SHA-256 before patching:
Windows PowerShell: Get-FileHash -Algorithm SHA256 "original.bin"
Linux: sha256sum "original.bin"

Apply the patch to the BIN, using a NEW destination filename. Substitute your
actual original path in these examples. Keep the original untouched.

Linux, with xdelta3 on PATH:
xdelta3 -d -s "original.bin" "Suikoden-II-Rebalanced-v1.1.xdelta" "Suikoden II Rebalanced v1.1.bin"

Windows PowerShell, with xdelta3.exe in the extracted directory:
.\xdelta3.exe -d -s "original.bin" "Suikoden-II-Rebalanced-v1.1.xdelta" "Suikoden II Rebalanced v1.1.bin"

Verify the resulting BIN against the v1.1 SHA-256 below. Copy your original
CUE to a separate CUE beside the new BIN. In the copied CUE only, change
the FILE entry to:
FILE "Suikoden II Rebalanced v1.1.bin" BINARY

Preserve all original TRACK and INDEX lines. Open that copied CUE in your
emulator. A new game is recommended for the complete rebalance.

v1.1 BIN SHA-256:
e193bd3d03c41ef59e50da57d23c78a70fae0138742582f53f4c10096f8fcfb3

Patch SHA-256:
87f183d394096cde947746d2bd96c85c3b40c7eadaa9fe62b709b01650a4442a

UPGRADING AND EXISTING SAVES

Apply v1.1 to your clean original, not to a v1.0 patched image. This is a
complete vanilla-to-v1.1 patch, so no earlier patch is required.

Vanilla saves store their own growth/rune-slot table. Disc patching does not
migrate that table or retroactively change earned stats. Save-migration tools
are not included in this three-file package. A new game receives the complete
configuration. Correctly migrated v0.99/v1.0 cards already have the matching
growth/slot table and need no new table migration for v1.1.

Use normal in-game saves. Restart the emulator on the v1.1 CUE to refresh
cached menu data. Do not carry emulator save states across versions.

VERIFICATION AND LIMITS

The v1.1 audit verifies every documented text/UI-layout edit and confirms that every
other resource byte stays identical to v1.0, apart from CD checksums.
The spelling scan covers 1071 readable ISO resources in game-font and ASCII
encodings, with an independent punctuation-aware review. Names, dialect and
binary/diagnostic false positives are reviewed rather than auto-corrected.
19 non-Form1 audio/video resources are excluded from the text scan.
The patch has deterministic repeat encoding, an exact decode round-trip and
original-preservation checks. The existing Linux tooling suite has 96 tests;
twelve new regression checks cover menus, spelling, currency, layout, controls, pointers
and unchanged resources.

The underlying v1.0 evidence includes Linux PS1 native-engine measurements,
selected downloaded-save battles and representative boss fights. v1.1 changes
only documented text/UI-layout fields; it does not turn earlier bounded evidence into a
new campaign certification. Current screenshots and their accompanying
capture notes distinguish visible scenes from measured action effects.

Additional Linux checks accepted a genuine 108-star Suikoden I save on both
vanilla and v1.1 cold boots. The v1.1 growth/rune-slot table matched the patched
image after import. On a separate genuine late-game imported save, normal
controller input reached living Gremio's Banner blocker dialogue and Tir's
fishing encounter. This is two separate checkpoint tests, not one uninterrupted
playthrough from import. The remaining rescue quest, its boss and Gregminster
return, plus the optional departure dialogue branch, remain unverified.

Ready for public testing. Full campaign difficulty, every legal recruitment
stage/loadout/Unite combination, endings and real hardware remain unverified.
This is not a complete translation or the complete upstream retail bugfix suite.
For a bug report include emulator/version, location, party/levels, equipment,
runes, reproduction steps, patched BIN hash and save origin.

CREDITS AND DISTRIBUTION

Rebalance by RetchERezzed. The signed negative-Kindness repair incorporates
Pyriel's published penalty-preserving fix from gs2-bugfixes, commit
e657ecafebdad2ed4c8e9031a8ab982fd506bf58, patch/NA/src/kindness_rune.asm:
https://github.com/pyriell/gs2-bugfixes

Only the patch and these two documents are included. No game image, BIOS,
emulator, downloaded save or save state is distributed. Keep your generated
game image and private test assets private.
