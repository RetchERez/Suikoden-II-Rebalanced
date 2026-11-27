SUIKODEN II: REBALANCED v1.3
By RetchERezzed


ABOUT

A combat rebalance for the original USA PlayStation release, intended to make
more party choices useful while keeping ordinary play and resource management
relevant. Selected growth improvements cover 22 characters. Earlier head rune
slots, personal-rune adjustments and stronger coefficients for 14 Unite families
are retained alongside the documented Kindness, text, Potch and HQ repairs.
README_EVERY_CHANGE.txt records exact vanilla-to-patch changes.

NEW IN v1.3

Four existing music streams now have matching CD-XA file-number metadata:
Annallee Song, War Theme 1, War Theme 3 and Chant Song. The audio samples and
executable song filters are unchanged. The 4,243 sector repairs match the
corresponding canonical Music Fixes bytes from Pyriel's project.

Meg's Trick returns to 300% once per battle, and Millie's Groundhog to 200%
once per battle. Their stronger opening attacks complement later spells or
support. This trades away v1.2's unlimited weaker attacks; it is not a universal
sustained-damage increase. Shin's Spider Slay remains repeatable at 200%.
Meg/Millie's growth improvements and Millie's head unlock at 30 are retained.
All 60 restored Trick description copies correct the original Winup typo and
now say "3x DMG 1 time only".

The representative save-based review covers Mist Shade, Sword and Abomination, alongside qualified earlier encounter evidence. The target remains moderate challenge, varied parties and no extra grinding. No enemy or boss numerical/AI changes were made. Abomination was a difficult, healing-intensive win; source equipment, empty rune slots, legacy growth tables and a conservative player policy limit the inference. These results support retaining the current numbers for public testing; they do not certify moderate difficulty across the whole game or every party.

RETAINED FROM v1.2 AND v1.1

Clive's five elapsed-time deadlines remain removed at Lakewest, Forest Village,
Rockaxe, Radat and Sajah. The normal game clock, story prerequisites, initial
Muse encounter and one-time flags remain. Already failed quest flags are not
reset and failed saves are not automatically recovered.

The reviewed spelling, Mercenary Soldier labels, rune help, capitalized/spaced
Potch and money-window clipping repairs are retained. This is not a full
retranslation. The signed negative-Kindness fix retains its normal penalty.
Two verified Headquarters exit-preload repairs are retained.

PACKAGE CONTENTS

  Suikoden-II-Rebalanced-v1.3.xdelta
  README.txt
  README_EVERY_CHANGE.txt

No ROM, BIOS, emulator, save or game audio is distributed

REQUIRED ORIGINAL

Use your own legally sourced untouched USA SLUS-00958 single-track
MODE2/2352 BIN/CUE. The BIN must be 513907296 bytes and match this SHA-256:

acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472

Keep a clean original and backups of your saves. Other regions/revisions,
prepatched images and compressed CHDs are unsupported patch inputs.

INSTALLATION

Obtain xdelta3 from its upstream project:
https://github.com/jmacd/xdelta/releases
The recorded Linux encoder is version 3.0.11; no application header is embedded.

Check the original BIN's SHA-256 before patching
Windows PowerShell: Get-FileHash -Algorithm SHA256 "original.bin"
Linux: sha256sum "original.bin"

Apply the patch using a NEW output filename

Linux:
xdelta3 -d -s "original.bin" "Suikoden-II-Rebalanced-v1.3.xdelta" "Suikoden II Rebalanced v1.3.bin"

Windows PowerShell with xdelta3.exe beside the patch:
.\xdelta3.exe -d -s "original.bin" "Suikoden-II-Rebalanced-v1.3.xdelta" "Suikoden II Rebalanced v1.3.bin"

Patched BIN SHA-256:
5a5d01a66dd4b105463ee63201c9b193ddcb9bb53d8fe591cab582dca5a33120

Patch SHA-256:
41c1b33ab8a6e760402729e79dabe138764daa0a560420c3efcac19b8018e2b3

Copy the original CUE to a separate file beside the new BIN. In that copied
CUE only, change its FILE entry to:
FILE "Suikoden II Rebalanced v1.3.bin" BINARY

Keep the original TRACK and INDEX lines and launch the copied CUE
Do not replace or patch over your clean original

EXISTING SAVES AND UPGRADES

Apply this complete patch to the clean original, including when upgrading.
Do not apply it over v1.0, v1.1 or v1.2.

A new game is recommended for the complete rebalance. Vanilla saves store
their own growth/rune-slot table. Disc patching does not migrate that table
or retroactively replace earned stats. Previously correctly migrated
Rebalanced cards already have the matching growth/slot configuration; v1.3
does not add another growth-table change. Migration tools are not in this ZIP.

Restart the emulator on the new CUE and use ordinary in-game saves
Do not carry emulator save states across versions

VERIFICATION AND LIMITS

The patch encodes identically twice and decodes to the exact BIN
hash. The 1,215 logical edits and 4,243 XA sector repairs are guarded by original
hashes and bytes. The whole-disc audit verifies checksums, unchanged layout
and every unlisted raw byte. The separate ledger lists all exact changes.

