SUIKODEN II: REBALANCED v1.2
By RetchERezzed

ABOUT THE PATCH

A focused combat rebalance for the original USA PlayStation game. It adjusts
growth for 22 characters, four head-rune unlock levels, personal runes and
14 named Unite families, and includes the documented Kindness, spelling
and Headquarters preload fixes. README_EVERY_CHANGE.txt lists every edit.

NEW IN v1.2

Removed Clive's five elapsed-playtime deadlines: Lakewest 11h, Forest Village 13h,
Rockaxe 14h, Radat 15h and Sajah 20h. The normal game clock keeps running.
Story access, recruitment prerequisites and one-time quest flags still apply.
You must still see the initial Muse encounter. Already failed or completed
quest flags are not reset; this does not automatically recover failed saves.
The combat configuration and all v1.1 text/Potch corrections are unchanged.

INCLUDED FROM v1.1

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
  Suikoden-II-Rebalanced-v1.2.xdelta
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
xdelta3 -d -s "original.bin" "Suikoden-II-Rebalanced-v1.2.xdelta" "Suikoden II Rebalanced v1.2.bin"

Windows PowerShell, with xdelta3.exe in the extracted directory:
.\xdelta3.exe -d -s "original.bin" "Suikoden-II-Rebalanced-v1.2.xdelta" "Suikoden II Rebalanced v1.2.bin"

Verify the resulting BIN against the v1.2 SHA-256 below. Copy your original
CUE to a separate CUE beside the new BIN. In the copied CUE only, change
the FILE entry to:
FILE "Suikoden II Rebalanced v1.2.bin" BINARY

Preserve all original TRACK and INDEX lines. Open that copied CUE in your
emulator. A new game is recommended for the complete rebalance.

v1.2 BIN SHA-256:
6202e1b7ace94d75f2cce162e5391bbf8ccc6720c484fe98df3b6984904cfabc

Patch SHA-256:
f079d16f488216e25c3080c91f53d6a513e5ad765d2a44ae30fdbfe06b800db8

UPGRADING AND EXISTING SAVES

Apply v1.2 to your clean original, not to a v1.0/v1.1 patched image. This is a
complete vanilla-to-v1.2 patch, so no earlier patch is required.

Vanilla saves store their own growth/rune-slot table. Disc patching does not
migrate that table or retroactively change earned stats. Save-migration tools
are not included in this three-file package. A new game receives the complete
configuration. Correctly migrated v0.99/v1.0/v1.1 cards already have the matching
growth/slot table and need no new table migration for v1.2.

Use normal in-game saves. Restart the emulator on the v1.2 CUE to refresh
cached menu data. Do not carry emulator save states across versions.

VERIFICATION AND LIMITS

The clean-original xdelta encodes identically twice and decodes to the exact
v1.2 BIN hash. A whole-disc comparison against v1.1 confirms five guarded local
instructions changed: 10 payload bytes plus 220 CD-checksum bytes, across five
sectors. Every other raw sector, file length and disc-layout entry is identical.
All previous 1280 guarded edits remain; the complete ledger now has 1285 edits.

Controlled Linux MIPS tests execute the actual five deadline callbacks, with
only the allocator stubbed. 40 original boundary cases and 340 candidate time cases
verify cutoff semantics, late acceptance, unchanged clock/story guard bytes,
stack, preserved registers and the actual callback result ABI. These controlled
CPU tests are separate from PS1 gameplay.

Native Linux PCSX-Redux compared the same normally prepared downloaded save
past 15 hours: v1.1 rejected the Radat deadline, while v1.2 allowed the event to
progress. Normal controller input and private card copies were used; no guest
clock, story, party or stat edits, cheats or state loads were used. Source
history before download is unknown. This is a Radat checkpoint comparison,
not an uninterrupted playthrough of all Clive scenes on v1.2. A normal
post-event save was cold-loaded on v1.2 and retained the verified quest progress.

Earlier v1.1 checks cover selected battles, a 108-star Suikoden I import with
patched-profile preservation, and the later living Gremio/Tir Banner intro.
The rest of Tir's rescue/recruitment/combat test remains deferred. A full
campaign, every recruitment/loadout/Unite variant, endings and real hardware
remain unverified. The spelling pass is not a complete retranslation.

Full GS2 Bug Fix Patch v2.02.078 compatibility

The full default bug-fix profile was combined with v1.2 and tested in native
Linux PCSX-Redux: overdue Radat progression, ordinary post-event save and fresh
cold reload, retained quest flags/party, field movement, and Shin using Spider
Slay twice in one battle followed by victory and return to the field.

The private Linux-built combination applies all 32 default options (35 PPF
files plus the Godspeed/Minotaur/Circlet text passes), keeping Kindness Penalty.
Independent checks verify all 1090 file payloads, all 17 disc-address tables,
changed-sector checksums and all 1285 Rebalanced edits. The standalone patch
and balance numbers are unchanged. The full external bug-fix pack is optional
and is not bundled in Rebalanced; only our existing Kindness repair is included.

The combined image was built directly in Linux from the shipped patch data.
The upstream Windows GUI/CD builder could not run in this WSL1 environment,
so its execution is not certified. These are bounded combined-image checks;
not every upstream fix, option combination or full campaign was playtested.

Apply clean original -> Rebalanced -> upstream bug-fix tool, keeping Kindness
set to Penalty. Our xdelta requires the clean original and cannot be applied
to an already bug-fix-patched image. No Penalty intentionally overrides our
Kindness behavior. Keep image/save backups and use normal saves, not old states.
Upstream: https://github.com/pyriell/gs2-bugfixes
Details: https://github.com/RetchERez/Suikoden-II-Rebalanced/blob/v1.2-compatibility/COMPATIBILITY.md

For a bug report include emulator/version, location, party/levels, equipment,
runes, reproduction steps, patched BIN hash and save origin.

CREDITS AND DISTRIBUTION

Additional thanks: Cloudstrife7894, Dyne

Rebalance by RetchERezzed. The signed negative-Kindness repair incorporates
Pyriel's published penalty-preserving fix from gs2-bugfixes, commit
e657ecafebdad2ed4c8e9031a8ab982fd506bf58, patch/NA/src/kindness_rune.asm:
https://github.com/pyriell/gs2-bugfixes

Only the patch and these two documents are included. No game image, BIOS,
emulator, downloaded save or save state is distributed. Keep your generated
game image and private test assets private.
