SUIKODEN II: COMBAT REBALANCED v1.0 Final
By RetchERezzed

PLAYER PACKAGE

This ZIP contains exactly three files:
  suikoden_ii_combat_rebalanced_v1.0_final.xdelta
  README.txt (installation, compatibility and testing limits)
  README_EVERY_CHANGE.txt (complete vanilla-to-v1.0 change list)

The game patch is identical to the previously verified v1.0 Final. This is
a smaller distribution package, with standalone xdelta3 instructions.

WHAT CHANGES

Character growth and rune-slot adjustments, personal-rune damage and repeat
use adjustments, Unite coefficients and descriptions, the signed negative
Kindness Rune fix, 64 Mercenary Soldier spelling corrections, and two
Headquarters exit-preload boundary repairs. The complete change list records
all 269 guarded edits across 72 game files, including original/final bytes
and file offsets. This is not a complete translation or retail bugfix suite.

REQUIRED ORIGINAL

Use your own legally sourced, untouched USA SLUS-00958 PlayStation BIN/CUE:
single-track MODE2/2352, with a BIN of exactly 513907296 bytes.

Original BIN SHA-256:
acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472

Other regions, revisions, prepatched images, and combinations with other
hacks are unsupported. Back up the clean original and your memory cards.
The patch is applied to the BIN, not the CUE or a compressed CHD file.

INSTALLATION

1. Extract all three files from this ZIP.
2. Obtain xdelta3 from its upstream project:
   https://github.com/jmacd/xdelta/releases
   Native Linux xdelta3 version 3.0.11 was used in the recorded checks.
3. Verify that your original BIN matches the size and SHA-256 above.
   Windows PowerShell: Get-FileHash -Algorithm SHA256 "original.bin"
   Linux: sha256sum "original.bin"
4. From the extracted directory, apply to a NEW output filename:

   Linux (xdelta3 installed on PATH):
   xdelta3 -d -s "original.bin" "suikoden_ii_combat_rebalanced_v1.0_final.xdelta" "Suikoden II Combat Rebalanced v1.0.bin"

   Windows PowerShell (xdelta3.exe in the extracted directory):
   .Þlta3.exe -d -s "original.bin" "suikoden_ii_combat_rebalanced_v1.0_final.xdelta" "Suikoden II Combat Rebalanced v1.0.bin"

   Substitute your actual original path. Keep the original untouched.
5. Verify the resulting BIN against the Final SHA-256 below. Do not use
   a result with a different hash.
6. Copy your original CUE to a separate CUE next to the new BIN. In that
   copy only, change its FILE entry to the new BIN filename, for example:

   FILE "Suikoden II Combat Rebalanced v1.0.bin" BINARY

   Preserve every TRACK and INDEX line from your original CUE unchanged.
   Open the copied CUE in your emulator and start a new game.

Final BIN SHA-256:
5e8233950e3ee0bdaf6a7fa180ea16da955e01b5b0c52f12dd769a8d357c1bde

Patch SHA-256:
1d37961d3e003000d72e2d594a425cb08a2ac2c88d5d34fb08cdfdcfab45c5cc

EXISTING SAVES

A new game is recommended for the complete rebalance. Vanilla saves store
their own character growth/rune-slot table; patching the disc alone does
not migrate that table or retroactively change earned stats. The save
migration tools are not included in this three-file player package.
Correctly migrated v0.99/v1.0 saves already have the matching table and
need no further table migration. Keep separate cards and use normal in-game
saves when switching images; do not carry emulator save states across builds.

TESTING AND LIMITS

The release was checked with Linux PS1 emulation, downloaded-save routes,
native engine measurements, patch/hash verification and 96 automated tests.
Focused checks include repeated Groundhog and Spider Slay in the same
battle, Tuta's automatic Medicine, Tomo's Unicorn action, Simone's physical
attack, normal victory/field continuation and representative boss fights.
Historical gameplay evidence retains the original image identity; relevant
unchanged resources were explicitly checked when carrying evidence forward.

v1.0 identifies this released configuration. It is ready for public testing;
it does not certify every character, legal recruitment stage, loadout,
Unite situation, encounter, campaign difficulty, ending, or emulator.
A full campaign playthrough and real-hardware testing remain outstanding.
No full translation pass or complete upstream bugfix collection is included.
For a bug report include emulator/version, location, party/levels, equipment,
runes, reproduction steps, Final BIN hash and save origin.

CREDITS AND DISTRIBUTION

Rebalance by RetchERezzed. Negative-Kindness repair incorporates Pyriel's
published signed-penalty-preserving fix from gs2-bugfixes, commit
e657ecafebdad2ed4c8e9031a8ab982fd506bf58, patch/NA/src/kindness_rune.asm:
https://github.com/pyriell/gs2-bugfixes

This ZIP distributes only the patch and these two text documents. It
contains no game image, BIOS, emulator, downloaded save, or save state.
Keep generated game images and private test assets private.