Native Linux PCSX-Redux observed actual Meg 300% and Millie 200% first-use
damage, same-battle menu blocking and new-battle reset. Shin remained able
to execute Spider Slay twice. Both first fights reached victory, rewards and
field movement. Damage observations were checked against actual complete
helper code, callsites and runtime inputs. The later candidate02 change is
only 60 Trick descriptions plus derived CD checksums; an independent review
proves all battle code and rune metadata match the mechanics-tested image.

The offensive resource planner checks shared finite MP and reserve budgets;
eight tests and independent exhaustive comparisons pass. Its 672 comparisons
are bounded sensitivities, not battle winrates or a full PS1 simulation.
The enemy selector audit traces real fixed 0-99 selection and retries and documents
old-model limitations. More Monte Carlo samples do not resolve missing AI,
targeting, status, acquisition, phase or campaign assumptions.

Music filters and all four complete decoded nonzero streams are verified.
An identical 287-command replay from the same ordinary save verified Annallee's
actual first song in Linux: a matched 30-second quiet window contains song PCM
on v1.3 and exact silence on vanilla, with the same field/story/script states.
The waveform correlates 0.99036 with the decoded Annallee asset, and both runs
reach her post-song dialogue. This tests her first actual scene; the other
three repaired tracks have routing and decode verification.
Sword was beaten in eight rounds with all six alive, using seven Medicine
charges and finite MP, followed by story/field continuation and an ordinary
save. Its conservative policy is not a minimum-resource benchmark, and the
legacy save retains retail cached growth profiles with unknown prior history.
Abomination was beaten in eight planned rounds with all six alive, using 16 Medicine charges and finite MP. Two survivors ended at 9 and 15 HP. Reward, post-boss dialogue and ordinary field movement were verified. An earlier policy lost; the retry differed in starting HP, resources and RNG, so this is not a controlled policy-only comparison. No extra training or equipment purchases were used. Four weapons were level 5; source gear, empty rune slots, legacy retail growth tables and conservative healing limit the difficulty assessment. These are observed costs, not minimum required resources or a whole-game balance certificate.

Actual Abomination MP costs: Riou 6 L1 + 1 L2 + 1 L3; Nanami 2 L1; Kahn 6 L1 + 1 L3. Medicine charges spent: Freed Y 5, Viktor 5, Nanami 6. Native Yell revival was not demonstrated because no KO occurred in the successful run. The ordinary post-inn save was cold-loaded; no post-Abomination save/reload test is claimed.

Healing spell descriptions list base powers. Native code and neutral-affinity, unboosted Riou MAGIC 77 inputs derive Great Blessing 147 and Battle Oath 377 before HP caps (base 70/300 plus MAGIC). This is a code/input derivation, not an isolated per-action heal measurement from whole-round HP snapshots.

Earlier checks include selected save-based fights, a 108-star Suikoden I import
and the living Gremio/Tir Banner introduction. The remaining Tir quest, every
recruitment/loadout/Unite variant, a full campaign, endings and real hardware
are not certified. Downloaded saves have unknown prior training/editing history.

Full GS2 Bug Fix Patch v2.02.078 compatibility

The optional full default profile was composed from the actual upstream patch
data in Linux. Independent candidate02 checks verify all 1,090 file payloads,
all 17 disc-address tables, all 35 PPFs, normal sector metadata/checksums and
retention of all 1,215 logical Rebalanced edits.

A combined mechanics candidate completed an overdue Radat event and ordinary
save, preserving quest flags and party. The final corrected combined image
also cold-loaded that same save, retained flags/party and allowed field movement.
Its campaign save blocks stayed byte-identical. All native inputs and RAM/card
results were independently reviewed. Earlier host cleanup timeouts are retained
in the private QA log; the final cold-load harness completed and reaped its
controlled test process. The 60-description difference between the longer
mechanics trial and corrected image is independently byte-audited.

The upstream Windows installer was not executed successfully in this WSL
environment. This verifies Linux data composition and bounded native routes,
not every external fix, option combination or full campaign.

The full pack remains optional and external. Rebalanced includes only its
documented standalone Kindness repair and the four canonical music repairs.
Use clean original -> Rebalanced -> optional upstream tool, keeping Kindness
set to Penalty. No Penalty intentionally overrides that behavior. The
Rebalanced xdelta requires the clean original and cannot accept an already
bugfix-patched image. Keep backups and use normal saves.
Upstream: https://github.com/pyriell/gs2-bugfixes

SPECIAL THANKS

Pyriel for the original penalty-preserving Kindness Rune fix and the canonical
Music Fixes reference used to verify the four stream repairs
https://github.com/pyriell/gs2-bugfixes

Cloudstrife7894 and Dyne
Community save authors whose checkpoints enabled the documented bounded tests

BUG REPORTS

Include emulator/version, location, party/levels, equipment, runes, reproduction
steps, patched BIN hash, save origin and whether the optional bugfix pack is used
