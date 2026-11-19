SUIKODEN II: REBALANCED v1.2
EVERY CHANGE FROM UNMODIFIED USA SLUS-00958
By RetchERezzed

Original BIN SHA-256: acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472
v1.2 BIN SHA-256:    6202e1b7ace94d75f2cce162e5391bbf8ccc6720c484fe98df3b6984904cfabc
xdelta SHA-256:       f079d16f488216e25c3080c91f53d6a513e5ad765d2a44ae30fdbfe06b800db8

All 1285 guarded edits across 217 game files are listed below.
There are 14484 differing payload bytes in 613 raw CD sectors.
Including regenerated EDC/ECC, 82609 raw bytes differ from vanilla.
Every untouched raw sector is identical. File lengths and disc layout stay unchanged.
Binary changes do not certify every possible gameplay outcome.

1. CHARACTER GROWTH - 48 LOGICAL FIELDS ACROSS 22 CHARACTERS
Numeric growth-rank codes describe future native growth; they are not
retroactive stat increases or promises about final stats. ALL and KOTEI
store mirrored packed nibbles. Exact physical edits are enumerated below.
Reference letter grades follow the handoff. Native rank codes and
measured growth remain authoritative.
Character / ID | Stat | retail code (grade) -> Final code (grade)
Shin / 15 | SPD | 4 (E) -> 5 (D)
Shin / 15 | HP | 4 (E) -> 5 (D)
Tomo / 17 | PROT | 4 (E) -> 5 (D)
Tomo / 17 | HP | 4 (E) -> 5 (D)
Bolgan / 21 | DEX | 2 (G) -> 3 (F)
Bolgan / 21 | SPD | 1 (H) -> 3 (F)
Tuta / 22 | MAG | 2 (G) -> 3 (F)
Tuta / 22 | HP | 0 (I) -> 2 (G)
Hanna / 23 | STR | 5 (D) -> 6 (C)
Hanna / 23 | SPD | 3 (F) -> 4 (E)
Millie / 24 | MAG | 4 (E) -> 5 (D) (KOTEI retail code 3)
Millie / 24 | HP | 3 (F) -> 4 (E)
Gengen / 28 | STR | 4 (E) -> 5 (D)
Gengen / 28 | PROT | 4 (E) -> 5 (D)
Gengen / 28 | HP | 4 (E) -> 5 (D)
Gabocha / 29 | STR | 3 (F) -> 4 (E)
Gabocha / 29 | SPD | 5 (D) -> 6 (C)
Gabocha / 29 | HP | 3 (F) -> 4 (E)
Shilo / 31 | STR | 4 (E) -> 5 (D)
Shilo / 31 | SPD | 4 (E) -> 5 (D)
Freed Y / 35 | STR | 4 (E) -> 5 (D)
Freed Y / 35 | HP | 4 (E) -> 5 (D)
Meg / 41 | MAG | 3 (F) -> 5 (D)
Meg / 41 | HP | 3 (F) -> 4 (E)
Gadget / 42 | STR | 4 (E) -> 5 (D)
Gadget / 42 | HP | 4 (E) -> 5 (D)
Genshu / 47 | STR | 5 (D) -> 6 (C)
Genshu / 47 | SPD | 5 (D) -> 6 (C)
Genshu / 47 | HP | 4 (E) -> 5 (D)
Tsai / 52 | STR | 4 (E) -> 5 (D)
Tsai / 52 | SPD | 4 (E) -> 5 (D)
Sid / 56 | STR | 4 (E) -> 5 (D)
Sid / 56 | MAG | 3 (F) -> 4 (E)
Yoshino / 57 | MAG | 4 (E) -> 5 (D)
Yoshino / 57 | HP | 4 (E) -> 5 (D)
Koyu / 59 | STR | 3 (F) -> 4 (E)
Koyu / 59 | PROT | 3 (F) -> 4 (E)
Lo Wen / 60 | STR | 5 (D) -> 6 (C)
Lo Wen / 60 | DEX | 4 (E) -> 5 (D)
Vincent / 64 | MAG | 3 (F) -> 4 (E)
Vincent / 64 | HP | 4 (E) -> 5 (D)
Simone / 65 | MAG | 4 (E) -> 5 (D)
Simone / 65 | HP | 4 (E) -> 5 (D)
Hai Yo / 66 | STR | 3 (F) -> 4 (E)
Hai Yo / 66 | DEX | 3 (F) -> 4 (E)
Hoi / 71 | STR | 3 (F) -> 4 (E)
Hoi / 71 | PROT | 3 (F) -> 4 (E)
Hoi / 71 | HP | 3 (F) -> 4 (E)

2. HEAD RUNE SLOT UNLOCKS
Tuta: Head rune slot level threshold: 35 -> 25.
Millie: Head rune slot level threshold: 35 -> 30.
Hai Yo: Head rune slot level threshold: 65 -> 45.
Hoi: Head rune slot level threshold: 80 -> 35.

3. PERSONAL RUNE DAMAGE AND REPEATABILITY
Trick (spell 79, rune 39) coefficient: 300% -> 175%.
Mayfly (spell 82, rune 42) coefficient: 100% -> 125%.
Swallow (spell 83, rune 43) coefficient: 100% -> 150%.
Groundhog (spell 85, rune 45) coefficient: 200% -> 150%.
Spider Slay (spell 95, rune 51) coefficient: 300% -> 200%.
Trick, Groundhog and Spider Slay each ignore their own once-per-battle
used-bit availability test in both battle overlays. Their retail used-bit
writers and other actor/status/target conditions are retained. Six exact
instruction edits and the three updated descriptions appear below.

4. UNITE COEFFICIENTS AND DESCRIPTIONS
The same changed records are mirrored in FST and SEC battle overlays.
Percentages are record coefficients; physical DEF and special action
branches affect actual damage. Swordsman uses the defended damage of
each participant before its coefficient. Retail 100 Kobold remains 300%;
its stale description is corrected. Cup of the Oath Bandit branches
change 200% to 225% at three holder cases in each overlay.
Bandit Attack: 150% -> 175% (records 42)
Beastmaster Attack: 150% -> 175% (records 47, 48, 49, 50)
Bow Attack: 50% -> 75% (records 12, 13, 14)
Bow Wow Attack: 150% -> 175% (records 8, 9)
Circus Attack: 200% -> 225% (records 27)
Copycat Attack: 100% -> 150% (records 25)
Dad & Daughter Attack: 100% -> 125% (records 18)
Double Kraken Attack: 100% -> 125% (records 23)
Kobold Attack: 100% -> 125% (records 3)
Narcissists Attack: 50% -> 75% (records 16)
Pretty Girl Attack: 50% -> 75% (records 38, 39)
Swordsman Attack: 50% -> 75% (records 24)
Tackle Attack: 75% -> 100% (records 35)
Winger Attack: 150% -> 175% (records 17)

5. KINDNESS RUNE SIGNED-RATING FIX
One executable instruction is replaced using Pyriel's published fix.
The unsigned mask caused negative ratings to wrap and reach 999 ATK.
Final preserves the signed negative rating and its attack penalty.
The separate no-negative-penalty alternative was not selected.
Attribution: Pyriel, gs2-bugfixes, commit
e657ecafebdad2ed4c8e9031a8ab982fd506bf58, patch/NA/src/kindness_rune.asm
https://github.com/pyriell/gs2-bugfixes

6. NPC LABEL SPELLING
Exactly 64 copies of 'Mercenary Solider' become 'Mercenary Soldier'.
The two adjacent glyphs exchange positions; each label keeps its byte
length and boundaries. This is a narrow spelling correction. A broader
translation rewrite is not implemented.

7. HEADQUARTERS EXIT PRELOAD FIX
Two field-data bytes, one each in VK01 and VK34, extend their shared
background preloads over the two
exit rows that a normal lower-wall approach could bypass. The retail
failure loads cached bar textures through the smaller world-map decoder
buffer and overwrites live collision data. The preload now runs first;
the existing exit waits for its normal completion. All three active
HQ scenes in each resource share its condition. Native regression scope and
remaining limits are recorded in final_closure_field_fault.json and
final_validation_hq_stages.json.
Combat numbers, texture/allocator code, neighboring preloads, exit
destination and story flags are unchanged.


8. NEW IN v1.1 - MENU TEXT AND REVIEWED SPELLING
The previous v1.0 updated the MAGI spell descriptions but left separate
rune-selection descriptions at vanilla wording. v1.1 changes all 177
identified named copies in 59 resources, covering field/shop/battle contexts.
Battle menus also have their own pointer-defined help strings. All ten
FST/SEC copies for the five damage-adjusted personal runes are corrected.
The spelling pass additionally fixes reviewed mistakes in dialogue,
equipment/rune/war descriptions, weapon labels and other menu text.
Names, dialect, singing and stammering are retained after contextual review.
Currency name: potch -> Potch in 380 references across 107 readable resources,
including menus, rewards, shops, spending and dialogue. Another 27 references
already used Potch and remain unchanged, giving 407 consistent references.
25 standalone currency labels also gain a leading space by using existing
null padding, so an amount is visibly separated from Potch. Slots and pointers
stay the same size; inline dialogue already has a space or line break.
30 verified money-window widths expand one text cell to fit the added space,
including 16-to-17-cell To go displays with their additional five-cell prefix.
Only the guarded width fields change; shop prices and currency values do not.
Two Chinchirorin To go windows also shift eight pixels left to keep their
expanded frames from overlapping the adjacent money display.
44 later full-size resize calls also use the expanded width, preventing shop
menus from restoring the old clipping rectangle after construction.
Some longer corrections use minor nearby wording or redundant whitespace
to preserve exact byte lengths. Readable before/after text is recorded below.
Trick: Windup Moll ATK 1 time -> 1.75x DMG Repeatable
Groundhog: 2 x damage 1 time only -> 1.5x DMG Repeatable
Spider Slay: 3 x damage 1 time only -> 2x DMG Repeatable
Decoded original wording may be shortened by the game UI. Exact bytes below
are authoritative. Rune IDs, links, flags, coefficients and combat program logic
stay unchanged. Only documented text/UI-layout fields and CD checksums change.
All 1071 readable Form1 ISO resources were scanned for these named records
and changed Unite descriptions. No stale named copy remains in that scope.
19 non-Form1 audio/video resources were excluded from the text scan.

9. EXACT MANIFEST EDITS - ALL 1285 ENTRIES

001. /CDROM/280_GAME/ALL.BIN +0x210 (528) - Shin SPD
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

002. /CDROM/280_GAME/ALL.BIN +0x211 (529) - Shin HP
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

003. /CDROM/280_GAME/ALL.BIN +0x233 (563) - Tomo PROT
     RETAIL HEX: 44
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

004. /CDROM/280_GAME/ALL.BIN +0x235 (565) - Tomo HP
     RETAIL HEX: 44
     v1.2 HEX:   45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

005. /CDROM/280_GAME/ALL.BIN +0x27C (636) - Bolgan DEX, Bolgan SPD
     RETAIL HEX: 21
     v1.2 HEX:   33
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

006. /CDROM/280_GAME/ALL.BIN +0x28C (652) - Tuta MAG
     RETAIL HEX: 22
     v1.2 HEX:   23
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

007. /CDROM/280_GAME/ALL.BIN +0x28F (655) - Tuta HP
     RETAIL HEX: 50
     v1.2 HEX:   52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

008. /CDROM/280_GAME/ALL.BIN +0x29E (670) - Hanna STR
     RETAIL HEX: 52
     v1.2 HEX:   62
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

009. /CDROM/280_GAME/ALL.BIN +0x2A0 (672) - Hanna SPD
     RETAIL HEX: 53
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

010. /CDROM/280_GAME/ALL.BIN +0x2B0 (688) - Millie MAG
     RETAIL HEX: 24
     v1.2 HEX:   25
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

011. /CDROM/280_GAME/ALL.BIN +0x2B3 (691) - Millie HP
     RETAIL HEX: 73
     v1.2 HEX:   74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

012. /CDROM/280_GAME/ALL.BIN +0x2F8 (760) - Gengen STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

013. /CDROM/280_GAME/ALL.BIN +0x2F9 (761) - Gengen PROT
     RETAIL HEX: 42
     v1.2 HEX:   52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

014. /CDROM/280_GAME/ALL.BIN +0x2FB (763) - Gengen HP
     RETAIL HEX: 64
     v1.2 HEX:   65
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

015. /CDROM/280_GAME/ALL.BIN +0x30A (778) - Gabocha STR
     RETAIL HEX: 33
     v1.2 HEX:   43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

016. /CDROM/280_GAME/ALL.BIN +0x30C (780) - Gabocha SPD
     RETAIL HEX: 65
     v1.2 HEX:   66
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

017. /CDROM/280_GAME/ALL.BIN +0x30D (781) - Gabocha HP
     RETAIL HEX: 63
     v1.2 HEX:   64
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

018. /CDROM/280_GAME/ALL.BIN +0x32E (814) - Shilo STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

019. /CDROM/280_GAME/ALL.BIN +0x330 (816) - Shilo SPD
     RETAIL HEX: 84
     v1.2 HEX:   85
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

020. /CDROM/280_GAME/ALL.BIN +0x376 (886) - Freed Y STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

021. /CDROM/280_GAME/ALL.BIN +0x379 (889) - Freed Y HP
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

022. /CDROM/280_GAME/ALL.BIN +0x3E2 (994) - Meg MAG
     RETAIL HEX: 33
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

023. /CDROM/280_GAME/ALL.BIN +0x3E5 (997) - Meg HP
     RETAIL HEX: 73
     v1.2 HEX:   74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

024. /CDROM/280_GAME/ALL.BIN +0x3F4 (1012) - Gadget STR
     RETAIL HEX: 40
     v1.2 HEX:   50
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

025. /CDROM/280_GAME/ALL.BIN +0x3F7 (1015) - Gadget HP
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

026. /CDROM/280_GAME/ALL.BIN +0x44E (1102) - Genshu STR
     RETAIL HEX: 53
     v1.2 HEX:   63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

027. /CDROM/280_GAME/ALL.BIN +0x450 (1104) - Genshu SPD
     RETAIL HEX: 55
     v1.2 HEX:   56
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

028. /CDROM/280_GAME/ALL.BIN +0x451 (1105) - Genshu HP
     RETAIL HEX: 54
     v1.2 HEX:   55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

029. /CDROM/280_GAME/ALL.BIN +0x4A8 (1192) - Tsai STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

030. /CDROM/280_GAME/ALL.BIN +0x4AA (1194) - Tsai SPD
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

031. /CDROM/280_GAME/ALL.BIN +0x4F0 (1264) - Sid STR, Sid MAG
     RETAIL HEX: 43
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

032. /CDROM/280_GAME/ALL.BIN +0x502 (1282) - Yoshino MAG
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

033. /CDROM/280_GAME/ALL.BIN +0x505 (1285) - Yoshino HP
     RETAIL HEX: 54
     v1.2 HEX:   55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

034. /CDROM/280_GAME/ALL.BIN +0x526 (1318) - Koyu STR
     RETAIL HEX: 33
     v1.2 HEX:   43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

035. /CDROM/280_GAME/ALL.BIN +0x527 (1319) - Koyu PROT
     RETAIL HEX: 35
     v1.2 HEX:   45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

036. /CDROM/280_GAME/ALL.BIN +0x538 (1336) - Lo Wen STR
     RETAIL HEX: 53
     v1.2 HEX:   63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

037. /CDROM/280_GAME/ALL.BIN +0x53A (1338) - Lo Wen DEX
     RETAIL HEX: 44
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

038. /CDROM/280_GAME/ALL.BIN +0x580 (1408) - Vincent MAG
     RETAIL HEX: 43
     v1.2 HEX:   44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

039. /CDROM/280_GAME/ALL.BIN +0x583 (1411) - Vincent HP
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

040. /CDROM/280_GAME/ALL.BIN +0x592 (1426) - Simone MAG
     RETAIL HEX: 44
     v1.2 HEX:   45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

041. /CDROM/280_GAME/ALL.BIN +0x595 (1429) - Simone HP
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

042. /CDROM/280_GAME/ALL.BIN +0x5A4 (1444) - Hai Yo STR
     RETAIL HEX: 33
     v1.2 HEX:   43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

043. /CDROM/280_GAME/ALL.BIN +0x5A6 (1446) - Hai Yo DEX
     RETAIL HEX: 34
     v1.2 HEX:   44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

044. /CDROM/280_GAME/ALL.BIN +0x5FE (1534) - Hoi STR
     RETAIL HEX: 32
     v1.2 HEX:   42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

045. /CDROM/280_GAME/ALL.BIN +0x5FF (1535) - Hoi PROT
     RETAIL HEX: 32
     v1.2 HEX:   42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

046. /CDROM/280_GAME/ALL.BIN +0x601 (1537) - Hoi HP
     RETAIL HEX: 73
     v1.2 HEX:   74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

047. /CDROM/280_GAME/KOTEI.BIN +0x110 (272) - Shin SPD
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

048. /CDROM/280_GAME/KOTEI.BIN +0x111 (273) - Shin HP
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

049. /CDROM/280_GAME/KOTEI.BIN +0x133 (307) - Tomo PROT
     RETAIL HEX: 44
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

050. /CDROM/280_GAME/KOTEI.BIN +0x135 (309) - Tomo HP
     RETAIL HEX: 44
     v1.2 HEX:   45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

051. /CDROM/280_GAME/KOTEI.BIN +0x17C (380) - Bolgan DEX, Bolgan SPD
     RETAIL HEX: 21
     v1.2 HEX:   33
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

052. /CDROM/280_GAME/KOTEI.BIN +0x18C (396) - Tuta MAG
     RETAIL HEX: 22
     v1.2 HEX:   23
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

053. /CDROM/280_GAME/KOTEI.BIN +0x18F (399) - Tuta HP
     RETAIL HEX: 50
     v1.2 HEX:   52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

054. /CDROM/280_GAME/KOTEI.BIN +0x19E (414) - Hanna STR
     RETAIL HEX: 52
     v1.2 HEX:   62
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

055. /CDROM/280_GAME/KOTEI.BIN +0x1A0 (416) - Hanna SPD
     RETAIL HEX: 53
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

056. /CDROM/280_GAME/KOTEI.BIN +0x1B0 (432) - Millie MAG
     RETAIL HEX: 23
     v1.2 HEX:   25
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

057. /CDROM/280_GAME/KOTEI.BIN +0x1B3 (435) - Millie HP
     RETAIL HEX: 73
     v1.2 HEX:   74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

058. /CDROM/280_GAME/KOTEI.BIN +0x1F8 (504) - Gengen STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

059. /CDROM/280_GAME/KOTEI.BIN +0x1F9 (505) - Gengen PROT
     RETAIL HEX: 42
     v1.2 HEX:   52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

060. /CDROM/280_GAME/KOTEI.BIN +0x1FB (507) - Gengen HP
     RETAIL HEX: 64
     v1.2 HEX:   65
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

061. /CDROM/280_GAME/KOTEI.BIN +0x20A (522) - Gabocha STR
     RETAIL HEX: 33
     v1.2 HEX:   43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

062. /CDROM/280_GAME/KOTEI.BIN +0x20C (524) - Gabocha SPD
     RETAIL HEX: 65
     v1.2 HEX:   66
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

063. /CDROM/280_GAME/KOTEI.BIN +0x20D (525) - Gabocha HP
     RETAIL HEX: 63
     v1.2 HEX:   64
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

064. /CDROM/280_GAME/KOTEI.BIN +0x22E (558) - Shilo STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

065. /CDROM/280_GAME/KOTEI.BIN +0x230 (560) - Shilo SPD
     RETAIL HEX: 84
     v1.2 HEX:   85
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

066. /CDROM/280_GAME/KOTEI.BIN +0x276 (630) - Freed Y STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

067. /CDROM/280_GAME/KOTEI.BIN +0x279 (633) - Freed Y HP
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

068. /CDROM/280_GAME/KOTEI.BIN +0x2E2 (738) - Meg MAG
     RETAIL HEX: 33
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

069. /CDROM/280_GAME/KOTEI.BIN +0x2E5 (741) - Meg HP
     RETAIL HEX: 73
     v1.2 HEX:   74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

070. /CDROM/280_GAME/KOTEI.BIN +0x2F4 (756) - Gadget STR
     RETAIL HEX: 40
     v1.2 HEX:   50
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

071. /CDROM/280_GAME/KOTEI.BIN +0x2F7 (759) - Gadget HP
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

072. /CDROM/280_GAME/KOTEI.BIN +0x34E (846) - Genshu STR
     RETAIL HEX: 53
     v1.2 HEX:   63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

073. /CDROM/280_GAME/KOTEI.BIN +0x350 (848) - Genshu SPD
     RETAIL HEX: 55
     v1.2 HEX:   56
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

074. /CDROM/280_GAME/KOTEI.BIN +0x351 (849) - Genshu HP
     RETAIL HEX: 54
     v1.2 HEX:   55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

075. /CDROM/280_GAME/KOTEI.BIN +0x3A8 (936) - Tsai STR
     RETAIL HEX: 43
     v1.2 HEX:   53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

076. /CDROM/280_GAME/KOTEI.BIN +0x3AA (938) - Tsai SPD
     RETAIL HEX: 74
     v1.2 HEX:   75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

077. /CDROM/280_GAME/KOTEI.BIN +0x3F0 (1008) - Sid STR, Sid MAG
     RETAIL HEX: 43
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

078. /CDROM/280_GAME/KOTEI.BIN +0x402 (1026) - Yoshino MAG
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

079. /CDROM/280_GAME/KOTEI.BIN +0x405 (1029) - Yoshino HP
     RETAIL HEX: 54
     v1.2 HEX:   55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

080. /CDROM/280_GAME/KOTEI.BIN +0x426 (1062) - Koyu STR
     RETAIL HEX: 33
     v1.2 HEX:   43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

081. /CDROM/280_GAME/KOTEI.BIN +0x427 (1063) - Koyu PROT
     RETAIL HEX: 35
     v1.2 HEX:   45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

082. /CDROM/280_GAME/KOTEI.BIN +0x438 (1080) - Lo Wen STR
     RETAIL HEX: 53
     v1.2 HEX:   63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

083. /CDROM/280_GAME/KOTEI.BIN +0x43A (1082) - Lo Wen DEX
     RETAIL HEX: 44
     v1.2 HEX:   54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

084. /CDROM/280_GAME/KOTEI.BIN +0x480 (1152) - Vincent MAG
     RETAIL HEX: 43
     v1.2 HEX:   44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

085. /CDROM/280_GAME/KOTEI.BIN +0x483 (1155) - Vincent HP
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

086. /CDROM/280_GAME/KOTEI.BIN +0x492 (1170) - Simone MAG
     RETAIL HEX: 44
     v1.2 HEX:   45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

087. /CDROM/280_GAME/KOTEI.BIN +0x495 (1173) - Simone HP
     RETAIL HEX: 34
     v1.2 HEX:   35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

088. /CDROM/280_GAME/KOTEI.BIN +0x4A4 (1188) - Hai Yo STR
     RETAIL HEX: 33
     v1.2 HEX:   43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

089. /CDROM/280_GAME/KOTEI.BIN +0x4A6 (1190) - Hai Yo DEX
     RETAIL HEX: 34
     v1.2 HEX:   44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

090. /CDROM/280_GAME/KOTEI.BIN +0x4FE (1278) - Hoi STR
     RETAIL HEX: 32
     v1.2 HEX:   42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

091. /CDROM/280_GAME/KOTEI.BIN +0x4FF (1279) - Hoi PROT
     RETAIL HEX: 32
     v1.2 HEX:   42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

092. /CDROM/280_GAME/KOTEI.BIN +0x501 (1281) - Hoi HP
     RETAIL HEX: 73
     v1.2 HEX:   74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

093. /CDROM/280_GAME/ALL.BIN +0x29A (666) - Tuta head unlock
     RETAIL HEX: 23
     v1.2 HEX:   19
     Meaning: Head rune slot level threshold: 35 -> 25.

094. /CDROM/280_GAME/ALL.BIN +0x2BE (702) - Millie head unlock
     RETAIL HEX: 23
     v1.2 HEX:   1E
     Meaning: Head rune slot level threshold: 35 -> 30.

095. /CDROM/280_GAME/ALL.BIN +0x5B2 (1458) - Hai Yo head unlock
     RETAIL HEX: 41
     v1.2 HEX:   2D
     Meaning: Head rune slot level threshold: 65 -> 45.

096. /CDROM/280_GAME/ALL.BIN +0x60C (1548) - Hoi head unlock
     RETAIL HEX: 50
     v1.2 HEX:   23
     Meaning: Head rune slot level threshold: 80 -> 35.

097. /CDROM/280_GAME/MAGI.BIN +0x13FC (5116) - Personal physical damage coefficient
     RETAIL HEX: 2C01
     v1.2 HEX:   AF00
     Meaning: Trick (spell 79, rune 39) coefficient: 300% -> 175%.

098. /CDROM/280_GAME/MAGI.BIN +0x14BC (5308) - Personal physical damage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Mayfly (spell 82, rune 42) coefficient: 100% -> 125%.

099. /CDROM/280_GAME/MAGI.BIN +0x14FC (5372) - Personal physical damage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   9600
     Meaning: Swallow (spell 83, rune 43) coefficient: 100% -> 150%.

100. /CDROM/280_GAME/MAGI.BIN +0x157C (5500) - Personal physical damage coefficient
     RETAIL HEX: C800
     v1.2 HEX:   9600
     Meaning: Groundhog (spell 85, rune 45) coefficient: 200% -> 150%.

101. /CDROM/280_GAME/MAGI.BIN +0x17FC (6140) - Personal physical damage coefficient
     RETAIL HEX: 2C01
     v1.2 HEX:   C800
     Meaning: Spider Slay (spell 95, rune 51) coefficient: 300% -> 200%.

102. /CDROM/280_GAME/MAGI.BIN +0x13D5 (5077) - Personal rune description
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Spell 79 menu text: 'Winup Doll ATK<65> 1 time' -> '1.75x DMG Repeatable'.

103. /CDROM/280_GAME/MAGI.BIN +0x1555 (5461) - Personal rune description
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Spell 85 menu text: '2 x damage 1 time only' -> '1.5x DMG Repeatable'.

104. /CDROM/280_GAME/MAGI.BIN +0x17D5 (6101) - Personal rune description
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Spell 95 menu text: '3 x damage 1 time only' -> '2x DMG Repeatable'.

105. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0xAE00 (44544) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 01004230
     v1.2 HEX:   00004230
     Meaning: Trick rune-specific used-bit availability test mask 0x1 -> 0x0 at guest 0x80035e00; used-bit writer and other gates unchanged.

106. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0xAE0C (44556) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 02004230
     v1.2 HEX:   00004230
     Meaning: Groundhog rune-specific used-bit availability test mask 0x2 -> 0x0 at guest 0x80035e0c; used-bit writer and other gates unchanged.

107. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0xAE50 (44624) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 04004230
     v1.2 HEX:   00004230
     Meaning: Spider Slay rune-specific used-bit availability test mask 0x4 -> 0x0 at guest 0x80035e50; used-bit writer and other gates unchanged.

108. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0xA5B8 (42424) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 01004230
     v1.2 HEX:   00004230
     Meaning: Trick rune-specific used-bit availability test mask 0x1 -> 0x0 at guest 0x800355b8; used-bit writer and other gates unchanged.

109. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0xA5C4 (42436) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 02004230
     v1.2 HEX:   00004230
     Meaning: Groundhog rune-specific used-bit availability test mask 0x2 -> 0x0 at guest 0x800355c4; used-bit writer and other gates unchanged.

110. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0xA608 (42504) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 04004230
     v1.2 HEX:   00004230
     Meaning: Spider Slay rune-specific used-bit availability test mask 0x4 -> 0x0 at guest 0x80035608; used-bit writer and other gates unchanged.

111. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2364C (144972) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Kobold Attack record ID 3; participants [28, 29]; coefficient 100% -> 125%.

112. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2361E (144926) - description
     RETAIL HEX: 991028103E4741102623661099103F10680E4111121F131811104F1E12111C111E131500
     v1.2 HEX:   99669A9D283E47411026236699103F10680E4111121F131811104F1E12111C111E131500
     Meaning: Kobold Attack record ID 3 menu text: '1 x DMG vs. 1 E <68> / Gabocha Unbalance' -> '1.25xDMG vs.1 E <68> / Gabocha Unbalance'.

113. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x237C8 (145352) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Bow Wow Attack record ID 8; participants [28, 26]; coefficient 150% -> 175%.

114. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2379A (145306) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 8 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

115. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23814 (145428) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Bow Wow Attack record ID 9; participants [29, 26]; coefficient 150% -> 175%.

116. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x237E6 (145382) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 9 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

117. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x238F8 (145656) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Bow Attack record ID 12; participants [30, 43]; coefficient 50% -> 75%.

118. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x238CA (145610) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 12 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

119. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23944 (145732) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Bow Attack record ID 13; participants [30, 67]; coefficient 50% -> 75%.

120. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23916 (145686) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 13 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

121. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23990 (145808) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Bow Attack record ID 14; participants [43, 67]; coefficient 50% -> 75%.

122. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23962 (145762) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 14 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

123. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A28 (145960) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Narcissists Attack record ID 16; participants [64, 65]; coefficient 50% -> 75%.

124. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x239FA (145914) - description
     RETAIL HEX: 98669D1028103E474110241F0E111C1C103F230000000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E474110241F0E111C1C103F2300000000000000000000000000000000
     Meaning: Narcissists Attack record ID 16 menu text: '0.5 x DMG to / all Es' -> '0.75 x DMG to / all Es'.

125. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A74 (146036) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Winger Attack record ID 17; participants [54, 56]; coefficient 150% -> 175%.

126. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A46 (145990) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A000000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A0000000000
     Meaning: Winger Attack record ID 17 menu text: '1.5 x DMG vs. 1 E / Poison <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Poison <69>30<94><6A>'.

127. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23AC0 (146112) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Dad & Daughter Attack record ID 18; participants [52, 17]; coefficient 100% -> 125%.

128. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A92 (146066) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     v1.2 HEX:   99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Dad & Daughter Attack record ID 18 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

129. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C3C (146492) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Double Kraken Attack record ID 23; participants [49, 74]; coefficient 100% -> 125%.

130. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C0E (146446) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     v1.2 HEX:   99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Double Kraken Attack record ID 23 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

131. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C88 (146568) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Swordsman Attack record ID 24; participants [15, 47]; coefficient 50% -> 75%.

132. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C5A (146522) - description
     RETAIL HEX: 98669D283E47411026236610111C1C103F230E4D251414151E101415112418109A989400
     v1.2 HEX:   98669F9D283E474110262366111C1C103F230E4D251414151E101415112418109A989400
     Meaning: Swordsman Attack record ID 24 menu text: '0.5xDMG vs. all Es / Sudden death 20<94>' -> '0.75xDMG vs.all Es / Sudden death 20<94>'.

133. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23CD4 (146644) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   9600
     Meaning: Copycat Attack record ID 25; participants [1, 71]; coefficient 100% -> 150%.

134. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23CA6 (146598) - description
     RETAIL HEX: 991028103E4741102623661099103F000000000000000000000000000000000000000000
     v1.2 HEX:   99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     Meaning: Copycat Attack record ID 25 menu text: '1 x DMG vs. 1 E' -> '1.5 x DMG vs. 1 E'.

135. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23D6C (146796) - percentage coefficient
     RETAIL HEX: C800
     v1.2 HEX:   E100
     Meaning: Circus Attack record ID 27; participants [19, 20, 21]; coefficient 200% -> 225%.

136. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23D3E (146750) - description
     RETAIL HEX: 9A1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500000000
     v1.2 HEX:   9A669A9D1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500
     Meaning: Circus Attack record ID 27 menu text: '2 x DMG vs. 1 E / Bolgan Unbalance' -> '2.25 x DMG vs. 1 E / Bolgan Unbalance'.

137. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23FCC (147404) - percentage coefficient
     RETAIL HEX: 4B00
     v1.2 HEX:   6400
     Meaning: Tackle Attack record ID 35; participants [23, 46]; coefficient 75% -> 100%.

138. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23F9E (147358) - description
     RETAIL HEX: 98669F9D1028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000
     v1.2 HEX:   991028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000000000
     Meaning: Tackle Attack record ID 35 menu text: '0.75 x DMG vs. / all Es Unbalance' -> '1 x DMG vs. / all Es Unbalance'.

139. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x240B0 (147632) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Pretty Girl Attack record ID 38; participants [8, 24, 41]; coefficient 50% -> 75%.

140. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x24082 (147586) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 38 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

141. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x240FC (147708) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Pretty Girl Attack record ID 39; participants [8, 83, 41]; coefficient 50% -> 75%.

142. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x240CE (147662) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 39 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

143. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2411A (147738) - description
     RETAIL HEX: 99283E47411026236610111C1C103F230E4111121F131811104F1E12111C111E13150000
     v1.2 HEX:   9B283E47411026236610111C1C103F230E3C1F2418104F1E12111C111E13150000000000
     Meaning: 100 Kobold Attack record ID 40 menu text: '1xDMG vs. all Es / Gabocha Unbalance' -> '3xDMG vs. all Es / Both Unbalance'.

144. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x241E0 (147936) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Bandit Attack record ID 42; participants [58, 59, 60]; coefficient 150% -> 175%.

145. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x241B2 (147890) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A0000
     Meaning: Bandit Attack record ID 42 menu text: '1.5 x DMG vs. 1 E / Knockdown <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Knockdown <69>30<94><6A>'.

146. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2435C (148316) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 47; participants [51, 49, 74]; coefficient 150% -> 175%.

147. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2432E (148270) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 47 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

148. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x243A8 (148392) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 48; participants [51, 49, 72]; coefficient 150% -> 175%.

149. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2437A (148346) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 48 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

150. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x243F4 (148468) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 49; participants [51, 49, 50]; coefficient 150% -> 175%.

151. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x243C6 (148422) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 49 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

152. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x24440 (148544) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 50; participants [51, 72, 50]; coefficient 150% -> 175%.

153. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x24412 (148498) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 50 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

154. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x1EC74 (126068) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     v1.2 HEX:   E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

155. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x1EC98 (126104) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     v1.2 HEX:   E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

156. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x1ECBC (126140) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     v1.2 HEX:   E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

157. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22E20 (142880) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Kobold Attack record ID 3; participants [28, 29]; coefficient 100% -> 125%.

158. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22DF2 (142834) - description
     RETAIL HEX: 991028103E4741102623661099103F10680E4111121F131811104F1E12111C111E131500
     v1.2 HEX:   99669A9D283E47411026236699103F10680E4111121F131811104F1E12111C111E131500
     Meaning: Kobold Attack record ID 3 menu text: '1 x DMG vs. 1 E <68> / Gabocha Unbalance' -> '1.25xDMG vs.1 E <68> / Gabocha Unbalance'.

159. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22F9C (143260) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Bow Wow Attack record ID 8; participants [28, 26]; coefficient 150% -> 175%.

160. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22F6E (143214) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 8 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

161. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22FE8 (143336) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Bow Wow Attack record ID 9; participants [29, 26]; coefficient 150% -> 175%.

162. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22FBA (143290) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 9 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

163. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x230CC (143564) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Bow Attack record ID 12; participants [30, 43]; coefficient 50% -> 75%.

164. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2309E (143518) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 12 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

165. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23118 (143640) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Bow Attack record ID 13; participants [30, 67]; coefficient 50% -> 75%.

166. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x230EA (143594) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 13 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

167. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23164 (143716) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Bow Attack record ID 14; participants [43, 67]; coefficient 50% -> 75%.

168. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23136 (143670) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 14 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

169. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x231FC (143868) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Narcissists Attack record ID 16; participants [64, 65]; coefficient 50% -> 75%.

170. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x231CE (143822) - description
     RETAIL HEX: 98669D1028103E474110241F0E111C1C103F230000000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E474110241F0E111C1C103F2300000000000000000000000000000000
     Meaning: Narcissists Attack record ID 16 menu text: '0.5 x DMG to / all Es' -> '0.75 x DMG to / all Es'.

171. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23248 (143944) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Winger Attack record ID 17; participants [54, 56]; coefficient 150% -> 175%.

172. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2321A (143898) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A000000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A0000000000
     Meaning: Winger Attack record ID 17 menu text: '1.5 x DMG vs. 1 E / Poison <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Poison <69>30<94><6A>'.

173. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23294 (144020) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Dad & Daughter Attack record ID 18; participants [52, 17]; coefficient 100% -> 125%.

174. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23266 (143974) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     v1.2 HEX:   99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Dad & Daughter Attack record ID 18 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

175. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23410 (144400) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   7D00
     Meaning: Double Kraken Attack record ID 23; participants [49, 74]; coefficient 100% -> 125%.

176. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x233E2 (144354) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     v1.2 HEX:   99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Double Kraken Attack record ID 23 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

177. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2345C (144476) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Swordsman Attack record ID 24; participants [15, 47]; coefficient 50% -> 75%.

178. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2342E (144430) - description
     RETAIL HEX: 98669D283E47411026236610111C1C103F230E4D251414151E101415112418109A989400
     v1.2 HEX:   98669F9D283E474110262366111C1C103F230E4D251414151E101415112418109A989400
     Meaning: Swordsman Attack record ID 24 menu text: '0.5xDMG vs. all Es / Sudden death 20<94>' -> '0.75xDMG vs.all Es / Sudden death 20<94>'.

179. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x234A8 (144552) - percentage coefficient
     RETAIL HEX: 6400
     v1.2 HEX:   9600
     Meaning: Copycat Attack record ID 25; participants [1, 71]; coefficient 100% -> 150%.

180. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2347A (144506) - description
     RETAIL HEX: 991028103E4741102623661099103F000000000000000000000000000000000000000000
     v1.2 HEX:   99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     Meaning: Copycat Attack record ID 25 menu text: '1 x DMG vs. 1 E' -> '1.5 x DMG vs. 1 E'.

181. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23540 (144704) - percentage coefficient
     RETAIL HEX: C800
     v1.2 HEX:   E100
     Meaning: Circus Attack record ID 27; participants [19, 20, 21]; coefficient 200% -> 225%.

182. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23512 (144658) - description
     RETAIL HEX: 9A1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500000000
     v1.2 HEX:   9A669A9D1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500
     Meaning: Circus Attack record ID 27 menu text: '2 x DMG vs. 1 E / Bolgan Unbalance' -> '2.25 x DMG vs. 1 E / Bolgan Unbalance'.

183. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x237A0 (145312) - percentage coefficient
     RETAIL HEX: 4B00
     v1.2 HEX:   6400
     Meaning: Tackle Attack record ID 35; participants [23, 46]; coefficient 75% -> 100%.

184. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23772 (145266) - description
     RETAIL HEX: 98669F9D1028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000
     v1.2 HEX:   991028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000000000
     Meaning: Tackle Attack record ID 35 menu text: '0.75 x DMG vs. / all Es Unbalance' -> '1 x DMG vs. / all Es Unbalance'.

185. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23884 (145540) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Pretty Girl Attack record ID 38; participants [8, 24, 41]; coefficient 50% -> 75%.

186. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23856 (145494) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 38 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

187. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x238D0 (145616) - percentage coefficient
     RETAIL HEX: 3200
     v1.2 HEX:   4B00
     Meaning: Pretty Girl Attack record ID 39; participants [8, 83, 41]; coefficient 50% -> 75%.

188. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x238A2 (145570) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     v1.2 HEX:   98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 39 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

189. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x238EE (145646) - description
     RETAIL HEX: 99283E47411026236610111C1C103F230E4111121F131811104F1E12111C111E13150000
     v1.2 HEX:   9B283E47411026236610111C1C103F230E3C1F2418104F1E12111C111E13150000000000
     Meaning: 100 Kobold Attack record ID 40 menu text: '1xDMG vs. all Es / Gabocha Unbalance' -> '3xDMG vs. all Es / Both Unbalance'.

190. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x239B4 (145844) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Bandit Attack record ID 42; participants [58, 59, 60]; coefficient 150% -> 175%.

191. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23986 (145798) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A0000
     Meaning: Bandit Attack record ID 42 menu text: '1.5 x DMG vs. 1 E / Knockdown <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Knockdown <69>30<94><6A>'.

192. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B30 (146224) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 47; participants [51, 49, 74]; coefficient 150% -> 175%.

193. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B02 (146178) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 47 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

194. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B7C (146300) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 48; participants [51, 49, 72]; coefficient 150% -> 175%.

195. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B4E (146254) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 48 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

196. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23BC8 (146376) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 49; participants [51, 49, 50]; coefficient 150% -> 175%.

197. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B9A (146330) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 49 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

198. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23C14 (146452) - percentage coefficient
     RETAIL HEX: 9600
     v1.2 HEX:   AF00
     Meaning: Beastmaster Attack record ID 50; participants [51, 72, 50]; coefficient 150% -> 175%.

199. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23BE6 (146406) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     v1.2 HEX:   99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 50 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

200. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x1DAE0 (121568) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     v1.2 HEX:   E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

201. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x1DB04 (121604) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     v1.2 HEX:   E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

202. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x1DB28 (121640) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     v1.2 HEX:   E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

203. /SLUS_009.58 +0x1E174 (123252) - Kindness signed-rating instruction
     RETAIL HEX: FFFF4332
     v1.2 HEX:   21184002
     Meaning: Kindness Rune: remove the unsigned16-bit mask from the signed rating path; signed negative ratings retain their attack penalty. The no-penalty alternative is not used.

204. /CDROM/010_ARA/VA03.BIN +0x8E94 (36500) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

205. /CDROM/010_ARA/VA05.BIN +0xB904 (47364) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

206. /CDROM/010_ARA/VA06.BIN +0x9360 (37728) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

207. /CDROM/010_ARA/VA11.BIN +0x559C (21916) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

208. /CDROM/020_ARB/VB02.BIN +0x975C (38748) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

209. /CDROM/020_ARB/VB03.BIN +0x9DCC (40396) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

210. /CDROM/020_ARB/VB04.BIN +0xAE50 (44624) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

211. /CDROM/020_ARB/VB05.BIN +0xAB28 (43816) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

212. /CDROM/020_ARB/VB06.BIN +0x2938 (10552) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

213. /CDROM/020_ARB/VB11.BIN +0xA1A0 (41376) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

214. /CDROM/020_ARB/VB14.BIN +0x8E64 (36452) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

215. /CDROM/020_ARB/VB15.BIN +0x4AE8 (19176) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

216. /CDROM/020_ARB/VB18.BIN +0xA8BC (43196) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

217. /CDROM/020_ARB/VB19.BIN +0x748C (29836) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

218. /CDROM/020_ARB/VB21.BIN +0xE884 (59524) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

219. /CDROM/030_ARC/VC01.BIN +0x1111C (69916) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

220. /CDROM/030_ARC/VC03.BIN +0x27E0 (10208) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

221. /CDROM/030_ARC/VC06.BIN +0x6780 (26496) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

222. /CDROM/030_ARC/VC07.BIN +0xD0E0 (53472) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

223. /CDROM/030_ARC/VC10.BIN +0x6784 (26500) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

224. /CDROM/030_ARC/VC11.BIN +0x68A0 (26784) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

225. /CDROM/030_ARC/VC16.BIN +0x83D0 (33744) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

226. /CDROM/030_ARC/VC18.BIN +0x8224 (33316) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

227. /CDROM/030_ARC/VC21.BIN +0x170A0 (94368) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

228. /CDROM/030_ARC/VC22.BIN +0xB14 (2836) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

229. /CDROM/030_ARC/VC24.BIN +0xB3E0 (46048) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

230. /CDROM/030_ARC/VC25.BIN +0x1C14 (7188) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

231. /CDROM/030_ARC/VC27.BIN +0x3780 (14208) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

232. /CDROM/030_ARC/VC28.BIN +0xF7C8 (63432) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

233. /CDROM/030_ARC/VC30.BIN +0x8038 (32824) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

234. /CDROM/040_ARD/VD01.BIN +0xE9B8 (59832) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

235. /CDROM/040_ARD/VD03.BIN +0x6D98 (28056) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

236. /CDROM/040_ARD/VD17.BIN +0x82C8 (33480) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

237. /CDROM/040_ARD/VD19.BIN +0x610C (24844) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

238. /CDROM/050_ARE/VE01.BIN +0xED2C (60716) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

239. /CDROM/050_ARE/VE02.BIN +0x7B20 (31520) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

240. /CDROM/050_ARE/VE05.BIN +0x1A70 (6768) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

241. /CDROM/050_ARE/VE10.BIN +0x6D40 (27968) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

242. /CDROM/050_ARE/VE13.BIN +0xFF80 (65408) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

243. /CDROM/060_ARF/VF01.BIN +0x943C (37948) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

244. /CDROM/060_ARF/VF03.BIN +0x9F4C (40780) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

245. /CDROM/060_ARF/VF05.BIN +0xD008 (53256) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

246. /CDROM/070_ARG/VG03.BIN +0x76FC (30460) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

247. /CDROM/070_ARG/VG06.BIN +0x6704 (26372) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

248. /CDROM/070_ARG/VG07.BIN +0x8770 (34672) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

249. /CDROM/070_ARG/VG08.BIN +0x8C38 (35896) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

250. /CDROM/070_ARG/VG13.BIN +0xA7A8 (42920) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

251. /CDROM/070_ARG/VG18.BIN +0x9F4C (40780) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

252. /CDROM/080_ARH/VH01.BIN +0xA820 (43040) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

253. /CDROM/080_ARH/VH02.BIN +0x8B20 (35616) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

254. /CDROM/080_ARH/VH03.BIN +0xD224 (53796) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

255. /CDROM/080_ARH/VH05.BIN +0xABDC (43996) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

256. /CDROM/080_ARH/VH06.BIN +0x802C (32812) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

257. /CDROM/080_ARH/VH11.BIN +0xA2D8 (41688) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

258. /CDROM/080_ARH/VH12.BIN +0x5334 (21300) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

259. /CDROM/080_ARH/VH13.BIN +0x8250 (33360) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

260. /CDROM/080_ARH/VH14.BIN +0x8A58 (35416) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

261. /CDROM/080_ARH/VH16.BIN +0x707C (28796) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

262. /CDROM/080_ARH/VH17.BIN +0xA298 (41624) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

263. /CDROM/090_ARI/VI01.BIN +0xE558 (58712) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

264. /CDROM/090_ARI/VI02.BIN +0x9CD4 (40148) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

265. /CDROM/090_ARI/VI12.BIN +0x90E0 (37088) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

266. /CDROM/090_ARI/VI14.BIN +0x1F28 (7976) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

267. /CDROM/100_ARJ/VJ17.BIN +0x2D40 (11584) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     v1.2 HEX:   47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

268. /CDROM/110_ARK/VK01.BIN +0x2098 (8344) - Headquarters world-map preload boundary
     RETAIL HEX: 013B6702889BFFFE
     v1.2 HEX:   013B6702889DFFFE
     Meaning: Headquarters exit: extend the shared background world-map preload from inclusive Y155 to157, covering the two exit rows. This prevents the lower-wall route from using a cached bar with world-map texture geometry and corrupting live collision data. X bounds, neighboring preloads, destination, story flags and combat data remain unchanged.

269. /CDROM/110_ARK/VK34.BIN +0x2478 (9336) - Headquarters world-map preload boundary
     RETAIL HEX: 013B6702889BFFFE
     v1.2 HEX:   013B6702889DFFFE
     Meaning: Headquarters exit: extend the shared background world-map preload from inclusive Y155 to157, covering the two exit rows. This prevents the lower-wall route from using a cached bar with world-map texture geometry and corrupting live collision data. X bounds, neighboring preloads, destination, story flags and combat data remain unchanged.

270. /CDROM/010_ARA/VA05.BIN +0x4A1CB (303563) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

271. /CDROM/010_ARA/VA06.BIN +0x364D3 (222419) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

272. /CDROM/010_ARA/VA08.BIN +0x38377 (230263) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

273. /CDROM/010_ARA/VA24.BIN +0x3910F (233743) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

274. /CDROM/020_ARB/VB04.BIN +0x41903 (268547) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

275. /CDROM/020_ARB/VB07.BIN +0x33ECF (212687) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

276. /CDROM/020_ARB/VB09.BIN +0x2A967 (174439) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

277. /CDROM/020_ARB/VB10.BIN +0x382CB (230091) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

278. /CDROM/020_ARB/VB12.BIN +0x3884B (231499) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

279. /CDROM/030_ARC/VC04.BIN +0x49663 (300643) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

280. /CDROM/030_ARC/VC07.BIN +0x3637B (222075) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

281. /CDROM/030_ARC/VC09.BIN +0x4294F (272719) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

282. /CDROM/030_ARC/VC28.BIN +0x3CF6F (249711) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

283. /CDROM/030_ARC/VC30.BIN +0x2E937 (190775) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

284. /CDROM/040_ARD/VD07.BIN +0xC303 (49923) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

285. /CDROM/050_ARE/VE06.BIN +0x46CAF (289967) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

286. /CDROM/060_ARF/VF01.BIN +0x3C257 (246359) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

287. /CDROM/060_ARF/VF02.BIN +0x45C0F (285711) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

288. /CDROM/060_ARF/VF04.BIN +0x46C63 (289891) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

289. /CDROM/090_ARI/VI05.BIN +0x367EF (223215) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

290. /CDROM/090_ARI/VI10.BIN +0x3B937 (244023) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

291. /CDROM/090_ARI/VI11.BIN +0x27783 (161667) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

292. /CDROM/100_ARJ/VJ24.BIN +0x2C067 (180327) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

293. /CDROM/110_ARK/VK06.BIN +0x45FAF (286639) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

294. /CDROM/130_SHOP/DOUGUYA1.BIN +0x10ECF (69327) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

295. /CDROM/130_SHOP/DOUGUYA2.BIN +0x10ECF (69327) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

296. /CDROM/130_SHOP/KAJIYA1.BIN +0xD8FF (55551) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

297. /CDROM/130_SHOP/KAJIYA2.BIN +0xD8FF (55551) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

298. /CDROM/130_SHOP/KANTEIY1.BIN +0xAA97 (43671) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

299. /CDROM/130_SHOP/KANTEIY2.BIN +0xAA97 (43671) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

300. /CDROM/130_SHOP/KOUEKI1.BIN +0xD65F (54879) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

301. /CDROM/130_SHOP/KOUEKI2.BIN +0xD65F (54879) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

302. /CDROM/130_SHOP/KPARTY1.BIN +0x720B (29195) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

303. /CDROM/130_SHOP/KPARTY2.BIN +0x720B (29195) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

304. /CDROM/130_SHOP/MONSYOY1.BIN +0xED6B (60779) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

305. /CDROM/130_SHOP/MONSYOY2.BIN +0xED6B (60779) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

306. /CDROM/130_SHOP/PARTYIN1.BIN +0xB4D3 (46291) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

307. /CDROM/130_SHOP/PARTYIN2.BIN +0xB4D3 (46291) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

308. /CDROM/140_HONP/FUDAZUK.BIN +0xCD27 (52519) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

309. /CDROM/140_HONP/HDOUGUYA.BIN +0x119C3 (72131) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

310. /CDROM/140_HONP/HKAJIYA.BIN +0xE217 (57879) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

311. /CDROM/140_HONP/HMONSYOY.BIN +0xEDAF (60847) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

312. /CDROM/140_HONP/KIKORI.BIN +0x36EF7 (225015) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

313. /CDROM/140_HONP/MOGURA.BIN +0x17A0B (96779) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

314. /CDROM/140_HONP/PARTYCE1.BIN +0x482CB (295627) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

315. /CDROM/140_HONP/PARTYCH2.BIN +0x46B4B (289611) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

316. /CDROM/140_HONP/PARTYCHG.BIN +0x46B4B (289611) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

317. /CDROM/140_HONP/RBATTLE.BIN +0x4B1E7 (307687) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

318. /CDROM/140_HONP/REST.BIN +0xB25F (45663) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

319. /CDROM/140_HONP/SOUKO.BIN +0x1D36B (119659) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

320. /CDROM/140_HONP/STONE.BIN +0x25D8F (155023) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

321. /CDROM/140_HONP/SYUGOITM.BIN +0x96F7 (38647) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

322. /CDROM/140_HONP/VB19PIN.BIN +0x743F (29759) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

323. /CDROM/140_HONP/VG08PIN.BIN +0x72A3 (29347) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

324. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0xB113 (45331) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

325. /CDROM/270_BOOT/BOOT.BIN +0x2D537 (185655) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

326. /CDROM/270_BOOT/G1LOAD.BIN +0x21327 (135975) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

327. /CDROM/270_BOOT/OVER.BIN +0x39F6B (237419) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

328. /CDROM/280_GAME/EMBL.BIN +0x987 (2439) - Rune menu description duplicate
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     v1.2 HEX:   99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Rune 39 menu description -> '1.75x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

329. /CDROM/010_ARA/VA05.BIN +0x4A33F (303935) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

330. /CDROM/010_ARA/VA06.BIN +0x36647 (222791) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

331. /CDROM/010_ARA/VA08.BIN +0x384EB (230635) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

332. /CDROM/010_ARA/VA24.BIN +0x39283 (234115) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

333. /CDROM/020_ARB/VB04.BIN +0x41A77 (268919) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

334. /CDROM/020_ARB/VB07.BIN +0x34043 (213059) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

335. /CDROM/020_ARB/VB09.BIN +0x2AADB (174811) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

336. /CDROM/020_ARB/VB10.BIN +0x3843F (230463) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

337. /CDROM/020_ARB/VB12.BIN +0x389BF (231871) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

338. /CDROM/030_ARC/VC04.BIN +0x497D7 (301015) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

339. /CDROM/030_ARC/VC07.BIN +0x364EF (222447) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

340. /CDROM/030_ARC/VC09.BIN +0x42AC3 (273091) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

341. /CDROM/030_ARC/VC28.BIN +0x3D0E3 (250083) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

342. /CDROM/030_ARC/VC30.BIN +0x2EAAB (191147) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

343. /CDROM/040_ARD/VD07.BIN +0xC477 (50295) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

344. /CDROM/050_ARE/VE06.BIN +0x46E23 (290339) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

345. /CDROM/060_ARF/VF01.BIN +0x3C3CB (246731) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

346. /CDROM/060_ARF/VF02.BIN +0x45D83 (286083) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

347. /CDROM/060_ARF/VF04.BIN +0x46DD7 (290263) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

348. /CDROM/090_ARI/VI05.BIN +0x36963 (223587) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

349. /CDROM/090_ARI/VI10.BIN +0x3BAAB (244395) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

350. /CDROM/090_ARI/VI11.BIN +0x278F7 (162039) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

351. /CDROM/100_ARJ/VJ24.BIN +0x2C1DB (180699) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

352. /CDROM/110_ARK/VK06.BIN +0x46123 (287011) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

353. /CDROM/130_SHOP/DOUGUYA1.BIN +0x11043 (69699) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

354. /CDROM/130_SHOP/DOUGUYA2.BIN +0x11043 (69699) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

355. /CDROM/130_SHOP/KAJIYA1.BIN +0xDA73 (55923) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

356. /CDROM/130_SHOP/KAJIYA2.BIN +0xDA73 (55923) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

357. /CDROM/130_SHOP/KANTEIY1.BIN +0xAC0B (44043) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

358. /CDROM/130_SHOP/KANTEIY2.BIN +0xAC0B (44043) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

359. /CDROM/130_SHOP/KOUEKI1.BIN +0xD7D3 (55251) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

360. /CDROM/130_SHOP/KOUEKI2.BIN +0xD7D3 (55251) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

361. /CDROM/130_SHOP/KPARTY1.BIN +0x737F (29567) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

362. /CDROM/130_SHOP/KPARTY2.BIN +0x737F (29567) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

363. /CDROM/130_SHOP/MONSYOY1.BIN +0xEEDF (61151) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

364. /CDROM/130_SHOP/MONSYOY2.BIN +0xEEDF (61151) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

365. /CDROM/130_SHOP/PARTYIN1.BIN +0xB647 (46663) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

366. /CDROM/130_SHOP/PARTYIN2.BIN +0xB647 (46663) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

367. /CDROM/140_HONP/FUDAZUK.BIN +0xCE9B (52891) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

368. /CDROM/140_HONP/HDOUGUYA.BIN +0x11B37 (72503) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

369. /CDROM/140_HONP/HKAJIYA.BIN +0xE38B (58251) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

370. /CDROM/140_HONP/HMONSYOY.BIN +0xEF23 (61219) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

371. /CDROM/140_HONP/KIKORI.BIN +0x3706B (225387) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

372. /CDROM/140_HONP/MOGURA.BIN +0x17B7F (97151) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

373. /CDROM/140_HONP/PARTYCE1.BIN +0x4843F (295999) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

374. /CDROM/140_HONP/PARTYCH2.BIN +0x46CBF (289983) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

375. /CDROM/140_HONP/PARTYCHG.BIN +0x46CBF (289983) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

376. /CDROM/140_HONP/RBATTLE.BIN +0x4B35B (308059) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

377. /CDROM/140_HONP/REST.BIN +0xB3D3 (46035) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

378. /CDROM/140_HONP/SOUKO.BIN +0x1D4DF (120031) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

379. /CDROM/140_HONP/STONE.BIN +0x25F03 (155395) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

380. /CDROM/140_HONP/SYUGOITM.BIN +0x986B (39019) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

381. /CDROM/140_HONP/VB19PIN.BIN +0x75B3 (30131) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

382. /CDROM/140_HONP/VG08PIN.BIN +0x7417 (29719) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

383. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0xB287 (45703) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

384. /CDROM/270_BOOT/BOOT.BIN +0x2D6AB (186027) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

385. /CDROM/270_BOOT/G1LOAD.BIN +0x2149B (136347) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

386. /CDROM/270_BOOT/OVER.BIN +0x3A0DF (237791) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

387. /CDROM/280_GAME/EMBL.BIN +0xAFB (2811) - Rune menu description duplicate
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Rune 45 menu description -> '1.5x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

388. /CDROM/010_ARA/VA05.BIN +0x4A4B3 (304307) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

389. /CDROM/010_ARA/VA06.BIN +0x367BB (223163) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

390. /CDROM/010_ARA/VA08.BIN +0x3865F (231007) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

391. /CDROM/010_ARA/VA24.BIN +0x393F7 (234487) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

392. /CDROM/020_ARB/VB04.BIN +0x41BEB (269291) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

393. /CDROM/020_ARB/VB07.BIN +0x341B7 (213431) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

394. /CDROM/020_ARB/VB09.BIN +0x2AC4F (175183) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

395. /CDROM/020_ARB/VB10.BIN +0x385B3 (230835) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

396. /CDROM/020_ARB/VB12.BIN +0x38B33 (232243) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

397. /CDROM/030_ARC/VC04.BIN +0x4994B (301387) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

398. /CDROM/030_ARC/VC07.BIN +0x36663 (222819) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

399. /CDROM/030_ARC/VC09.BIN +0x42C37 (273463) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

400. /CDROM/030_ARC/VC28.BIN +0x3D257 (250455) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

401. /CDROM/030_ARC/VC30.BIN +0x2EC1F (191519) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

402. /CDROM/040_ARD/VD07.BIN +0xC5EB (50667) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

403. /CDROM/050_ARE/VE06.BIN +0x46F97 (290711) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

404. /CDROM/060_ARF/VF01.BIN +0x3C53F (247103) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

405. /CDROM/060_ARF/VF02.BIN +0x45EF7 (286455) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

406. /CDROM/060_ARF/VF04.BIN +0x46F4B (290635) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

407. /CDROM/090_ARI/VI05.BIN +0x36AD7 (223959) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

408. /CDROM/090_ARI/VI10.BIN +0x3BC1F (244767) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

409. /CDROM/090_ARI/VI11.BIN +0x27A6B (162411) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

410. /CDROM/100_ARJ/VJ24.BIN +0x2C34F (181071) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

411. /CDROM/110_ARK/VK06.BIN +0x46297 (287383) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

412. /CDROM/130_SHOP/DOUGUYA1.BIN +0x111B7 (70071) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

413. /CDROM/130_SHOP/DOUGUYA2.BIN +0x111B7 (70071) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

414. /CDROM/130_SHOP/KAJIYA1.BIN +0xDBE7 (56295) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

415. /CDROM/130_SHOP/KAJIYA2.BIN +0xDBE7 (56295) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

416. /CDROM/130_SHOP/KANTEIY1.BIN +0xAD7F (44415) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

417. /CDROM/130_SHOP/KANTEIY2.BIN +0xAD7F (44415) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

418. /CDROM/130_SHOP/KOUEKI1.BIN +0xD947 (55623) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

419. /CDROM/130_SHOP/KOUEKI2.BIN +0xD947 (55623) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

420. /CDROM/130_SHOP/KPARTY1.BIN +0x74F3 (29939) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

421. /CDROM/130_SHOP/KPARTY2.BIN +0x74F3 (29939) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

422. /CDROM/130_SHOP/MONSYOY1.BIN +0xF053 (61523) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

423. /CDROM/130_SHOP/MONSYOY2.BIN +0xF053 (61523) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

424. /CDROM/130_SHOP/PARTYIN1.BIN +0xB7BB (47035) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

425. /CDROM/130_SHOP/PARTYIN2.BIN +0xB7BB (47035) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

426. /CDROM/140_HONP/FUDAZUK.BIN +0xD00F (53263) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

427. /CDROM/140_HONP/HDOUGUYA.BIN +0x11CAB (72875) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

428. /CDROM/140_HONP/HKAJIYA.BIN +0xE4FF (58623) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

429. /CDROM/140_HONP/HMONSYOY.BIN +0xF097 (61591) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

430. /CDROM/140_HONP/KIKORI.BIN +0x371DF (225759) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

431. /CDROM/140_HONP/MOGURA.BIN +0x17CF3 (97523) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

432. /CDROM/140_HONP/PARTYCE1.BIN +0x485B3 (296371) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

433. /CDROM/140_HONP/PARTYCH2.BIN +0x46E33 (290355) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

434. /CDROM/140_HONP/PARTYCHG.BIN +0x46E33 (290355) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

435. /CDROM/140_HONP/RBATTLE.BIN +0x4B4CF (308431) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

436. /CDROM/140_HONP/REST.BIN +0xB547 (46407) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

437. /CDROM/140_HONP/SOUKO.BIN +0x1D653 (120403) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

438. /CDROM/140_HONP/STONE.BIN +0x26077 (155767) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

439. /CDROM/140_HONP/SYUGOITM.BIN +0x99DF (39391) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

440. /CDROM/140_HONP/VB19PIN.BIN +0x7727 (30503) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

441. /CDROM/140_HONP/VG08PIN.BIN +0x758B (30091) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

442. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0xB3FB (46075) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

443. /CDROM/270_BOOT/BOOT.BIN +0x2D81F (186399) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

444. /CDROM/270_BOOT/G1LOAD.BIN +0x2160F (136719) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

445. /CDROM/270_BOOT/OVER.BIN +0x3A253 (238163) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

446. /CDROM/280_GAME/EMBL.BIN +0xC6F (3183) - Rune menu description duplicate
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     v1.2 HEX:   9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Rune 51 menu description -> '2x DMG Repeatable'; bounded32-byte field, name/metadata unchanged.

447. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x280B0 (164016) - Battle rune help description
     RETAIL HEX: 4E1F2910221F121F241011242411131B230E3D1F1D121124101F1E1315101F1E1C290000
     v1.2 HEX:   99669F9D283E47410E4C152015112411121C150000000000000000000000000000000000
     Meaning: Spell 79 battle-menu help -> '1.75xDMG / Repeatable'; original pointer-defined string slot unchanged.

448. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x280FC (164092) - Battle rune help description
     RETAIL HEX: 3B242411131B23109910221F270E4C25191E231012111C111E131500
     v1.2 HEX:   99669A9D283E474110221F270E4C25191E231012111C111E13150000
     Meaning: Spell 82 battle-menu help -> '1.25xDMG row / Ruins balance'; original pointer-defined string slot unchanged.

449. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x28118 (164120) - Battle rune help description
     RETAIL HEX: 4D251414151E10141511241810699B98946A0E4C25191E231012111C111E131500000000
     v1.2 HEX:   99669D283E4741109B98941014151124180E4C25191E231012111C111E13150000000000
     Meaning: Spell 83 battle-menu help -> '1.5xDMG 30% death / Ruins balance'; original pointer-defined string slot unchanged.

450. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x28154 (164180) - Battle rune help description
     RETAIL HEX: 9A1028103E47410E3D1F1D121124101F1E1315101F1E1C2900000000
     v1.2 HEX:   99669D283E47410E4C152015112411121C1500000000000000000000
     Meaning: Spell 85 battle-menu help -> '1.5xDMG / Repeatable'; original pointer-defined string slot unchanged.

451. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2828C (164492) - Battle rune help description
     RETAIL HEX: 9B1028103E47410E3D1F1D121124101F1E1315101F1E1C2900000000
     v1.2 HEX:   9A283E47410E4C152015112411121C15000000000000000000000000
     Meaning: Spell 95 battle-menu help -> '2xDMG / Repeatable'; original pointer-defined string slot unchanged.

452. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x26DE8 (159208) - Battle rune help description
     RETAIL HEX: 4E1F2910221F121F241011242411131B230E3D1F1D121124101F1E1315101F1E1C290000
     v1.2 HEX:   99669F9D283E47410E4C152015112411121C150000000000000000000000000000000000
     Meaning: Spell 79 battle-menu help -> '1.75xDMG / Repeatable'; original pointer-defined string slot unchanged.

453. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x26E34 (159284) - Battle rune help description
     RETAIL HEX: 3B242411131B23109910221F270E4C25191E231012111C111E131500
     v1.2 HEX:   99669A9D283E474110221F270E4C25191E231012111C111E13150000
     Meaning: Spell 82 battle-menu help -> '1.25xDMG row / Ruins balance'; original pointer-defined string slot unchanged.

454. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x26E50 (159312) - Battle rune help description
     RETAIL HEX: 4D251414151E10141511241810699B98946A0E4C25191E231012111C111E131500000000
     v1.2 HEX:   99669D283E4741109B98941014151124180E4C25191E231012111C111E13150000000000
     Meaning: Spell 83 battle-menu help -> '1.5xDMG 30% death / Ruins balance'; original pointer-defined string slot unchanged.

455. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x26E8C (159372) - Battle rune help description
     RETAIL HEX: 9A1028103E47410E3D1F1D121124101F1E1315101F1E1C2900000000
     v1.2 HEX:   99669D283E47410E4C152015112411121C1500000000000000000000
     Meaning: Spell 85 battle-menu help -> '1.5xDMG / Repeatable'; original pointer-defined string slot unchanged.

456. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x26FC4 (159684) - Battle rune help description
     RETAIL HEX: 9B1028103E47410E3D1F1D121124101F1E1315101F1E1C2900000000
     v1.2 HEX:   9A283E47410E4C152015112411121C15000000000000000000000000
     Meaning: Spell 95 battle-menu help -> '2xDMG / Repeatable'; original pointer-defined string slot unchanged.

457. /CDROM/030_ARC/VC07.BIN +0xB6CD (46797) - Dialogue spelling
     RETAIL HEX: 511510232520221923151410291F2566666666161F221719261510252366
     v1.2 HEX:   51151023252220221923151410291F25666666161F221719261510252366
     Meaning: 'We suprised you....forgive us.' -> 'We surprised you...forgive us.'; equal-length sentence.

458. /CDROM/030_ARC/VC08.BIN +0x1629 (5673) - Dialogue spelling
     RETAIL HEX: 511510232520221923151410291F2566666666161F221719261510252366
     v1.2 HEX:   51151023252220221923151410291F25666666161F221719261510252366
     Meaning: 'We suprised you....forgive us.' -> 'We surprised you...forgive us.'; equal-length sentence.

459. /CDROM/030_ARC/VC30.BIN +0x6625 (26149) - Dialogue spelling
     RETAIL HEX: 511510232520221923151410291F2566666666161F221719261510252366
     v1.2 HEX:   51151023252220221923151410291F25666666161F221719261510252366
     Meaning: 'We suprised you....forgive us.' -> 'We surprised you...forgive us.'; equal-length sentence.

460. /CDROM/010_ARA/VA03.BIN +0x4537 (17719) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

461. /CDROM/010_ARA/VA05.BIN +0x92CB (37579) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

462. /CDROM/010_ARA/VA06.BIN +0x6A5F (27231) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

463. /CDROM/010_ARA/VA07.BIN +0x1613 (5651) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

464. /CDROM/010_ARA/VA08.BIN +0x61AF (25007) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

465. /CDROM/010_ARA/VA12.BIN +0x337F (13183) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

466. /CDROM/010_ARA/VA16.BIN +0x1593 (5523) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

467. /CDROM/010_ARA/VA18.BIN +0x22BF (8895) - Reviewed spelling and text fit
     RETAIL HEX: 231F1D151F1E151027181F101811230E131F1D1D19
     v1.2 HEX:   111E291F1E151027181F101811230E131F1D1D1924
     Meaning: commited -> committed; bounded text fit: reviewed wording: someone who has -> anyone who has
     ORIGINAL TEXT:  / I can't recognize someone who has / commited treason as a member of / the Atreides Clan."
     v1.1 TEXT:      / I can't recognize anyone who has / committed treason as a member of / the Atreides Clan."

468. /CDROM/010_ARA/VA03.BIN +0x5501 (21761) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

469. /CDROM/010_ARA/VA05.BIN +0xA295 (41621) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

470. /CDROM/010_ARA/VA06.BIN +0x7A29 (31273) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

471. /CDROM/010_ARA/VA07.BIN +0x25DD (9693) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

472. /CDROM/010_ARA/VA08.BIN +0x7179 (29049) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

473. /CDROM/010_ARA/VA12.BIN +0x4349 (17225) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

474. /CDROM/010_ARA/VA16.BIN +0x255D (9565) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

475. /CDROM/010_ARA/VA18.BIN +0x3289 (12937) - Reviewed spelling and text fit
     RETAIL HEX: 491610131F2523
     v1.2 HEX:   101010104D2522
     Meaning: couse -> course; bounded text fit: reviewed affirmation: Of couse -> Sure
     ORIGINAL TEXT: "Of couse, 
     v1.1 TEXT:     "    Sure, 

476. /CDROM/010_ARA/VA03.BIN +0x68CA (26826) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

477. /CDROM/010_ARA/VA05.BIN +0xB65E (46686) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

478. /CDROM/010_ARA/VA06.BIN +0x8DF2 (36338) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

479. /CDROM/010_ARA/VA07.BIN +0x39A6 (14758) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

480. /CDROM/010_ARA/VA08.BIN +0x8542 (34114) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

481. /CDROM/010_ARA/VA12.BIN +0x5712 (22290) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

482. /CDROM/010_ARA/VA16.BIN +0x3926 (14630) - Reviewed spelling and text fit
     RETAIL HEX: 17109A101611261F22192415
     v1.2 HEX:   191E17109A102022192A1514
     Meaning: remaing -> remaining; bounded text fit: reviewed wording: remaining 2 favorite -> remaining 2 prized
     ORIGINAL TEXT:  / Nanami's remaing 2 favorite vases
     v1.1 TEXT:      / Nanami's remaining 2 prized vases

483. /CDROM/010_ARA/VA03.BIN +0x9241 (37441) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122681043101815112214102418112410231F1D150E231311222910231F251E14191E171011221D291013111C1C15140E
     v1.2 HEX:   112020151122681043101815112214102418112410231F1D150E231311222910231F251E14191E171011221D291013111C1C15140E10
     Meaning: dissappear -> disappear; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Is this country going to / dissappear? I heard that some / scary sounding army called / 
     v1.1 TEXT:     "Is this country going to / disappear? I heard that some / scary sounding army called /  

484. /CDROM/010_ARA/VA05.BIN +0x4AB8B (306059) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

485. /CDROM/010_ARA/VA06.BIN +0x36E93 (224915) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

486. /CDROM/010_ARA/VA08.BIN +0x38D37 (232759) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

487. /CDROM/010_ARA/VA24.BIN +0x39ACF (236239) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

488. /CDROM/020_ARB/VB04.BIN +0x422C3 (271043) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

489. /CDROM/020_ARB/VB07.BIN +0x3488F (215183) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

490. /CDROM/020_ARB/VB09.BIN +0x2B327 (176935) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

491. /CDROM/020_ARB/VB10.BIN +0x38C8B (232587) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

492. /CDROM/020_ARB/VB12.BIN +0x3920B (233995) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

493. /CDROM/030_ARC/VC04.BIN +0x4A023 (303139) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

494. /CDROM/030_ARC/VC07.BIN +0x36D3B (224571) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

495. /CDROM/030_ARC/VC09.BIN +0x4330F (275215) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

496. /CDROM/030_ARC/VC28.BIN +0x3D92F (252207) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

497. /CDROM/030_ARC/VC30.BIN +0x2F2F7 (193271) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

498. /CDROM/040_ARD/VD07.BIN +0xCCC3 (52419) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

499. /CDROM/050_ARE/VE06.BIN +0x4766F (292463) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

500. /CDROM/060_ARF/VF01.BIN +0x3CC17 (248855) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

501. /CDROM/060_ARF/VF02.BIN +0x465CF (288207) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

502. /CDROM/060_ARF/VF04.BIN +0x47623 (292387) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

503. /CDROM/090_ARI/VI05.BIN +0x371AF (225711) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

504. /CDROM/090_ARI/VI10.BIN +0x3C2F7 (246519) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

505. /CDROM/090_ARI/VI11.BIN +0x28143 (164163) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

506. /CDROM/100_ARJ/VJ24.BIN +0x2CA27 (182823) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

507. /CDROM/110_ARK/VK06.BIN +0x4696F (289135) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

508. /CDROM/130_SHOP/DOUGUYA1.BIN +0x1188F (71823) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

509. /CDROM/130_SHOP/DOUGUYA2.BIN +0x1188F (71823) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

510. /CDROM/130_SHOP/KAJIYA1.BIN +0xE2BF (58047) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

511. /CDROM/130_SHOP/KAJIYA2.BIN +0xE2BF (58047) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

512. /CDROM/130_SHOP/KANTEIY1.BIN +0xB457 (46167) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

513. /CDROM/130_SHOP/KANTEIY2.BIN +0xB457 (46167) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

514. /CDROM/130_SHOP/KOUEKI1.BIN +0xE01F (57375) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

515. /CDROM/130_SHOP/KOUEKI2.BIN +0xE01F (57375) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

516. /CDROM/130_SHOP/KPARTY1.BIN +0x7BCB (31691) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

517. /CDROM/130_SHOP/KPARTY2.BIN +0x7BCB (31691) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

518. /CDROM/130_SHOP/MONSYOY1.BIN +0xF72B (63275) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

519. /CDROM/130_SHOP/MONSYOY2.BIN +0xF72B (63275) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

520. /CDROM/130_SHOP/PARTYIN1.BIN +0xBE93 (48787) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

521. /CDROM/130_SHOP/PARTYIN2.BIN +0xBE93 (48787) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

522. /CDROM/140_HONP/FUDAZUK.BIN +0xD6E7 (55015) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

523. /CDROM/140_HONP/HDOUGUYA.BIN +0x12383 (74627) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

524. /CDROM/140_HONP/HKAJIYA.BIN +0xEBD7 (60375) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

525. /CDROM/140_HONP/HMONSYOY.BIN +0xF76F (63343) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

526. /CDROM/140_HONP/KIKORI.BIN +0x378B7 (227511) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

527. /CDROM/140_HONP/MOGURA.BIN +0x183CB (99275) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

528. /CDROM/140_HONP/PARTYCE1.BIN +0x48C8B (298123) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

529. /CDROM/140_HONP/PARTYCH2.BIN +0x4750B (292107) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

530. /CDROM/140_HONP/PARTYCHG.BIN +0x4750B (292107) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

531. /CDROM/140_HONP/RBATTLE.BIN +0x4BBA7 (310183) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

532. /CDROM/140_HONP/REST.BIN +0xBC1F (48159) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

533. /CDROM/140_HONP/SOUKO.BIN +0x1DD2B (122155) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

534. /CDROM/140_HONP/STONE.BIN +0x2674F (157519) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

535. /CDROM/140_HONP/SYUGOITM.BIN +0xA0B7 (41143) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

536. /CDROM/140_HONP/VB19PIN.BIN +0x7DFF (32255) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

537. /CDROM/140_HONP/VG08PIN.BIN +0x7C63 (31843) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

538. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0xBAD3 (47827) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

539. /CDROM/270_BOOT/BOOT.BIN +0x2DEF7 (188151) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

540. /CDROM/270_BOOT/G1LOAD.BIN +0x21CE7 (138471) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

541. /CDROM/270_BOOT/OVER.BIN +0x3A92B (239915) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

542. /CDROM/280_GAME/EMBL.BIN +0x1347 (4935) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Cannot be targetted by enemy
     v1.1 TEXT:     Cannot be targeted by enemy 

543. /CDROM/010_ARA/VA05.BIN +0x4ABCA (306122) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

544. /CDROM/010_ARA/VA06.BIN +0x36ED2 (224978) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

545. /CDROM/010_ARA/VA08.BIN +0x38D76 (232822) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

546. /CDROM/010_ARA/VA24.BIN +0x39B0E (236302) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

547. /CDROM/020_ARB/VB04.BIN +0x42302 (271106) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

548. /CDROM/020_ARB/VB07.BIN +0x348CE (215246) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

549. /CDROM/020_ARB/VB09.BIN +0x2B366 (176998) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

550. /CDROM/020_ARB/VB10.BIN +0x38CCA (232650) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

551. /CDROM/020_ARB/VB12.BIN +0x3924A (234058) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

552. /CDROM/030_ARC/VC04.BIN +0x4A062 (303202) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

553. /CDROM/030_ARC/VC07.BIN +0x36D7A (224634) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

554. /CDROM/030_ARC/VC09.BIN +0x4334E (275278) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

555. /CDROM/030_ARC/VC28.BIN +0x3D96E (252270) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

556. /CDROM/030_ARC/VC30.BIN +0x2F336 (193334) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

557. /CDROM/040_ARD/VD07.BIN +0xCD02 (52482) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

558. /CDROM/050_ARE/VE06.BIN +0x476AE (292526) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

559. /CDROM/060_ARF/VF01.BIN +0x3CC56 (248918) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

560. /CDROM/060_ARF/VF02.BIN +0x4660E (288270) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

561. /CDROM/060_ARF/VF04.BIN +0x47662 (292450) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

562. /CDROM/090_ARI/VI05.BIN +0x371EE (225774) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

563. /CDROM/090_ARI/VI10.BIN +0x3C336 (246582) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

564. /CDROM/090_ARI/VI11.BIN +0x28182 (164226) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

565. /CDROM/100_ARJ/VJ24.BIN +0x2CA66 (182886) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

566. /CDROM/110_ARK/VK06.BIN +0x469AE (289198) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

567. /CDROM/130_SHOP/DOUGUYA1.BIN +0x118CE (71886) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

568. /CDROM/130_SHOP/DOUGUYA2.BIN +0x118CE (71886) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

569. /CDROM/130_SHOP/KAJIYA1.BIN +0xE2FE (58110) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

570. /CDROM/130_SHOP/KAJIYA2.BIN +0xE2FE (58110) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

571. /CDROM/130_SHOP/KANTEIY1.BIN +0xB496 (46230) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

572. /CDROM/130_SHOP/KANTEIY2.BIN +0xB496 (46230) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

573. /CDROM/130_SHOP/KOUEKI1.BIN +0xE05E (57438) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

574. /CDROM/130_SHOP/KOUEKI2.BIN +0xE05E (57438) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

575. /CDROM/130_SHOP/KPARTY1.BIN +0x7C0A (31754) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

576. /CDROM/130_SHOP/KPARTY2.BIN +0x7C0A (31754) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

577. /CDROM/130_SHOP/MONSYOY1.BIN +0xF76A (63338) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

578. /CDROM/130_SHOP/MONSYOY2.BIN +0xF76A (63338) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

579. /CDROM/130_SHOP/PARTYIN1.BIN +0xBED2 (48850) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

580. /CDROM/130_SHOP/PARTYIN2.BIN +0xBED2 (48850) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

581. /CDROM/140_HONP/FUDAZUK.BIN +0xD726 (55078) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

582. /CDROM/140_HONP/HDOUGUYA.BIN +0x123C2 (74690) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

583. /CDROM/140_HONP/HKAJIYA.BIN +0xEC16 (60438) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

584. /CDROM/140_HONP/HMONSYOY.BIN +0xF7AE (63406) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

585. /CDROM/140_HONP/KIKORI.BIN +0x378F6 (227574) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

586. /CDROM/140_HONP/MOGURA.BIN +0x1840A (99338) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

587. /CDROM/140_HONP/PARTYCE1.BIN +0x48CCA (298186) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

588. /CDROM/140_HONP/PARTYCH2.BIN +0x4754A (292170) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

589. /CDROM/140_HONP/PARTYCHG.BIN +0x4754A (292170) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

590. /CDROM/140_HONP/RBATTLE.BIN +0x4BBE6 (310246) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

591. /CDROM/140_HONP/REST.BIN +0xBC5E (48222) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

592. /CDROM/140_HONP/SOUKO.BIN +0x1DD6A (122218) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

593. /CDROM/140_HONP/STONE.BIN +0x2678E (157582) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

594. /CDROM/140_HONP/SYUGOITM.BIN +0xA0F6 (41206) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

595. /CDROM/140_HONP/VB19PIN.BIN +0x7E3E (32318) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

596. /CDROM/140_HONP/VG08PIN.BIN +0x7CA2 (31906) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

597. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0xBB12 (47890) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

598. /CDROM/270_BOOT/BOOT.BIN +0x2DF36 (188214) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

599. /CDROM/270_BOOT/G1LOAD.BIN +0x21D26 (138534) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

600. /CDROM/270_BOOT/OVER.BIN +0x3A96A (239978) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

601. /CDROM/280_GAME/EMBL.BIN +0x1386 (4998) - Reviewed spelling and text fit
     RETAIL HEX: 24151410122910151E151D29
     v1.2 HEX:   151410122910151E151D2910
     Meaning: targetted -> targeted; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Easy to be targetted by enemy
     v1.1 TEXT:     Easy to be targeted by enemy 

602. /CDROM/010_ARA/VA05.BIN +0x4B0D3 (307411) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

603. /CDROM/010_ARA/VA06.BIN +0x373DB (226267) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

604. /CDROM/010_ARA/VA08.BIN +0x3927F (234111) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

605. /CDROM/010_ARA/VA24.BIN +0x3A017 (237591) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

606. /CDROM/020_ARB/VB04.BIN +0x4280B (272395) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

607. /CDROM/020_ARB/VB07.BIN +0x34DD7 (216535) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

608. /CDROM/020_ARB/VB09.BIN +0x2B86F (178287) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

609. /CDROM/020_ARB/VB10.BIN +0x391D3 (233939) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

610. /CDROM/020_ARB/VB12.BIN +0x39753 (235347) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

611. /CDROM/030_ARC/VC04.BIN +0x4A56B (304491) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

612. /CDROM/030_ARC/VC07.BIN +0x37283 (225923) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

613. /CDROM/030_ARC/VC09.BIN +0x43857 (276567) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

614. /CDROM/030_ARC/VC28.BIN +0x3DE77 (253559) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

615. /CDROM/030_ARC/VC30.BIN +0x2F83F (194623) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

616. /CDROM/040_ARD/VD07.BIN +0xD20B (53771) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

617. /CDROM/050_ARE/VE06.BIN +0x47BB7 (293815) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

618. /CDROM/060_ARF/VF01.BIN +0x3D15F (250207) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

619. /CDROM/060_ARF/VF02.BIN +0x46B17 (289559) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

620. /CDROM/060_ARF/VF04.BIN +0x47B6B (293739) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

621. /CDROM/090_ARI/VI05.BIN +0x376F7 (227063) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

622. /CDROM/090_ARI/VI10.BIN +0x3C83F (247871) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

623. /CDROM/090_ARI/VI11.BIN +0x2868B (165515) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

624. /CDROM/100_ARJ/VJ24.BIN +0x2CF6F (184175) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

625. /CDROM/110_ARK/VK06.BIN +0x46EB7 (290487) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

626. /CDROM/130_SHOP/DOUGUYA1.BIN +0x11DD7 (73175) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

627. /CDROM/130_SHOP/DOUGUYA2.BIN +0x11DD7 (73175) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

628. /CDROM/130_SHOP/KAJIYA1.BIN +0x791C (31004) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00>

629. /CDROM/130_SHOP/KAJIYA1.BIN +0xE807 (59399) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

630. /CDROM/130_SHOP/KAJIYA2.BIN +0x791C (31004) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00>

631. /CDROM/130_SHOP/KAJIYA2.BIN +0xE807 (59399) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

632. /CDROM/130_SHOP/KANTEIY1.BIN +0xB99F (47519) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

633. /CDROM/130_SHOP/KANTEIY2.BIN +0xB99F (47519) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

634. /CDROM/130_SHOP/KOUEKI1.BIN +0xE567 (58727) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

635. /CDROM/130_SHOP/KOUEKI2.BIN +0xE567 (58727) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

636. /CDROM/130_SHOP/KPARTY1.BIN +0x8113 (33043) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

637. /CDROM/130_SHOP/KPARTY2.BIN +0x8113 (33043) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

638. /CDROM/130_SHOP/MONSYOY1.BIN +0xFC73 (64627) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

639. /CDROM/130_SHOP/MONSYOY2.BIN +0xFC73 (64627) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

640. /CDROM/130_SHOP/PARTYIN1.BIN +0xC3DB (50139) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

641. /CDROM/130_SHOP/PARTYIN2.BIN +0xC3DB (50139) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

642. /CDROM/140_HONP/FUDAZUK.BIN +0xDC2F (56367) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

643. /CDROM/140_HONP/HDOUGUYA.BIN +0x128CB (75979) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

644. /CDROM/140_HONP/HKAJIYA.BIN +0x8234 (33332) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00>

645. /CDROM/140_HONP/HKAJIYA.BIN +0xF11F (61727) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

646. /CDROM/140_HONP/HMONSYOY.BIN +0xFCB7 (64695) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

647. /CDROM/140_HONP/KIKORI.BIN +0x37DFF (228863) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

648. /CDROM/140_HONP/MOGURA.BIN +0x18913 (100627) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

649. /CDROM/140_HONP/PARTYCE1.BIN +0x491D3 (299475) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

650. /CDROM/140_HONP/PARTYCH2.BIN +0x47A53 (293459) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

651. /CDROM/140_HONP/PARTYCHG.BIN +0x47A53 (293459) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

652. /CDROM/140_HONP/RBATTLE.BIN +0x4C0EF (311535) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

653. /CDROM/140_HONP/REST.BIN +0xC167 (49511) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

654. /CDROM/140_HONP/SOUKO.BIN +0x1E273 (123507) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

655. /CDROM/140_HONP/STONE.BIN +0x26C97 (158871) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

656. /CDROM/140_HONP/SYUGOITM.BIN +0xA5FF (42495) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

657. /CDROM/140_HONP/VB19PIN.BIN +0x8347 (33607) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

658. /CDROM/140_HONP/VG08PIN.BIN +0x81AB (33195) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

659. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0xC01B (49179) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

660. /CDROM/270_BOOT/BOOT.BIN +0x2E43F (189503) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

661. /CDROM/270_BOOT/G1LOAD.BIN +0x2222F (139823) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

662. /CDROM/270_BOOT/OVER.BIN +0x3AE73 (241267) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

663. /CDROM/280_GAME/EMBL.BIN +0x188F (6287) - Reviewed spelling and text fit
     RETAIL HEX: 11231510201122242965103B4E4E104F4A6510514A4800
     v1.2 HEX:   1511231510201122242965103B4E4E104F4A6510514A48
     Meaning: Decrase -> Decrease; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: Decrase party, ATT UP, WPN<00><00><00><00><00><00>
     v1.1 TEXT:     Decrease party, ATT UP, WPN<00><00><00><00><00>

664. /CDROM/010_ARA/VA14.BIN +0x25FD (9725) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

665. /CDROM/010_ARA/VA17.BIN +0x255D (9565) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

666. /CDROM/010_ARA/VA18.BIN +0x4F15 (20245) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

667. /CDROM/010_ARA/VA19.BIN +0x249D (9373) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

668. /CDROM/010_ARA/VA20.BIN +0x2439 (9273) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

669. /CDROM/010_ARA/VA21.BIN +0x43C9 (17353) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

670. /CDROM/020_ARB/VB04.BIN +0x9B69 (39785) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

671. /CDROM/020_ARB/VB12.BIN +0xA5C5 (42437) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241023251414151E1C29101419232311201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F2522101211131B66A4
     v1.2 HEX:   23251414151E1C29101419231120201511221514660E5115101419141EA624101B1E1F2710271811241018112020151E1514660E4E18111E1B10171F1410291F25A62215101211131B66A4101010
     Meaning: dissapeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "You just suddenly dissapeared. / We didn't know what happened. / Thank god your back."
     v1.1 TEXT:     "You suddenly disappeared. / We didn't know what happened. / Thank god you're back."   

672. /CDROM/010_ARA/VA22.BIN +0x52D (1325) - Reviewed spelling and text fit
     RETAIL HEX: 191E1124151046111429103B1E1112151C1C1566
     v1.2 HEX:   23191E1124151046111429103B1E1112151C1C15
     Meaning: assasinate -> assassinate; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: But if I did, it would be that / I had to betray the City-State / and assasinate Lady Anabelle...."
     v1.1 TEXT:     But if I did, it would be that / I had to betray the City-State / and assassinate Lady Anabelle..."

673. /CDROM/010_ARA/VA24.BIN +0x695D (26973) - Reviewed spelling and text fit
     RETAIL HEX: 191E1124151046111429103B1E1112151C1C1566
     v1.2 HEX:   23191E1124151046111429103B1E1112151C1C15
     Meaning: assasinate -> assassinate; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: But if I did, it would be that / I had to betray the City-State / and assasinate Lady Anabelle...."
     v1.1 TEXT:     But if I did, it would be that / I had to betray the City-State / and assassinate Lady Anabelle..."

674. /CDROM/020_ARB/VB01.BIN +0x947 (2375) - Reviewed spelling and text fit
     RETAIL HEX: 241815101113131F1D1F141124191F1E230E241F1F10131F1D161F222411121C15651024181F25171866
     v1.2 HEX:   1113131F1D1D1F141124191F1E230E241F1F10131F1D161F222411121C15651024181F25171866101010
     Meaning: accomodations -> accommodations; bounded text fit: reviewed wording: the accommodations -> accommodations
     ORIGINAL TEXT: You may not find the accomodations / too comfortable, though.
     v1.1 TEXT:     You may not find accommodations / too comfortable, though.   

675. /CDROM/020_ARB/VB05.BIN +0x4E2F (20015) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

676. /CDROM/020_ARB/VB14.BIN +0x4063 (16483) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

677. /CDROM/020_ARB/VB18.BIN +0x555F (21855) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

678. /CDROM/030_ARC/VC21.BIN +0x16D63 (93539) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

679. /CDROM/040_ARD/VD01.BIN +0x554B (21835) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

680. /CDROM/050_ARE/VE07.BIN +0x900B (36875) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

681. /CDROM/070_ARG/VG08.BIN +0x517F (20863) - Reviewed spelling and text fit
     RETAIL HEX: 241113180E271819131868
     v1.2 HEX:   1113180E27181913186810
     Meaning: Dettach -> Detach; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Dettach / which?
     v1.1 TEXT:     Detach / which? 

682. /CDROM/030_ARC/VC01.BIN +0xDAB4 (55988) - Reviewed spelling and text fit
     RETAIL HEX: 1E2910271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D2418191E170E16221F1D1011101415112210162219151E1468A4
     v1.2 HEX:   10271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D152418191E170E16221F1D1011101415112210162219151E1468A410
     Meaning: somthing -> something; bounded text fit: reviewed wording: any worse thing -> a worse thing
     ORIGINAL TEXT: Can there be any worse thing in / the world than to lose somthing / from a dear friend?"
     v1.1 TEXT:     Can there be a worse thing in / the world than to lose something / from a dear friend?" 

683. /CDROM/030_ARC/VC21.BIN +0x137C4 (79812) - Reviewed spelling and text fit
     RETAIL HEX: 1E2910271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D2418191E170E16221F1D1011101415112210162219151E1468A4
     v1.2 HEX:   10271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D152418191E170E16221F1D1011101415112210162219151E1468A410
     Meaning: somthing -> something; bounded text fit: reviewed wording: any worse thing -> a worse thing
     ORIGINAL TEXT: Can there be any worse thing in / the world than to lose somthing / from a dear friend?"
     v1.1 TEXT:     Can there be a worse thing in / the world than to lose something / from a dear friend?" 

684. /CDROM/030_ARC/VC24.BIN +0x9EE0 (40672) - Reviewed spelling and text fit
     RETAIL HEX: 1E2910271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D2418191E170E16221F1D1011101415112210162219151E1468A4
     v1.2 HEX:   10271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D152418191E170E16221F1D1011101415112210162219151E1468A410
     Meaning: somthing -> something; bounded text fit: reviewed wording: any worse thing -> a worse thing
     ORIGINAL TEXT: Can there be any worse thing in / the world than to lose somthing / from a dear friend?"
     v1.1 TEXT:     Can there be a worse thing in / the world than to lose something / from a dear friend?" 

685. /CDROM/030_ARC/VC26.BIN +0x21FC (8700) - Reviewed spelling and text fit
     RETAIL HEX: 1E2910271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D2418191E170E16221F1D1011101415112210162219151E1468A4
     v1.2 HEX:   10271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D152418191E170E16221F1D1011101415112210162219151E1468A410
     Meaning: somthing -> something; bounded text fit: reviewed wording: any worse thing -> a worse thing
     ORIGINAL TEXT: Can there be any worse thing in / the world than to lose somthing / from a dear friend?"
     v1.1 TEXT:     Can there be a worse thing in / the world than to lose something / from a dear friend?" 

686. /CDROM/040_ARD/VD02.BIN +0xC870 (51312) - Reviewed spelling and text fit
     RETAIL HEX: 1E2910271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D2418191E170E16221F1D1011101415112210162219151E1468A4
     v1.2 HEX:   10271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D152418191E170E16221F1D1011101415112210162219151E1468A410
     Meaning: somthing -> something; bounded text fit: reviewed wording: any worse thing -> a worse thing
     ORIGINAL TEXT: Can there be any worse thing in / the world than to lose somthing / from a dear friend?"
     v1.1 TEXT:     Can there be a worse thing in / the world than to lose something / from a dear friend?" 

687. /CDROM/060_ARF/VF05.BIN +0xB868 (47208) - Reviewed spelling and text fit
     RETAIL HEX: 1E2910271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D2418191E170E16221F1D1011101415112210162219151E1468A4
     v1.2 HEX:   10271F222315102418191E1710191E0E24181510271F221C14102418111E10241F101C1F231510231F1D152418191E170E16221F1D1011101415112210162219151E1468A410
     Meaning: somthing -> something; bounded text fit: reviewed wording: any worse thing -> a worse thing
     ORIGINAL TEXT: Can there be any worse thing in / the world than to lose somthing / from a dear friend?"
     v1.1 TEXT:     Can there be a worse thing in / the world than to lose something / from a dear friend?" 

688. /CDROM/040_ARD/VD03.BIN +0x7B17 (31511) - Reviewed spelling and text fit
     RETAIL HEX: 1415131923191F1E6610531F25101D25231EA6240E121C111D1510291F252223151C1610152615222924191D150E231F1D152418191E17101211141018112020151E2310241F10291F25220E161F1C1C1F2715222366A4
     v1.2 HEX:   13181F1913156610531F25101D2523241EA6240E121C111D1510291F252223151C1610151113181024191D150E231F1D152418191E17101211141018112020151E2310241F10291F25220E161F1C1C1F2715222366A410
     Meaning: everytime -> each time; musn't -> mustn't; bounded text fit: reviewed wording: decision -> choice
     ORIGINAL TEXT: It's our decision. You musn't / blame yourself everytime / something bad happens to your / followers."
     v1.1 TEXT:     It's our choice. You mustn't / blame yourself each time / something bad happens to your / followers." 

689. /CDROM/040_ARD/VD17.BIN +0x9047 (36935) - Reviewed spelling and text fit
     RETAIL HEX: 1415131923191F1E6610531F25101D25231EA6240E121C111D1510291F252223151C1610152615222924191D150E231F1D152418191E17101211141018112020151E2310241F10291F25220E161F1C1C1F2715222366A4
     v1.2 HEX:   13181F1913156610531F25101D2523241EA6240E121C111D1510291F252223151C1610151113181024191D150E231F1D152418191E17101211141018112020151E2310241F10291F25220E161F1C1C1F2715222366A410
     Meaning: everytime -> each time; musn't -> mustn't; bounded text fit: reviewed wording: decision -> choice
     ORIGINAL TEXT: It's our decision. You musn't / blame yourself everytime / something bad happens to your / followers."
     v1.1 TEXT:     It's our choice. You mustn't / blame yourself each time / something bad happens to your / followers." 

690. /CDROM/040_ARD/VD04.BIN +0xAE1E (44574) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122191E176666660E51151013111EA624101A2523241019171E1F2215102418192367676767A4
     v1.2 HEX:   112020151122191E176666660E51151013111EA624101A2523241019171E1F2215102418192367676767A410
     Meaning: dissappearing -> disappearing; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "So he's the reason little girls / have been dissappearing... / We can't just ignore this!!!!"
     v1.1 TEXT:     "So he's the reason little girls / have been disappearing... / We can't just ignore this!!!!" 

691. /CDROM/040_ARD/VD05.BIN +0x898D (35213) - Reviewed spelling and text fit
     RETAIL HEX: 2410291F25660E4A1C1511231510171F10252010241F10241815109A1E1410161C1F1F2266A4
     v1.2 HEX:   252410291F25660E4A1C1511231510171F10241F10241815109A1E1410161C1F1F2266A41010
     Meaning: abot -> about; bounded text fit: reviewed wording: Please go up to -> Please go to
     ORIGINAL TEXT: "Richmond told me abot you. / Please go up to the 2nd floor."
     v1.1 TEXT:     "Richmond told me about you. / Please go to the 2nd floor."  

692. /CDROM/040_ARD/VD19.BIN +0x7AD5 (31445) - Reviewed spelling and text fit
     RETAIL HEX: 2410291F25660E4A1C1511231510171F10252010241F10241815109A1E1410161C1F1F2266A4
     v1.2 HEX:   252410291F25660E4A1C1511231510171F10241F10241815109A1E1410161C1F1F2266A41010
     Meaning: abot -> about; bounded text fit: reviewed wording: Please go up to -> Please go to
     ORIGINAL TEXT: "Richmond told me abot you. / Please go up to the 2nd floor."
     v1.1 TEXT:     "Richmond told me about you. / Please go to the 2nd floor."  

693. /CDROM/040_ARD/VD06.BIN +0x44CC2 (281794) - Reviewed spelling and text fit
     RETAIL HEX: 1F
     v1.2 HEX:   15
     Meaning: Sorceror -> Sorcerer; bounded text fit: no wording adjustment
     ORIGINAL TEXT: <E4>xe<80><E8>xe<80><FC>re<80>?se<80><30>ue<80><E4>we<80>Sorceror
     v1.1 TEXT:     <E4>xe<80><E8>xe<80><FC>re<80>?se<80><30>ue<80><E4>we<80>Sorcerer

694. /CDROM/040_ARD/VD10.BIN +0x19FE6 (106470) - Reviewed spelling and text fit
     RETAIL HEX: 1F
     v1.2 HEX:   15
     Meaning: Sorceror -> Sorcerer; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Sorceror
     v1.1 TEXT:     Sorcerer

695. /CDROM/040_ARD/VD11.BIN +0x1C55A (116058) - Reviewed spelling and text fit
     RETAIL HEX: 1F
     v1.2 HEX:   15
     Meaning: Sorceror -> Sorcerer; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Sorceror
     v1.1 TEXT:     Sorcerer

696. /CDROM/040_ARD/VD12.BIN +0x1A852 (108626) - Reviewed spelling and text fit
     RETAIL HEX: 1F
     v1.2 HEX:   15
     Meaning: Sorceror -> Sorcerer; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Sorceror
     v1.1 TEXT:     Sorcerer

697. /CDROM/040_ARD/VD13.BIN +0x25946 (153926) - Reviewed spelling and text fit
     RETAIL HEX: 1F
     v1.2 HEX:   15
     Meaning: Sorceror -> Sorcerer; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Sorceror
     v1.1 TEXT:     Sorcerer

698. /CDROM/040_ARD/VD07.BIN +0x4634 (17972) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122191E1767676767676767676767
     v1.2 HEX:   112020151122191E176767676767676767676710
     Meaning: dissappearing -> disappearing; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is dissappearing!!!!!!!!!!
     v1.1 TEXT:     Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is disappearing!!!!!!!!!! 

699. /CDROM/040_ARD/VD07.BIN +0x4A23 (18979) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122191E1767676767676767676767
     v1.2 HEX:   112020151122191E176767676767676767676710
     Meaning: dissappearing -> disappearing; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is dissappearing!!!!!!!!!!
     v1.1 TEXT:     Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is disappearing!!!!!!!!!! 

700. /CDROM/040_ARD/VD09.BIN +0x32E0 (13024) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122191E1767676767676767676767
     v1.2 HEX:   112020151122191E176767676767676767676710
     Meaning: dissappearing -> disappearing; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is dissappearing!!!!!!!!!!
     v1.1 TEXT:     Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is disappearing!!!!!!!!!! 

701. /CDROM/040_ARD/VD09.BIN +0x36CF (14031) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122191E1767676767676767676767
     v1.2 HEX:   112020151122191E176767676767676767676710
     Meaning: dissappearing -> disappearing; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is dissappearing!!!!!!!!!!
     v1.1 TEXT:     Excellent!!!!! Excellent!!!!!! / The rumbling in my body!!!!! / The thirst that scorched my flesh! / It is disappearing!!!!!!!!!! 

702. /CDROM/040_ARD/VD17.BIN +0xEE34 (60980) - Reviewed spelling and text fit
     RETAIL HEX: 261510191E101D2910181511222410241811240E291F251013111E1027191E66A4
     v1.2 HEX:   15261510191E101D291018151122240E291F251013111E1027191E66A410101010
     Meaning: belive -> believe; bounded text fit: reviewed wording: I believe in my heart that -> I believe in my heart
     ORIGINAL TEXT: . / I belive in my heart that / you can win."
     v1.1 TEXT:     . / I believe in my heart / you can win."    

703. /CDROM/050_ARE/VE01.BIN +0x7B30 (31536) - Reviewed spelling and text fit
     RETAIL HEX: 1914
     v1.2 HEX:   1419
     Meaning: soliders -> soldiers; bounded text fit: no wording adjustment
     ORIGINAL TEXT: The Academy seems safe, but / the town's crawling with Highland / soliders, so be careful. See ya!"
     v1.1 TEXT:     The Academy seems safe, but / the town's crawling with Highland / soldiers, so be careful. See ya!"

704. /CDROM/050_ARE/VE06.BIN +0xA9A4 (43428) - Reviewed spelling and text fit
     RETAIL HEX: 1914
     v1.2 HEX:   1419
     Meaning: soliders -> soldiers; bounded text fit: no wording adjustment
     ORIGINAL TEXT: The Academy seems safe, but / the town's crawling with Highland / soliders, so be careful. See ya!"
     v1.1 TEXT:     The Academy seems safe, but / the town's crawling with Highland / soldiers, so be careful. See ya!"

705. /CDROM/050_ARE/VE13.BIN +0x8D84 (36228) - Reviewed spelling and text fit
     RETAIL HEX: 1914
     v1.2 HEX:   1419
     Meaning: soliders -> soldiers; bounded text fit: no wording adjustment
     ORIGINAL TEXT: The Academy seems safe, but / the town's crawling with Highland / soliders, so be careful. See ya!"
     v1.1 TEXT:     The Academy seems safe, but / the town's crawling with Highland / soldiers, so be careful. See ya!"

706. /CDROM/050_ARE/VE16.BIN +0x73C8 (29640) - Reviewed spelling and text fit
     RETAIL HEX: 1914
     v1.2 HEX:   1419
     Meaning: soliders -> soldiers; bounded text fit: no wording adjustment
     ORIGINAL TEXT: The Academy seems safe, but / the town's crawling with Highland / soliders, so be careful. See ya!"
     v1.1 TEXT:     The Academy seems safe, but / the town's crawling with Highland / soldiers, so be careful. See ya!"

707. /CDROM/050_ARE/VE07.BIN +0xB0F4 (45300) - Reviewed spelling and text fit
     RETAIL HEX: 22231013111C1C101924666666680E3B1810291523651014152324191E2966104324A6231014152324191E2966
     v1.2 HEX:   2522231013111C1C101924666666680E531523651014152324191E2966104324A6231014152324191E29661010
     Meaning: troubadors -> troubadours; bounded text fit: reviewed wording: Ah yes -> Yes
     ORIGINAL TEXT: Why, you ask? Tee-hee. / What do the troubadors call it...? / Ah yes, destiny. It's destiny.
     v1.1 TEXT:     Why, you ask? Tee-hee. / What do the troubadours call it...? / Yes, destiny. It's destiny.  

708. /CDROM/050_ARE/VE07.BIN +0x136E0 (79584) - Reviewed spelling and text fit
     RETAIL HEX: 2315111318191E170E161F221011104142494D4E666666A4
     v1.2 HEX:   1C1F1F1B191E170E161F221011104142494D4E666666A410
     Meaning: seaching -> looking; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Come on, we're seaching / for a GHOST..."
     v1.1 TEXT:     "Come on, we're looking / for a GHOST..." 

709. /CDROM/050_ARE/VE08.BIN +0xBE29 (48681) - Reviewed spelling and text fit
     RETAIL HEX: 24181510111914101F16104E271F104C19261522650E2715101122151EA62410191E101110201F2319241F1E10241F10271117150E27112210111711191E232410421917181C111E14A623101D11191E1011221D2966
     v1.2 HEX:   111914101F16104E271F104C19261522650E2715101122151EA62410191E101110201F231924191F1E10241F10271117150E27112210111711191E232410421917181C111E14A623101D11191E1011221D2966101010
     Meaning: positon -> position; bounded text fit: reviewed wording: the aid -> aid
     ORIGINAL TEXT: Even with the aid of Two River, / we aren't in a positon to wage / war against Highland's main army.
     v1.1 TEXT:     Even with aid of Two River, / we aren't in a position to wage / war against Highland's main army.   

710. /CDROM/050_ARE/VE14.BIN +0xBE5D (48733) - Reviewed spelling and text fit
     RETAIL HEX: 24181510111914101F16104E271F104C19261522650E2715101122151EA62410191E101110201F2319241F1E10241F10271117150E27112210111711191E232410421917181C111E14A623101D11191E1011221D2966
     v1.2 HEX:   111914101F16104E271F104C19261522650E2715101122151EA62410191E101110201F231924191F1E10241F10271117150E27112210111711191E232410421917181C111E14A623101D11191E1011221D2966101010
     Meaning: positon -> position; bounded text fit: reviewed wording: the aid -> aid
     ORIGINAL TEXT: Even with the aid of Two River, / we aren't in a positon to wage / war against Highland's main army.
     v1.1 TEXT:     Even with aid of Two River, / we aren't in a position to wage / war against Highland's main army.   

711. /CDROM/060_ARF/VF04.BIN +0x9D28 (40232) - Reviewed spelling and text fit
     RETAIL HEX: 111C231F10191E10241F271E10161F220E1D191C1924112229102422111E191E171015281522131923152366
     v1.2 HEX:   191E10241F271E10161F220E1D191C192411222910242211191E191E17101528152213192315236610101010
     Meaning: traning -> training; bounded text fit: reviewed wording: is also in town for -> is in town for
     ORIGINAL TEXT: "Kasumi, the Vice-Chancellor of / Rokkaku, is also in town for / military traning exercises. 
     v1.1 TEXT:     "Kasumi, the Vice-Chancellor of / Rokkaku, is in town for / military training exercises.     

712. /CDROM/060_ARF/VF04.BIN +0xB8F3 (47347) - Reviewed spelling and text fit
     RETAIL HEX: 161F2210191E14152015
     v1.2 HEX:   1F1610191E141520151E
     Meaning: indepedence -> independence; bounded text fit: reviewed wording: for independence -> of independence
     ORIGINAL TEXT: "This is the 'Blinking Mirror,' / one of the treasures of the Toran / Republic. It was used in our war / for indepedence, but now I 
     v1.1 TEXT:     "This is the 'Blinking Mirror,' / one of the treasures of the Toran / Republic. It was used in our war / of independence, but now I 

713. /CDROM/110_ARK/VK01.BIN +0x9AD7 (39639) - Reviewed spelling and text fit
     RETAIL HEX: 161F2210191E14152015
     v1.2 HEX:   1F1610191E141520151E
     Meaning: indepedence -> independence; bounded text fit: reviewed wording: for independence -> of independence
     ORIGINAL TEXT: "This is the 'Blinking Mirror,' / one of the treasures of the Toran / Republic. It was used in our war / for indepedence, but now I 
     v1.1 TEXT:     "This is the 'Blinking Mirror,' / one of the treasures of the Toran / Republic. It was used in our war / of independence, but now I 

714. /CDROM/070_ARG/VG01.BIN +0x5EDD (24285) - Reviewed spelling and text fit
     RETAIL HEX: 1417
     v1.2 HEX:   1714
     Meaning: kindgom -> kingdom; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Thus, Lord Gustav and citizens, / I'd like you all to leave. Of / course if you become a zombie / you can stay in my kindgom."
     v1.1 TEXT:     Thus, Lord Gustav and citizens, / I'd like you all to leave. Of / course if you become a zombie / you can stay in my kingdom."

715. /CDROM/070_ARG/VG14.BIN +0x1385 (4997) - Reviewed spelling and text fit
     RETAIL HEX: 1417
     v1.2 HEX:   1714
     Meaning: kindgom -> kingdom; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Thus, Lord Gustav and citizens, / I'd like you all to leave. Of / course if you become a zombie / you can stay in my kindgom."
     v1.1 TEXT:     Thus, Lord Gustav and citizens, / I'd like you all to leave. Of / course if you become a zombie / you can stay in my kingdom."

716. /CDROM/070_ARG/VG17.BIN +0x4B79 (19321) - Reviewed spelling and text fit
     RETAIL HEX: 1417
     v1.2 HEX:   1714
     Meaning: kindgom -> kingdom; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Thus, Lord Gustav and citizens, / I'd like you all to leave. Of / course if you become a zombie / you can stay in my kindgom."
     v1.1 TEXT:     Thus, Lord Gustav and citizens, / I'd like you all to leave. Of / course if you become a zombie / you can stay in my kingdom."

717. /CDROM/070_ARG/VG03.BIN +0x3A79 (14969) - Reviewed spelling and text fit
     RETAIL HEX: 1D111E1117151410241F101523131120156510122524101E1F1F1E15101B1E1F27230E2718152215104415232310111E14104211252315221011221566A4
     v1.2 HEX:   152313112015146510122524101E1F101F1E15101B1E1F27230E2718152215104415232310111E14104211252315221011221566A4101010101010101010
     Meaning: noone -> no one; bounded text fit: reviewed wording: managed to escape -> escaped
     ORIGINAL TEXT: "The troops we sent really got hit / hard. Apparently Klaus and Ridley / managed to escape, but noone knows / where Jess and Hauser are."
     v1.1 TEXT:     "The troops we sent really got hit / hard. Apparently Klaus and Ridley / escaped, but no one knows / where Jess and Hauser are."         

718. /CDROM/070_ARG/VG13.BIN +0x6B25 (27429) - Reviewed spelling and text fit
     RETAIL HEX: 1D111E1117151410241F101523131120156510122524101E1F1F1E15101B1E1F27230E2718152215104415232310111E14104211252315221011221566A4
     v1.2 HEX:   152313112015146510122524101E1F101F1E15101B1E1F27230E2718152215104415232310111E14104211252315221011221566A4101010101010101010
     Meaning: noone -> no one; bounded text fit: reviewed wording: managed to escape -> escaped
     ORIGINAL TEXT: "The troops we sent really got hit / hard. Apparently Klaus and Ridley / managed to escape, but noone knows / where Jess and Hauser are."
     v1.1 TEXT:     "The troops we sent really got hit / hard. Apparently Klaus and Ridley / escaped, but no one knows / where Jess and Hauser are."         

719. /CDROM/070_ARG/VG06.BIN +0x6BF0 (27632) - Reviewed spelling and text fit
     RETAIL HEX: 1914
     v1.2 HEX:   1419
     Meaning: soliders -> soldiers; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "I want to go see my friend who's / in Crom Village, but the Tinto / soliders won't let me pass. It's / the fault of the Highland Army..."
     v1.1 TEXT:     "I want to go see my friend who's / in Crom Village, but the Tinto / soldiers won't let me pass. It's / the fault of the Highland Army..."

720. /CDROM/070_ARG/VG08.BIN +0xA108 (41224) - Reviewed spelling and text fit
     RETAIL HEX: 104E1815104619261523101F1610241815104215221F
     v1.2 HEX:   4E1815104619261523101F1610241815104215221F15
     Meaning: Heros -> Heroes; bounded text fit: collapse double space
     ORIGINAL TEXT:  /       The Lives of the Heros
     v1.1 TEXT:      /      The Lives of the Heroes

721. /CDROM/070_ARG/VG18.BIN +0xB41C (46108) - Reviewed spelling and text fit
     RETAIL HEX: 104E1815104619261523101F1610241815104215221F
     v1.2 HEX:   4E1815104619261523101F1610241815104215221F15
     Meaning: Heros -> Heroes; bounded text fit: collapse double space
     ORIGINAL TEXT:  /       The Lives of the Heros
     v1.1 TEXT:      /      The Lives of the Heroes

722. /CDROM/080_ARH/VH02.BIN +0x71D9 (29145) - Reviewed spelling and text fit
     RETAIL HEX: 151410111624152210291F2522
     v1.2 HEX:   24151410111624152210241815
     Meaning: exhaused -> exhausted; bounded text fit: reviewed wording: after your -> after the
     ORIGINAL TEXT: "If you're exhaused after your / journey, why not rest here?"
     v1.1 TEXT:     "If you're exhausted after the / journey, why not rest here?"

723. /CDROM/090_ARI/VI01.BIN +0x68F3 (26867) - Reviewed spelling and text fit
     RETAIL HEX: 201F23152323101F25221018151122242310111E14101F25220E231B191C1C2366104D2522151C2910241815291027191C1C1011191410291F2566A4
     v1.2 HEX:   18112615101F25221018151122242310111E14101F25220E231B191C1C2366104D2522151C2910241815291027191C1C1011191410291F2566A41010
     Meaning: posess -> have; bounded text fit: no wording adjustment
     ORIGINAL TEXT: We are no longer Knights, but we / still posess our hearts and our / skills. Surely they will aid you."
     v1.1 TEXT:     We are no longer Knights, but we / still have our hearts and our / skills. Surely they will aid you."  

724. /CDROM/090_ARI/VI04.BIN +0x1FAF (8111) - Reviewed spelling and text fit
     RETAIL HEX: 201F23152323101F25221018151122242310111E14101F25220E231B191C1C2366104D2522151C2910241815291027191C1C1011191410291F2566A4
     v1.2 HEX:   18112615101F25221018151122242310111E14101F25220E231B191C1C2366104D2522151C2910241815291027191C1C1011191410291F2566A41010
     Meaning: posess -> have; bounded text fit: no wording adjustment
     ORIGINAL TEXT: We are no longer Knights, but we / still posess our hearts and our / skills. Surely they will aid you."
     v1.1 TEXT:     We are no longer Knights, but we / still have our hearts and our / skills. Surely they will aid you."  

725. /CDROM/090_ARI/VI05.BIN +0x65BF (26047) - Reviewed spelling and text fit
     RETAIL HEX: 201F23152323101F25221018151122242310111E14101F25220E231B191C1C2366104D2522151C2910241815291027191C1C1011191410291F2566A4
     v1.2 HEX:   18112615101F25221018151122242310111E14101F25220E231B191C1C2366104D2522151C2910241815291027191C1C1011191410291F2566A41010
     Meaning: posess -> have; bounded text fit: no wording adjustment
     ORIGINAL TEXT: We are no longer Knights, but we / still posess our hearts and our / skills. Surely they will aid you."
     v1.1 TEXT:     We are no longer Knights, but we / still have our hearts and our / skills. Surely they will aid you."  

726. /CDROM/090_ARI/VI12.BIN +0x5FCE (24526) - Reviewed spelling and text fit
     RETAIL HEX: 1519
     v1.2 HEX:   1915
     Meaning: weild -> wield; bounded text fit: no wording adjustment
     ORIGINAL TEXT: , / I will weild this sword again."
     v1.1 TEXT:     , / I will wield this sword again."

727. /CDROM/090_ARI/VI12.BIN +0x6D2B (27947) - Reviewed spelling and text fit
     RETAIL HEX: 1123
     v1.2 HEX:   1311
     Meaning: Ocassionally -> Occasionally; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Ocassionally the Knights / recruit from even us plains / folk."
     v1.1 TEXT:     "Occasionally the Knights / recruit from even us plains / folk."

728. /CDROM/090_ARI/VI12.BIN +0x7723 (30499) - Reviewed spelling and text fit
     RETAIL HEX: 1123
     v1.2 HEX:   1311
     Meaning: Ocassionally -> Occasionally; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Ocassionally the Knights / recruit from even us plains / folk."
     v1.1 TEXT:     "Occasionally the Knights / recruit from even us plains / folk."

729. /CDROM/100_ARJ/VJ16.BIN +0x2AA6 (10918) - Reviewed spelling and text fit
     RETAIL HEX: 1915
     v1.2 HEX:   1519
     Meaning: wierd -> weird; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "There's nobody here? / Isn't this wierd, 
     v1.1 TEXT:     "There's nobody here? / Isn't this weird, 

730. /CDROM/100_ARJ/VJ17.BIN +0x3C06 (15366) - Reviewed spelling and text fit
     RETAIL HEX: 191E1124191F1E6510241815109A0E1611131523101F161024181510421F271C191E1710501F191315104125191C1466
     v1.2 HEX:   23191E1124191F1E651024271F0E1611131523101F161024181510421F271C191E1710501F191315104125191C146610
     Meaning: Assasination -> Assassination; bounded text fit: reviewed wording: the 2 -> two
     ORIGINAL TEXT: Protection and Assasination, the 2 / faces of the Howling Voice Guild.
     v1.1 TEXT:     Protection and Assassination, two / faces of the Howling Voice Guild. 

731. /CDROM/110_ARK/VK01.BIN +0x9F2E (40750) - Reviewed spelling and text fit
     RETAIL HEX: 11
     v1.2 HEX:   15
     Meaning: independant -> independent; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Officially the Knights will stay / independant in return for helping / Highland, but in effect they've / become puppets of Highland."
     v1.1 TEXT:     "Officially the Knights will stay / independent in return for helping / Highland, but in effect they've / become puppets of Highland."

732. /CDROM/110_ARK/VK10.BIN +0x14C76 (85110) - Reviewed spelling and text fit
     RETAIL HEX: 11
     v1.2 HEX:   15
     Meaning: independant -> independent; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Officially the Knights will stay / independant in return for helping / Highland, but in effect they've / become puppets of Highland."
     v1.1 TEXT:     "Officially the Knights will stay / independent in return for helping / Highland, but in effect they've / become puppets of Highland."

733. /CDROM/110_ARK/VK34.BIN +0xBF3A (48954) - Reviewed spelling and text fit
     RETAIL HEX: 11
     v1.2 HEX:   15
     Meaning: independant -> independent; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Officially the Knights will stay / independant in return for helping / Highland, but in effect they've / become puppets of Highland."
     v1.1 TEXT:     "Officially the Knights will stay / independent in return for helping / Highland, but in effect they've / become puppets of Highland."

734. /CDROM/110_ARK/VK03.BIN +0x375B (14171) - Reviewed spelling and text fit
     RETAIL HEX: 1C192429101F16102418150E1C1926191E1710241F1022151D151D1215221024181510122211261522290E1F161024181F23151027181F101419151466
     v1.2 HEX:   191C192429101F16102418150E1C1926191E1710241F1022151D151D1215221024181510122211261522290E1F161024181F23151027181F1014191514
     Meaning: responsiblity -> responsibility; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: "It's the responsiblity of the / living to remember the bravery / of those who died....."
     v1.1 TEXT:     "It's the responsibility of the / living to remember the bravery / of those who died...."

735. /CDROM/110_ARK/VK04.BIN +0x7887 (30855) - Reviewed spelling and text fit
     RETAIL HEX: 241810111C1C101D29101D1917182466A4
     v1.2 HEX:   1924181016251C1C10161F22131566A410
     Meaning: wth -> with; bounded text fit: reviewed wording: all my might -> full force
     ORIGINAL TEXT:  Army, / I'll fight wth all my might."
     v1.1 TEXT:      Army, / I'll fight with full force." 

736. /CDROM/110_ARK/VK04.BIN +0x94D7 (38103) - Reviewed spelling and text fit
     RETAIL HEX: 241810111C1C101D29101D1917182466A4
     v1.2 HEX:   1924181016251C1C10161F22131566A410
     Meaning: wth -> with; bounded text fit: reviewed wording: all my might -> full force
     ORIGINAL TEXT:  Army, / I'll fight wth all my might."
     v1.1 TEXT:      Army, / I'll fight with full force." 

737. /CDROM/110_ARK/VK04.BIN +0x9D27 (40231) - Reviewed spelling and text fit
     RETAIL HEX: 241810111C1C101D29101D1917182466A4
     v1.2 HEX:   1924181016251C1C10161F22131566A410
     Meaning: wth -> with; bounded text fit: reviewed wording: all my might -> full force
     ORIGINAL TEXT:  Army, / I'll fight wth all my might."
     v1.1 TEXT:      Army, / I'll fight with full force." 

738. /CDROM/110_ARK/VK05.BIN +0x7357 (29527) - Reviewed spelling and text fit
     RETAIL HEX: 241810111C1C101D29101D1917182466A4
     v1.2 HEX:   1924181016251C1C10161F22131566A410
     Meaning: wth -> with; bounded text fit: reviewed wording: all my might -> full force
     ORIGINAL TEXT:  Army, / I'll fight wth all my might."
     v1.1 TEXT:      Army, / I'll fight with full force." 

739. /CDROM/110_ARK/VK05.BIN +0x8FA7 (36775) - Reviewed spelling and text fit
     RETAIL HEX: 241810111C1C101D29101D1917182466A4
     v1.2 HEX:   1924181016251C1C10161F22131566A410
     Meaning: wth -> with; bounded text fit: reviewed wording: all my might -> full force
     ORIGINAL TEXT:  Army, / I'll fight wth all my might."
     v1.1 TEXT:      Army, / I'll fight with full force." 

740. /CDROM/110_ARK/VK05.BIN +0x97F7 (38903) - Reviewed spelling and text fit
     RETAIL HEX: 241810111C1C101D29101D1917182466A4
     v1.2 HEX:   1924181016251C1C10161F22131566A410
     Meaning: wth -> with; bounded text fit: reviewed wording: all my might -> full force
     ORIGINAL TEXT:  Army, / I'll fight wth all my might."
     v1.1 TEXT:      Army, / I'll fight with full force." 

741. /CDROM/110_ARK/VK04.BIN +0x7C97 (31895) - Reviewed spelling and text fit
     RETAIL HEX: 111E29101D1F22150E191E2415222324191E171023241F2219152310241F1024151C1C66A4
     v1.2 HEX:   1D1F22150E191E241522152324191E171023241F2219152310241F1024151C1C66A4101010
     Meaning: intersting -> interesting; bounded text fit: reviewed wording: any more -> more
     ORIGINAL TEXT: "What is it sonny? / Granny doesn't have any more / intersting stories to tell."
     v1.1 TEXT:     "What is it sonny? / Granny doesn't have more / interesting stories to tell."   

742. /CDROM/110_ARK/VK05.BIN +0x7767 (30567) - Reviewed spelling and text fit
     RETAIL HEX: 111E29101D1F22150E191E2415222324191E171023241F2219152310241F1024151C1C66A4
     v1.2 HEX:   1D1F22150E191E241522152324191E171023241F2219152310241F1024151C1C66A4101010
     Meaning: intersting -> interesting; bounded text fit: reviewed wording: any more -> more
     ORIGINAL TEXT: "What is it sonny? / Granny doesn't have any more / intersting stories to tell."
     v1.1 TEXT:     "What is it sonny? / Granny doesn't have more / interesting stories to tell."   

743. /CDROM/110_ARK/VK07.BIN +0x12C7C (76924) - Reviewed spelling and text fit
     RETAIL HEX: 19
     v1.2 HEX:   24
     Meaning: liitle -> little; bounded text fit: no wording adjustment
     ORIGINAL TEXT: b<80>"Don't worry, liitle brother. / Your big sister will protect you."
     v1.1 TEXT:     b<80>"Don't worry, little brother. / Your big sister will protect you."

744. /CDROM/110_ARK/VK07.BIN +0x12E68 (77416) - Reviewed spelling and text fit
     RETAIL HEX: 19
     v1.2 HEX:   24
     Meaning: liitle -> little; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Don't worry, liitle brother. / Your big sister will protect you."
     v1.1 TEXT:     "Don't worry, little brother. / Your big sister will protect you."

745. /CDROM/110_ARK/VK07.BIN +0x15B04 (88836) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

746. /CDROM/110_ARK/VK07.BIN +0x15C3C (89148) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

747. /CDROM/110_ARK/VK07.BIN +0x15D48 (89416) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

748. /CDROM/110_ARK/VK10.BIN +0x177FC (96252) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

749. /CDROM/110_ARK/VK10.BIN +0x178F8 (96504) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

750. /CDROM/110_ARK/VK10.BIN +0x179EC (96748) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

751. /CDROM/110_ARK/VK10.BIN +0x17AE0 (96992) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

752. /CDROM/110_ARK/VK10.BIN +0x17BA8 (97192) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

753. /CDROM/110_ARK/VK10.BIN +0x17CE0 (97504) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

754. /CDROM/110_ARK/VK24.BIN +0xC064 (49252) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

755. /CDROM/110_ARK/VK24.BIN +0xC160 (49504) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

756. /CDROM/110_ARK/VK24.BIN +0xC254 (49748) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

757. /CDROM/110_ARK/VK24.BIN +0xC348 (49992) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

758. /CDROM/110_ARK/VK24.BIN +0xC410 (50192) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

759. /CDROM/110_ARK/VK24.BIN +0xC548 (50504) - Reviewed spelling and text fit
     RETAIL HEX: 1A2523241027111E24151410241F1011231B103B20201C1510231F1D150E21251523241F1E2366104324A62310171F1F1410232425142910161F22101D1566A4
     v1.2 HEX:   27111E24151410241F1011231B103B20201C1510231F1D150E2125152324191F1E2366104324A62310171F1F1410232425142910161F22101D1566A410101010
     Meaning: questons -> questions; bounded text fit: reviewed wording: just wanted -> wanted
     ORIGINAL TEXT: . / What am I doing here? / I uh just wanted to ask Apple some / questons. It's good study for me."
     v1.1 TEXT:     . / What am I doing here? / I uh wanted to ask Apple some / questions. It's good study for me."    

760. /CDROM/110_ARK/VK09.BIN +0x5E7E (24190) - Reviewed spelling and text fit
     RETAIL HEX: 241916251C6666660E66
     v1.2 HEX:   25241916251C6666660E
     Meaning: beatiful -> beautiful; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: "Karen sure is beatiful... / .....sigh...."
     v1.1 TEXT:     "Karen sure is beautiful... / ....sigh...."

761. /CDROM/110_ARK/VK19.BIN +0x7417 (29719) - Reviewed spelling and text fit
     RETAIL HEX: 66241815102422252418666666660E531F2510141F1EA624101D15111E666666660E431013111EA6241012151C19
     v1.2 HEX:   241815102422252418666666660E531F2510141F1EA624101D15111E666666660E431013111EA6241012151C1915
     Meaning: belive -> believe; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: "A cloud....the truth.... / You don't mean.... / I can't belive it..."
     v1.1 TEXT:     "A cloud...the truth.... / You don't mean.... / I can't believe it..."

762. /CDROM/110_ARK/VK30.BIN +0x7E07 (32263) - Reviewed spelling and text fit
     RETAIL HEX: 66241815102422252418666666660E531F2510141F1EA624101D15111E666666660E431013111EA6241012151C19
     v1.2 HEX:   241815102422252418666666660E531F2510141F1EA624101D15111E666666660E431013111EA6241012151C1915
     Meaning: belive -> believe; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: "A cloud....the truth.... / You don't mean.... / I can't belive it..."
     v1.1 TEXT:     "A cloud...the truth.... / You don't mean.... / I can't believe it..."

763. /CDROM/110_ARK/VK19.BIN +0x7C5E (31838) - Reviewed spelling and text fit
     RETAIL HEX: 2311
     v1.2 HEX:   1120
     Meaning: dissapoint -> disappoint; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Bah!! You dissapoint me, Retso!"
     v1.1 TEXT:     "Bah!! You disappoint me, Retso!"

764. /CDROM/110_ARK/VK30.BIN +0x864E (34382) - Reviewed spelling and text fit
     RETAIL HEX: 2311
     v1.2 HEX:   1120
     Meaning: dissapoint -> disappoint; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Bah!! You dissapoint me, Retso!"
     v1.1 TEXT:     "Bah!! You disappoint me, Retso!"

765. /CDROM/110_ARK/VK20.BIN +0x4AFC (19196) - Reviewed spelling and text fit
     RETAIL HEX: 660E4E18
     v1.2 HEX:   0E4E1819
     Meaning: Ths -> This; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: ..... / Ths will be a terrible battle..."
     v1.1 TEXT:     .... / This will be a terrible battle..."

766. /CDROM/110_ARK/VK29.BIN +0x6EF1 (28401) - Reviewed spelling and text fit
     RETAIL HEX: 2311202015112210191E10110E17221F2520101F1610161C1515191E1710231F1C141915222366A4
     v1.2 HEX:   11202015112210191E10110E17221F2520101F1610161C1515191E1710231F1C141915222366A410
     Meaning: dissappear -> disappear; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "It's easy to dissappear in a / group of fleeing soldiers."
     v1.1 TEXT:     "It's easy to disappear in a / group of fleeing soldiers." 

767. /CDROM/140_HONP/BOOK.BIN +0x75C9 (30153) - Reviewed spelling and text fit
     RETAIL HEX: 1B1E19131B191E170E1F1E10451F121F1C140E1D15112420191523650E18111D12252217152223101F220E23111E142719131815230E191E10111E101F20151E0E1619151C1466
     v1.2 HEX:   1E19131B191E170E1F1E10451F121F1C140E1D15112420191523650E18111D12252217152223101F220E23111E142719131815230E191E10111E101F20151E0E1619151C146610
     Meaning: picknicking -> picnicking; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Kobold Village /  /  You may have / fun picknicking / on Kobold / meatpies, / hamburgers or / sandwiches / in an open / field.
     v1.1 TEXT:     Kobold Village /  /  You may have / fun picnicking / on Kobold / meatpies, / hamburgers or / sandwiches / in an open / field. 

768. /CDROM/140_HONP/MEYASU.BIN +0xA135 (41269) - Reviewed spelling and text fit
     RETAIL HEX: 2210131C1F24181523660E0E10
     v1.2 HEX:   192210131C1F24181523660E0E
     Meaning: ther -> their; bounded text fit: collapse double space
     ORIGINAL TEXT: Everyone here is / so nice. / It's a pleasure to / wash ther clothes. /  /    Yoshino
     v1.1 TEXT:     Everyone here is / so nice. / It's a pleasure to / wash their clothes. /  /   Yoshino

769. /CDROM/140_HONP/MEYASU.BIN +0xA439 (42041) - Reviewed spelling and text fit
     RETAIL HEX: 1E191E17660E43A61D10161123241522102418111E0E152615226610401123241522102418111E0E2418151027191E14670E10
     v1.2 HEX:   191E191E17660E43A61D10161123241522102418111E0E152615226610401123241522102418111E0E2418151027191E14670E
     Meaning: traning -> training; bounded text fit: collapse double space
     ORIGINAL TEXT: I've been traning. / I'm faster than / ever. Faster than / the wind! /    Stallion
     v1.1 TEXT:     I've been training. / I'm faster than / ever. Faster than / the wind! /   Stallion

770. /CDROM/140_HONP/MEYASU.BIN +0xBAEF (47855) - Reviewed spelling and text fit
     RETAIL HEX: 1F2418152265102715101D2523240E23152410111E101528111D201C1510161F220E241815101318191C1422151E1011230E1B1E191718242366
     v1.2 HEX:   101F2418152265102715101D2523240E23152410111E101528111D201C1510161F220E241815101318191C1422151E1011230E1B1E1917182423
     Meaning: eachother -> each other; bounded text fit: normalize extended ellipsis
     ORIGINAL TEXT: in order to create / a bright, shining / tomorrow in which / we may all live / happily amongst / eachother, we must / set an example for / the children as / knights....
     v1.1 TEXT:     in order to create / a bright, shining / tomorrow in which / we may all live / happily amongst / each other, we must / set an example for / the children as / knights...

771. /CDROM/140_HONP/MOGURA.BIN +0x107AD (67501) - Reviewed spelling and text fit
     RETAIL HEX: 2324101C1526151C660E4324A623101215232410241F102022111324191315101F1E1024181923
     v1.2 HEX:   152324101C1526151C660E4324A623101215232410241F102022111324191315101F1E10241815
     Meaning: easist -> easiest; bounded text fit: reviewed wording: on this -> on the
     ORIGINAL TEXT: "This is the easist level. / It's best to practice on this / level until you improve."
     v1.1 TEXT:     "This is the easiest level. / It's best to practice on the / level until you improve."

772. /CDROM/140_HONP/PARTYCE1.BIN +0x41EEA (270058) - Reviewed spelling and text fit
     RETAIL HEX: 1C221917182466
     v1.2 HEX:   22191718246610
     Meaning: allright -> alright; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Yes, well...allright.
     v1.1 TEXT:     Yes, well...alright. 

773. /CDROM/140_HONP/PARTYCH2.BIN +0x4076A (264042) - Reviewed spelling and text fit
     RETAIL HEX: 1C221917182466
     v1.2 HEX:   22191718246610
     Meaning: allright -> alright; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Yes, well...allright.
     v1.1 TEXT:     Yes, well...alright. 

774. /CDROM/140_HONP/PARTYCHG.BIN +0x4076A (264042) - Reviewed spelling and text fit
     RETAIL HEX: 1C221917182466
     v1.2 HEX:   22191718246610
     Meaning: allright -> alright; bounded text fit: no wording adjustment
     ORIGINAL TEXT: Yes, well...allright.
     v1.1 TEXT:     Yes, well...alright. 

775. /CDROM/140_HONP/RBATTLE.BIN +0xEF97 (61335) - Reviewed spelling and text fit
     RETAIL HEX: 1F
     v1.2 HEX:   15
     Meaning: sorceror -> sorcerer; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "He's a powerful sorceror with a / good face, but a bad personality! / It's Leknaat's pupil, Luc!!!!"
     v1.1 TEXT:     "He's a powerful sorcerer with a / good face, but a bad personality! / It's Leknaat's pupil, Luc!!!!"

776. /CDROM/140_HONP/TANTEI.BIN +0x11837 (71735) - Reviewed spelling and text fit
     RETAIL HEX: 221F251E140E27192418103D1811131F1011
     v1.2 HEX:   121F25240E27192418103D1811131F101110
     Meaning: alot -> a lot; bounded text fit: reviewed wording: hung around -> hung about
     ORIGINAL TEXT: "I heard that he hung around / with Chaco alot when they were / both little kids."
     v1.1 TEXT:     "I heard that he hung about / with Chaco a lot when they were / both little kids."

777. /CDROM/140_HONP/TANTEI.BIN +0x184F7 (99575) - Reviewed spelling and text fit
     RETAIL HEX: 16191E14101F252410291F2522101318111E13150E1F1610111023251313152316251C1011242411131B10111711191E23240E1110251E1924101229102523191E171018152210A64D131F2524A60E1112191C19242966A4
     v1.2 HEX:   1C1511221E10291F2522101318111E13150E1F161011102325131315232316251C1011242411131B10111711191E23240E1110251E1924101229102523191E171018152210A64D131F2524A60E1112191C19242966A41010
     Meaning: succesful -> successful; bounded text fit: reviewed wording: find out -> learn
     ORIGINAL TEXT: "With Kasumi in your unit, / you can find out your chance / of a succesful attack against / a unit by using her 'Scout' / ability."
     v1.1 TEXT:     "With Kasumi in your unit, / you can learn your chance / of a successful attack against / a unit by using her 'Scout' / ability."  

778. /CDROM/140_HONP/TANTEI.BIN +0x19B5A (105306) - Reviewed spelling and text fit
     RETAIL HEX: 1913660E3C2524102418112410271123109B1029151122231011171F66A4
     v1.2 HEX:   1C1913660E4E18112410271123109B1029151122231011171F66A4101010
     Meaning: Repubic -> Republic; bounded text fit: reviewed wording: But that was -> That was
     ORIGINAL TEXT: "Could it be teleport shock? / She said that just before she / came here, she was celebrating / the birth of the Toran Repubic. / But that was 3 years ago."
     v1.1 TEXT:     "Could it be teleport shock? / She said that just before she / came here, she was celebrating / the birth of the Toran Republic. / That was 3 years ago."   

779. /CDROM/140_HONP/TANTEI.BIN +0x1A017 (106519) - Reviewed spelling and text fit
     RETAIL HEX: 23112020151122151466A4
     v1.2 HEX:   112020151122151466A410
     Meaning: dissappeared -> disappeared; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "The Sindar are a mysterious / tribe that came from the north / and left ruins in every land / they visited. They finally went / south and just dissappeared."
     v1.1 TEXT:     "The Sindar are a mysterious / tribe that came from the north / and left ruins in every land / they visited. They finally went / south and just disappeared." 

780. /CDROM/140_HONP/TANTEI.BIN +0x1A6F0 (108272) - Reviewed spelling and text fit
     RETAIL HEX: 17191E111C1C291016221F1D102418150E41221123231C111E14236510122524101815101D1F26151410241F0E471124191C1411102718151E1018151027112310291F251E1710111E140E241F1F1B10241815102415232410241F101215131F1D1510110E1B1E191718246610421510111E141047191B1C1F241F2610121513111D150E1B1E1917182423101F1E102418151023111D151014112966A4
     v1.2 HEX:   1917191E111C1C291016221F1D102418150E41221123231C111E14236510122524101815101D1F26151410241F0E471124191C1411102718151E10291F251E1710111E140E241F1F1B10241815102415232410241F101215131F1D1510110E1B1E191718246610421510111E141047191B1C1F241F2610121513111D150E1B1E1917182423101F1E102418151023111D151014112966A4101010101010
     Meaning: orginally -> originally; bounded text fit: reviewed wording: when he was young -> when young
     ORIGINAL TEXT: "He's orginally from the / Grasslands, but he moved to / Matilda when he was young and / took the test to become a / knight. He and Miklotov became / knights on the same day."
     v1.1 TEXT:     "He's originally from the / Grasslands, but he moved to / Matilda when young and / took the test to become a / knight. He and Miklotov became / knights on the same day."      

781. /CDROM/140_HONP/TEAMCHG.BIN +0x1D455 (119893) - Reviewed spelling and text fit
     RETAIL HEX: 3F261522291F1E1510232022151114101F252410111E140E232520201F222410151113181F24181522670E5115101E15151410241F10232422151E172418151E101F25220E141516151E23152367A4
     v1.2 HEX:   3B1C1C10232022151114101F252410111E140E232520201F22241015111318101F24181522670E5115101E15151410241F10232422151E172418151E101F25220E141516151E23152367A410101010
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Everyone spread -> All spread
     ORIGINAL TEXT: "Everyone spread out and / support eachother! / We need to strengthen our / defenses!"
     v1.1 TEXT:     "All spread out and / support each other! / We need to strengthen our / defenses!"    

782. /CDROM/140_HONP/TEAMCHG2.BIN +0x1D455 (119893) - Reviewed spelling and text fit
     RETAIL HEX: 3F261522291F1E1510232022151114101F252410111E140E232520201F222410151113181F24181522670E5115101E15151410241F10232422151E172418151E101F25220E141516151E23152367A4
     v1.2 HEX:   3B1C1C10232022151114101F252410111E140E232520201F22241015111318101F24181522670E5115101E15151410241F10232422151E172418151E101F25220E141516151E23152367A410101010
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Everyone spread -> All spread
     ORIGINAL TEXT: "Everyone spread out and / support eachother! / We need to strengthen our / defenses!"
     v1.1 TEXT:     "All spread out and / support each other! / We need to strengthen our / defenses!"    

783. /CDROM/290_WAR/WAR_10.BIN +0xA8DA5 (691621) - Reviewed spelling and text fit
     RETAIL HEX: 3F261522291F1E1510232022151114101F252410111E140E232520201F222410151113181F24181522670E5115101E15151410241F10232422151E172418151E101F25220E141516151E23152367A4
     v1.2 HEX:   3B1C1C10232022151114101F252410111E140E232520201F22241015111318101F24181522670E5115101E15151410241F10232422151E172418151E101F25220E141516151E23152367A410101010
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Everyone spread -> All spread
     ORIGINAL TEXT: "Everyone spread out and / support eachother! / We need to strengthen our / defenses!"
     v1.1 TEXT:     "All spread out and / support each other! / We need to strengthen our / defenses!"    

784. /CDROM/270_BOOT/END_DAT6.BIN +0x97D (2429) - Reviewed spelling and text fit
     RETAIL HEX: 221513151926151410242211191E191E1710112310110E1D191C24112229102324221124151719232466
     v1.2 HEX:   242211191E151410112310110E1D191C1924112229102324221124151719232466101010101010101010
     Meaning: miltary -> military; bounded text fit: reviewed wording: received training -> trained
     ORIGINAL TEXT:  and / received training as a / miltary strategist.
     v1.1 TEXT:      and / trained as a / military strategist.         

785. /CDROM/270_BOOT/EVENTDA5.BIN +0x404C (16460) - Reviewed spelling and text fit
     RETAIL HEX: 191EA623103E111717
     v1.2 HEX:   23191E103E11171710
     Meaning: Assasin -> Assassin; bounded text fit: fit corrected weapon label without possessive apostrophe
     ORIGINAL TEXT: Assasin's Dagg
     v1.1 TEXT:     Assassin Dagg 

786. /CDROM/280_GAME/MAGI.BIN +0x1625 (5669) - Reviewed spelling and text fit
     RETAIL HEX: 1F1E1710262366161C2915222300
     v1.2 HEX:   221F1E1710262366161C29152223
     Meaning: Stong -> Strong; bounded text fit: verified typed description capacity
     ORIGINAL TEXT: DMG to 1 row, Stong vs.flyers<00><00><00>
     v1.1 TEXT:     DMG to 1 row, Strong vs.flyers<00><00>

787. /CDROM/290_WAR/WAR_01.BIN +0x2308C (143500) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

788. /CDROM/290_WAR/WAR_02.BIN +0x230C8 (143560) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

789. /CDROM/290_WAR/WAR_03.BIN +0x231D4 (143828) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

790. /CDROM/290_WAR/WAR_04.BIN +0x23164 (143716) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

791. /CDROM/290_WAR/WAR_05.BIN +0x232AC (144044) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

792. /CDROM/290_WAR/WAR_06.BIN +0x2349C (144540) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

793. /CDROM/290_WAR/WAR_07.BIN +0x234BC (144572) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

794. /CDROM/290_WAR/WAR_08.BIN +0x23638 (144952) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

795. /CDROM/290_WAR/WAR_09.BIN +0x23474 (144500) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

796. /CDROM/290_WAR/WAR_10.BIN +0x23424 (144420) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

797. /CDROM/290_WAR/WAR_11.BIN +0x234B4 (144564) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

798. /CDROM/290_WAR/WAR_12.BIN +0x23580 (144768) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

799. /CDROM/290_WAR/WAR_13.BIN +0x23520 (144672) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

800. /CDROM/290_WAR/WAR_14.BIN +0x233F4 (144372) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

801. /CDROM/290_WAR/WAR_15.BIN +0x23440 (144448) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

802. /CDROM/290_WAR/WAR_16.BIN +0x2355C (144732) - Reviewed spelling and text fit
     RETAIL HEX: 47111B151011141A1113151E240E151E151D2910251E1924231016191718240E15111318
     v1.2 HEX:   4615241011141A1113151E240E151E151D2910251E1924231016191718240E1511131810
     Meaning: eachother -> each other; bounded text fit: reviewed wording: Make adjacent -> Let adjacent
     ORIGINAL TEXT: Make adjacent / enemy units fight / eachother
     v1.1 TEXT:     Let adjacent / enemy units fight / each other

803. /CDROM/140_HONP/MEYASU.BIN +0xC9EB (51691) - Reviewed spelling and text fit
     RETAIL HEX: 651024181124A623101A25232410110E1619222324101422111624651012252410291F250E1715241024181510191415116666660E10
     v1.2 HEX:   1C651024181124A623101A25232410110E1619222324101422111624651012252410291F250E1715241024181510191415116666660E
     Meaning: Wel -> Well; bounded text fit: collapse one redundant space in the same letter
     ORIGINAL TEXT: How's this<A2> / "Dearest Flik. / I love thee as a bee / loves a flower...." / Wel, that's just a / first draft, but you / get the idea... /    From Nina
     v1.1 TEXT:     How's this<A2> / "Dearest Flik. / I love thee as a bee / loves a flower...." / Well, that's just a / first draft, but you / get the idea... /   From Nina

804. /CDROM/020_ARB/VB02.BIN +0x8B18 (35608) - Reviewed spelling and text fit
     RETAIL HEX: 24A6
     v1.2 HEX:   A624
     Meaning: Dont' -> Don't; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Dont' forget!"
     v1.1 TEXT:     "Don't forget!"

805. /CDROM/020_ARB/VB03.BIN +0x4DD4 (19924) - Reviewed spelling and text fit
     RETAIL HEX: 24A6
     v1.2 HEX:   A624
     Meaning: Dont' -> Don't; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Dont' forget!"
     v1.1 TEXT:     "Don't forget!"

806. /CDROM/020_ARB/VB04.BIN +0x8254 (33364) - Reviewed spelling and text fit
     RETAIL HEX: 24A6
     v1.2 HEX:   A624
     Meaning: Dont' -> Don't; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Dont' forget!"
     v1.1 TEXT:     "Don't forget!"

807. /CDROM/020_ARB/VB05.BIN +0x6BD4 (27604) - Reviewed spelling and text fit
     RETAIL HEX: 1EA62410171F10241F1024181510481F22241810
     v1.2 HEX:   241EA62410171F10241F1024181510481F222418
     Meaning: musn't -> mustn't; bounded text fit: remove redundant space immediately before line break
     ORIGINAL TEXT: "You musn't go to the North  / Sparrow Pass. A horrible  / Mist Monster lives there.
     v1.1 TEXT:     "You mustn't go to the North / Sparrow Pass. A horrible  / Mist Monster lives there.

808. /CDROM/020_ARB/VB14.BIN +0x6228 (25128) - Reviewed spelling and text fit
     RETAIL HEX: 24A6
     v1.2 HEX:   A624
     Meaning: Dont' -> Don't; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Dont' forget!"
     v1.1 TEXT:     "Don't forget!"

809. /CDROM/020_ARB/VB18.BIN +0x7304 (29444) - Reviewed spelling and text fit
     RETAIL HEX: 1EA62410171F10241F1024181510481F22241810
     v1.2 HEX:   241EA62410171F10241F1024181510481F222418
     Meaning: musn't -> mustn't; bounded text fit: remove redundant space immediately before line break
     ORIGINAL TEXT: "You musn't go to the North  / Sparrow Pass. A horrible  / Mist Monster lives there.
     v1.1 TEXT:     "You mustn't go to the North / Sparrow Pass. A horrible  / Mist Monster lives there.

810. /CDROM/020_ARB/VB19.BIN +0x47D0 (18384) - Reviewed spelling and text fit
     RETAIL HEX: 24A6
     v1.2 HEX:   A624
     Meaning: Dont' -> Don't; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Dont' forget!"
     v1.1 TEXT:     "Don't forget!"

811. /CDROM/080_ARH/VH01.BIN +0x762F (30255) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

812. /CDROM/080_ARH/VH03.BIN +0x727F (29311) - Reviewed spelling and text fit
     RETAIL HEX: 1EA62410181511221410111E291F1E151024111C1B1011121F25240E241815104E152324101F1610241815104F1E19131F221E1023191E131510430E2711231011101318191C
     v1.2 HEX:   151EA62410181511221410111E291F1E151024111C1B1011121F25240E241815104E152324101F1610241815104F1E19131F221E1023191E1315101D290E1318191C14181F1F
     Meaning: havn't -> haven't; bounded text fit: equivalent wording: since I was a child -> since my childhood
     ORIGINAL TEXT: I havn't heard anyone talk about / the Test of the Unicorn since I / was a child. / It's just an old, old fairy tale."
     v1.1 TEXT:     I haven't heard anyone talk about / the Test of the Unicorn since my / childhood. / It's just an old, old fairy tale."

813. /CDROM/080_ARH/VH05.BIN +0x964B (38475) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

814. /CDROM/080_ARH/VH06.BIN +0x4E3B (20027) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

815. /CDROM/080_ARH/VH07.BIN +0x187F (6271) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

816. /CDROM/080_ARH/VH09.BIN +0x1713 (5907) - Reviewed spelling and text fit
     RETAIL HEX: 1EA62410181511221410111E291F1E151024111C1B1011121F25240E241815104E152324101F1610241815104F1E19131F221E1023191E131510430E2711231011101318191C
     v1.2 HEX:   151EA62410181511221410111E291F1E151024111C1B1011121F25240E241815104E152324101F1610241815104F1E19131F221E1023191E1315101D290E1318191C14181F1F
     Meaning: havn't -> haven't; bounded text fit: equivalent wording: since I was a child -> since my childhood
     ORIGINAL TEXT: I havn't heard anyone talk about / the Test of the Unicorn since I / was a child. / It's just an old, old fairy tale."
     v1.1 TEXT:     I haven't heard anyone talk about / the Test of the Unicorn since my / childhood. / It's just an old, old fairy tale."

817. /CDROM/080_ARH/VH10.BIN +0xC2AB (49835) - Reviewed spelling and text fit
     RETAIL HEX: 1EA62410181511221410111E291F1E151024111C1B1011121F25240E241815104E152324101F1610241815104F1E19131F221E1023191E131510430E2711231011101318191C
     v1.2 HEX:   151EA62410181511221410111E291F1E151024111C1B1011121F25240E241815104E152324101F1610241815104F1E19131F221E1023191E1315101D290E1318191C14181F1F
     Meaning: havn't -> haven't; bounded text fit: equivalent wording: since I was a child -> since my childhood
     ORIGINAL TEXT: I havn't heard anyone talk about / the Test of the Unicorn since I / was a child. / It's just an old, old fairy tale."
     v1.1 TEXT:     I haven't heard anyone talk about / the Test of the Unicorn since my / childhood. / It's just an old, old fairy tale."

818. /CDROM/080_ARH/VH11.BIN +0x70E7 (28903) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

819. /CDROM/080_ARH/VH13.BIN +0x5057 (20567) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

820. /CDROM/080_ARH/VH14.BIN +0x74BF (29887) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

821. /CDROM/080_ARH/VH16.BIN +0x3E83 (16003) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

822. /CDROM/080_ARH/VH17.BIN +0x709F (28831) - Reviewed spelling and text fit
     RETAIL HEX: 17221511240E1318111E13151024181124102715101D2523
     v1.2 HEX:   16191E150E1318111E13151024181124102715101D252324
     Meaning: musn't -> mustn't; bounded text fit: reviewed wording: a great -> a fine
     ORIGINAL TEXT: "Be serious! This is a great / chance that we musn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.
     v1.1 TEXT:     "Be serious! This is a fine / chance that we mustn't pass up. / The Kobolds don't trust us and / the Wingers are no use either.

823. /CDROM/110_ARK/VK24.BIN +0xB8E4 (47332) - Reviewed spelling and text fit
     RETAIL HEX: A6231014111E1715221F252366A4
     v1.2 HEX:   231014111E1715221F252366A410
     Meaning: get's -> gets; bounded text fit: no wording adjustment
     ORIGINAL TEXT: "Well if that's what your / strategist says, maybe you should / do it. You can always run away / if it get's dangerous."
     v1.1 TEXT:     "Well if that's what your / strategist says, maybe you should / do it. You can always run away / if it gets dangerous." 

824. /CDROM/290_WAR/WAR_12.BIN +0xA83CB (689099) - Reviewed spelling and text fit
     RETAIL HEX: 1EA624101C1F231567
     v1.2 HEX:   241EA624101C1F2315
     Meaning: musn't -> mustn't; bounded text fit: triple exclamation -> double for fixed text budget
     ORIGINAL TEXT: "Attack!! / In the name of the Karaya, / we musn't lose!!!"
     v1.1 TEXT:     "Attack!! / In the name of the Karaya, / we mustn't lose!!"

825. /CDROM/010_ARA/VA03.BIN +0x695F (26975) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

826. /CDROM/010_ARA/VA03.BIN +0x7DFB (32251) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

827. /CDROM/010_ARA/VA03.BIN +0x8F11 (36625) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

828. /CDROM/010_ARA/VA03.BIN +0x8F3B (36667) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

829. /CDROM/010_ARA/VA05.BIN +0xB6F3 (46835) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

830. /CDROM/010_ARA/VA06.BIN +0x8E87 (36487) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

831. /CDROM/010_ARA/VA07.BIN +0x3A3B (14907) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

832. /CDROM/010_ARA/VA08.BIN +0x85D7 (34263) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

833. /CDROM/010_ARA/VA12.BIN +0x57A7 (22439) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

834. /CDROM/010_ARA/VA16.BIN +0x39BB (14779) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

835. /CDROM/020_ARB/VB03.BIN +0x366C (13932) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

836. /CDROM/020_ARB/VB03.BIN +0x3694 (13972) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

837. /CDROM/020_ARB/VB03.BIN +0x3887 (14471) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

838. /CDROM/020_ARB/VB03.BIN +0x42BD (17085) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

839. /CDROM/020_ARB/VB03.BIN +0x4410 (17424) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

840. /CDROM/020_ARB/VB04.BIN +0x6CF8 (27896) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

841. /CDROM/020_ARB/VB04.BIN +0x6D20 (27936) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

842. /CDROM/020_ARB/VB04.BIN +0x773D (30525) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

843. /CDROM/020_ARB/VB04.BIN +0x7890 (30864) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

844. /CDROM/020_ARB/VB05.BIN +0x4CC8 (19656) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

845. /CDROM/020_ARB/VB05.BIN +0x4CF0 (19696) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

846. /CDROM/020_ARB/VB05.BIN +0xA40F (41999) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

847. /CDROM/020_ARB/VB05.BIN +0xA4BE (42174) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

848. /CDROM/020_ARB/VB05.BIN +0xA55D (42333) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

849. /CDROM/020_ARB/VB05.BIN +0xA5C8 (42440) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

850. /CDROM/020_ARB/VB06.BIN +0x10AD (4269) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

851. /CDROM/020_ARB/VB06.BIN +0x209B (8347) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

852. /CDROM/020_ARB/VB06.BIN +0x214A (8522) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

853. /CDROM/020_ARB/VB06.BIN +0x21E9 (8681) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

854. /CDROM/020_ARB/VB06.BIN +0x2254 (8788) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

855. /CDROM/020_ARB/VB06.BIN +0x2ABC (10940) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

856. /CDROM/020_ARB/VB06.BIN +0x2AD8 (10968) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

857. /CDROM/020_ARB/VB07.BIN +0xB34B (45899) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

858. /CDROM/020_ARB/VB07.BIN +0xB3FA (46074) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

859. /CDROM/020_ARB/VB07.BIN +0xB499 (46233) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

860. /CDROM/020_ARB/VB07.BIN +0xB504 (46340) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

861. /CDROM/020_ARB/VB08.BIN +0x84FC (34044) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

862. /CDROM/020_ARB/VB08.BIN +0x8564 (34148) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

863. /CDROM/020_ARB/VB08.BIN +0x859E (34206) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

864. /CDROM/020_ARB/VB09.BIN +0x5D81 (23937) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

865. /CDROM/020_ARB/VB14.BIN +0x464D (17997) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

866. /CDROM/020_ARB/VB16.BIN +0x2371 (9073) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

867. /CDROM/020_ARB/VB17.BIN +0x83C8 (33736) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

868. /CDROM/020_ARB/VB17.BIN +0x8430 (33840) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

869. /CDROM/020_ARB/VB17.BIN +0x846A (33898) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

870. /CDROM/020_ARB/VB18.BIN +0x53F8 (21496) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

871. /CDROM/020_ARB/VB18.BIN +0x5420 (21536) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

872. /CDROM/020_ARB/VB19.BIN +0x2BF5 (11253) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

873. /CDROM/030_ARC/VC01.BIN +0xDEDC (57052) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

874. /CDROM/030_ARC/VC01.BIN +0xDF0F (57103) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

875. /CDROM/030_ARC/VC04.BIN +0x87F8 (34808) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

876. /CDROM/030_ARC/VC04.BIN +0x8820 (34848) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

877. /CDROM/030_ARC/VC04.BIN +0xBB96 (48022) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

878. /CDROM/030_ARC/VC06.BIN +0x6263 (25187) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

879. /CDROM/030_ARC/VC06.BIN +0x6312 (25362) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

880. /CDROM/030_ARC/VC06.BIN +0x63B1 (25521) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

881. /CDROM/030_ARC/VC06.BIN +0x641C (25628) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

882. /CDROM/030_ARC/VC06.BIN +0x6996 (27030) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

883. /CDROM/030_ARC/VC06.BIN +0xBA58 (47704) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

884. /CDROM/030_ARC/VC06.BIN +0xBA75 (47733) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

885. /CDROM/030_ARC/VC12.BIN +0x12F30 (77616) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

886. /CDROM/030_ARC/VC12.BIN +0x12F98 (77720) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

887. /CDROM/030_ARC/VC12.BIN +0x12FD2 (77778) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

888. /CDROM/030_ARC/VC13.BIN +0x142B8 (82616) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

889. /CDROM/030_ARC/VC13.BIN +0x14320 (82720) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

890. /CDROM/030_ARC/VC13.BIN +0x1435A (82778) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

891. /CDROM/030_ARC/VC18.BIN +0x26B5 (9909) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

892. /CDROM/030_ARC/VC19.BIN +0x1199 (4505) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

893. /CDROM/030_ARC/VC21.BIN +0xE574 (58740) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

894. /CDROM/030_ARC/VC21.BIN +0xE581 (58753) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

895. /CDROM/030_ARC/VC21.BIN +0xE5B5 (58805) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

896. /CDROM/030_ARC/VC21.BIN +0xE69B (59035) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

897. /CDROM/030_ARC/VC21.BIN +0xE7BD (59325) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

898. /CDROM/030_ARC/VC21.BIN +0xE917 (59671) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

899. /CDROM/030_ARC/VC21.BIN +0xE99B (59803) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

900. /CDROM/030_ARC/VC21.BIN +0x13BEC (80876) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

901. /CDROM/030_ARC/VC21.BIN +0x13C1F (80927) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

902. /CDROM/030_ARC/VC21.BIN +0x147F6 (83958) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

903. /CDROM/030_ARC/VC21.BIN +0x16B3D (92989) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

904. /CDROM/030_ARC/VC21.BIN +0x16B65 (93029) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

905. /CDROM/030_ARC/VC23.BIN +0x11F1 (4593) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

906. /CDROM/030_ARC/VC24.BIN +0xA308 (41736) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

907. /CDROM/030_ARC/VC24.BIN +0xA33B (41787) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

908. /CDROM/030_ARC/VC26.BIN +0x2624 (9764) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

909. /CDROM/030_ARC/VC26.BIN +0x2657 (9815) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

910. /CDROM/040_ARD/VD01.BIN +0x53B0 (21424) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

911. /CDROM/040_ARD/VD01.BIN +0x53D8 (21464) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

912. /CDROM/040_ARD/VD01.BIN +0x66B5 (26293) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

913. /CDROM/040_ARD/VD02.BIN +0xCC98 (52376) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

914. /CDROM/040_ARD/VD02.BIN +0xCCCB (52427) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

915. /CDROM/040_ARD/VD03.BIN +0xF41C (62492) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

916. /CDROM/040_ARD/VD03.BIN +0xF484 (62596) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

917. /CDROM/040_ARD/VD03.BIN +0xF4BE (62654) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

918. /CDROM/040_ARD/VD05.BIN +0x8121 (33057) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

919. /CDROM/040_ARD/VD05.BIN +0x82AA (33450) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

920. /CDROM/040_ARD/VD05.BIN +0x8972 (35186) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

921. /CDROM/040_ARD/VD05.BIN +0xDD00 (56576) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

922. /CDROM/040_ARD/VD05.BIN +0xDD5F (56671) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

923. /CDROM/040_ARD/VD05.BIN +0xDDBA (56762) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

924. /CDROM/040_ARD/VD06.BIN +0xB30D (45837) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

925. /CDROM/040_ARD/VD06.BIN +0xBA20 (47648) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

926. /CDROM/040_ARD/VD06.BIN +0xBA88 (47752) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

927. /CDROM/040_ARD/VD06.BIN +0xBAC2 (47810) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

928. /CDROM/040_ARD/VD11.BIN +0x9239 (37433) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

929. /CDROM/040_ARD/VD11.BIN +0x93C2 (37826) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

930. /CDROM/040_ARD/VD12.BIN +0x7625 (30245) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

931. /CDROM/040_ARD/VD12.BIN +0x77AE (30638) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

932. /CDROM/040_ARD/VD13.BIN +0xA1E1 (41441) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

933. /CDROM/040_ARD/VD13.BIN +0xA36A (41834) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

934. /CDROM/040_ARD/VD16.BIN +0x669D (26269) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

935. /CDROM/040_ARD/VD17.BIN +0x67AC (26540) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

936. /CDROM/040_ARD/VD17.BIN +0x67CA (26570) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

937. /CDROM/040_ARD/VD17.BIN +0xC3F7 (50167) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

938. /CDROM/040_ARD/VD17.BIN +0xC409 (50185) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

939. /CDROM/040_ARD/VD17.BIN +0x1069B (67227) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

940. /CDROM/040_ARD/VD19.BIN +0x5F78 (24440) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

941. /CDROM/040_ARD/VD19.BIN +0x5FA0 (24480) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

942. /CDROM/040_ARD/VD19.BIN +0x7269 (29289) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

943. /CDROM/040_ARD/VD19.BIN +0x73F2 (29682) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

944. /CDROM/040_ARD/VD19.BIN +0x7ABA (31418) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

945. /CDROM/050_ARE/VE02.BIN +0x7684 (30340) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

946. /CDROM/050_ARE/VE02.BIN +0x76AE (30382) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

947. /CDROM/050_ARE/VE02.BIN +0xE5C4 (58820) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

948. /CDROM/050_ARE/VE02.BIN +0xE62C (58924) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

949. /CDROM/050_ARE/VE02.BIN +0xE666 (58982) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

950. /CDROM/050_ARE/VE07.BIN +0x8D16 (36118) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

951. /CDROM/050_ARE/VE10.BIN +0x6A10 (27152) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

952. /CDROM/050_ARE/VE10.BIN +0x6A38 (27192) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

953. /CDROM/060_ARF/VF03.BIN +0x9470 (38000) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

954. /CDROM/060_ARF/VF03.BIN +0x9498 (38040) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

955. /CDROM/060_ARF/VF03.BIN +0x9590 (38288) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

956. /CDROM/060_ARF/VF03.BIN +0x95B8 (38328) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

957. /CDROM/060_ARF/VF04.BIN +0xDA1C (55836) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

958. /CDROM/060_ARF/VF05.BIN +0x8D25 (36133) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

959. /CDROM/060_ARF/VF05.BIN +0xBC90 (48272) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

960. /CDROM/060_ARF/VF05.BIN +0xBCC3 (48323) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

961. /CDROM/060_ARF/VF05.BIN +0xCB4C (52044) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

962. /CDROM/060_ARF/VF05.BIN +0xCB74 (52084) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

963. /CDROM/060_ARF/VF05.BIN +0xCC60 (52320) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

964. /CDROM/060_ARF/VF05.BIN +0xCC88 (52360) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

965. /CDROM/060_ARF/VF06.BIN +0x9520 (38176) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

966. /CDROM/060_ARF/VF06.BIN +0x9588 (38280) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

967. /CDROM/060_ARF/VF06.BIN +0x95C2 (38338) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

968. /CDROM/060_ARF/VF07.BIN +0xADC4 (44484) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

969. /CDROM/060_ARF/VF07.BIN +0xAE2C (44588) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

970. /CDROM/060_ARF/VF07.BIN +0xAE66 (44646) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

971. /CDROM/070_ARG/VG03.BIN +0x7A9E (31390) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

972. /CDROM/070_ARG/VG03.BIN +0x7AB9 (31417) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

973. /CDROM/070_ARG/VG03.BIN +0x7C04 (31748) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

974. /CDROM/070_ARG/VG03.BIN +0x7C1B (31771) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

975. /CDROM/070_ARG/VG03.BIN +0x7CF4 (31988) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

976. /CDROM/070_ARG/VG06.BIN +0x39DC (14812) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

977. /CDROM/070_ARG/VG06.BIN +0x3A04 (14852) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

978. /CDROM/070_ARG/VG06.BIN +0x6817 (26647) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

979. /CDROM/070_ARG/VG06.BIN +0x692E (26926) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

980. /CDROM/070_ARG/VG07.BIN +0x58C0 (22720) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

981. /CDROM/070_ARG/VG07.BIN +0x58E8 (22760) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

982. /CDROM/070_ARG/VG08.BIN +0x5455 (21589) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

983. /CDROM/070_ARG/VG08.BIN +0x547D (21629) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

984. /CDROM/070_ARG/VG13.BIN +0x653D (25917) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

985. /CDROM/070_ARG/VG13.BIN +0x6565 (25957) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

986. /CDROM/070_ARG/VG13.BIN +0xAB4A (43850) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

987. /CDROM/070_ARG/VG13.BIN +0xAB65 (43877) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

988. /CDROM/070_ARG/VG13.BIN +0xACB0 (44208) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

989. /CDROM/070_ARG/VG13.BIN +0xACC7 (44231) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

990. /CDROM/070_ARG/VG13.BIN +0xADA0 (44448) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

991. /CDROM/070_ARG/VG13.BIN +0xD93C (55612) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

992. /CDROM/070_ARG/VG13.BIN +0xD9A4 (55716) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

993. /CDROM/070_ARG/VG13.BIN +0xD9DE (55774) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

994. /CDROM/070_ARG/VG15.BIN +0xB730 (46896) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

995. /CDROM/070_ARG/VG15.BIN +0xB798 (47000) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

996. /CDROM/070_ARG/VG15.BIN +0xB7D2 (47058) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

997. /CDROM/080_ARH/VH01.BIN +0xB648 (46664) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

998. /CDROM/080_ARH/VH01.BIN +0xB659 (46681) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

999. /CDROM/080_ARH/VH01.BIN +0xB720 (46880) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1000. /CDROM/080_ARH/VH01.BIN +0xB7FD (47101) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1001. /CDROM/080_ARH/VH01.BIN +0xB877 (47223) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1002. /CDROM/080_ARH/VH01.BIN +0xB8BF (47295) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1003. /CDROM/080_ARH/VH01.BIN +0xB941 (47425) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1004. /CDROM/080_ARH/VH01.BIN +0xBA5E (47710) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1005. /CDROM/080_ARH/VH01.BIN +0xBAD8 (47832) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1006. /CDROM/080_ARH/VH01.BIN +0xBB20 (47904) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1007. /CDROM/080_ARH/VH02.BIN +0x596D (22893) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1008. /CDROM/080_ARH/VH02.BIN +0x5995 (22933) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1009. /CDROM/080_ARH/VH02.BIN +0x7B6B (31595) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1010. /CDROM/080_ARH/VH02.BIN +0x7BF9 (31737) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1011. /CDROM/080_ARH/VH02.BIN +0x89C0 (35264) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1012. /CDROM/080_ARH/VH02.BIN +0x8A28 (35368) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1013. /CDROM/080_ARH/VH02.BIN +0x8A62 (35426) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1014. /CDROM/080_ARH/VH03.BIN +0xCAA0 (51872) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1015. /CDROM/080_ARH/VH03.BIN +0xCAC8 (51912) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1016. /CDROM/080_ARH/VH03.BIN +0xCBA4 (52132) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1017. /CDROM/080_ARH/VH03.BIN +0xCBCC (52172) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1018. /CDROM/080_ARH/VH04.BIN +0xD388 (54152) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1019. /CDROM/080_ARH/VH04.BIN +0xD399 (54169) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1020. /CDROM/080_ARH/VH04.BIN +0xD460 (54368) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1021. /CDROM/080_ARH/VH04.BIN +0xD53D (54589) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1022. /CDROM/080_ARH/VH04.BIN +0xD5B7 (54711) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1023. /CDROM/080_ARH/VH04.BIN +0xD5FF (54783) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1024. /CDROM/080_ARH/VH04.BIN +0xD681 (54913) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1025. /CDROM/080_ARH/VH04.BIN +0xD79E (55198) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1026. /CDROM/080_ARH/VH04.BIN +0xD818 (55320) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1027. /CDROM/080_ARH/VH04.BIN +0xD860 (55392) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1028. /CDROM/080_ARH/VH04.BIN +0xE214 (57876) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1029. /CDROM/080_ARH/VH04.BIN +0xE27C (57980) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1030. /CDROM/080_ARH/VH04.BIN +0xE2B6 (58038) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1031. /CDROM/080_ARH/VH06.BIN +0x8DDC (36316) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1032. /CDROM/080_ARH/VH06.BIN +0x8DED (36333) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1033. /CDROM/080_ARH/VH06.BIN +0x8EB4 (36532) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1034. /CDROM/080_ARH/VH06.BIN +0x8F91 (36753) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1035. /CDROM/080_ARH/VH06.BIN +0x900B (36875) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1036. /CDROM/080_ARH/VH06.BIN +0x9053 (36947) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1037. /CDROM/080_ARH/VH06.BIN +0x90D5 (37077) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1038. /CDROM/080_ARH/VH06.BIN +0x91F2 (37362) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1039. /CDROM/080_ARH/VH06.BIN +0x926C (37484) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1040. /CDROM/080_ARH/VH06.BIN +0x92B4 (37556) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1041. /CDROM/080_ARH/VH11.BIN +0x349C (13468) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1042. /CDROM/080_ARH/VH11.BIN +0x34BD (13501) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1043. /CDROM/080_ARH/VH11.BIN +0x353A (13626) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1044. /CDROM/080_ARH/VH11.BIN +0xB268 (45672) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1045. /CDROM/080_ARH/VH11.BIN +0xB279 (45689) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1046. /CDROM/080_ARH/VH11.BIN +0xB340 (45888) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1047. /CDROM/080_ARH/VH11.BIN +0xB41D (46109) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1048. /CDROM/080_ARH/VH11.BIN +0xB497 (46231) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1049. /CDROM/080_ARH/VH11.BIN +0xB4DF (46303) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1050. /CDROM/080_ARH/VH11.BIN +0xB561 (46433) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1051. /CDROM/080_ARH/VH11.BIN +0xB67E (46718) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1052. /CDROM/080_ARH/VH11.BIN +0xB6F8 (46840) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1053. /CDROM/080_ARH/VH11.BIN +0xB740 (46912) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1054. /CDROM/080_ARH/VH12.BIN +0x615C (24924) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1055. /CDROM/080_ARH/VH12.BIN +0x616D (24941) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1056. /CDROM/080_ARH/VH12.BIN +0x6234 (25140) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1057. /CDROM/080_ARH/VH12.BIN +0x6311 (25361) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1058. /CDROM/080_ARH/VH12.BIN +0x638B (25483) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1059. /CDROM/080_ARH/VH12.BIN +0x63D3 (25555) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1060. /CDROM/080_ARH/VH12.BIN +0x6455 (25685) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1061. /CDROM/080_ARH/VH12.BIN +0x6572 (25970) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1062. /CDROM/080_ARH/VH12.BIN +0x65EC (26092) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1063. /CDROM/080_ARH/VH12.BIN +0x6634 (26164) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1064. /CDROM/080_ARH/VH13.BIN +0x907C (36988) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1065. /CDROM/080_ARH/VH13.BIN +0x908D (37005) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1066. /CDROM/080_ARH/VH13.BIN +0x9154 (37204) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1067. /CDROM/080_ARH/VH13.BIN +0x9231 (37425) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1068. /CDROM/080_ARH/VH13.BIN +0x92AB (37547) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1069. /CDROM/080_ARH/VH13.BIN +0x92F3 (37619) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1070. /CDROM/080_ARH/VH13.BIN +0x9375 (37749) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1071. /CDROM/080_ARH/VH13.BIN +0x9492 (38034) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1072. /CDROM/080_ARH/VH13.BIN +0x950C (38156) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1073. /CDROM/080_ARH/VH13.BIN +0x9554 (38228) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1074. /CDROM/080_ARH/VH15.BIN +0xD1C4 (53700) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1075. /CDROM/080_ARH/VH15.BIN +0xD1D5 (53717) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1076. /CDROM/080_ARH/VH15.BIN +0xD29C (53916) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1077. /CDROM/080_ARH/VH15.BIN +0xD379 (54137) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1078. /CDROM/080_ARH/VH15.BIN +0xD3F3 (54259) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1079. /CDROM/080_ARH/VH15.BIN +0xD43B (54331) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1080. /CDROM/080_ARH/VH15.BIN +0xD4BD (54461) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1081. /CDROM/080_ARH/VH15.BIN +0xD5DA (54746) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1082. /CDROM/080_ARH/VH15.BIN +0xD654 (54868) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1083. /CDROM/080_ARH/VH15.BIN +0xD69C (54940) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1084. /CDROM/080_ARH/VH15.BIN +0xE050 (57424) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1085. /CDROM/080_ARH/VH15.BIN +0xE0B8 (57528) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1086. /CDROM/080_ARH/VH15.BIN +0xE0F2 (57586) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1087. /CDROM/080_ARH/VH16.BIN +0x7E30 (32304) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1088. /CDROM/080_ARH/VH16.BIN +0x7E41 (32321) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1089. /CDROM/080_ARH/VH16.BIN +0x7F08 (32520) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1090. /CDROM/080_ARH/VH16.BIN +0x7FE5 (32741) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1091. /CDROM/080_ARH/VH16.BIN +0x805F (32863) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1092. /CDROM/080_ARH/VH16.BIN +0x80A7 (32935) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1093. /CDROM/080_ARH/VH16.BIN +0x8129 (33065) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1094. /CDROM/080_ARH/VH16.BIN +0x8246 (33350) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1095. /CDROM/080_ARH/VH16.BIN +0x82C0 (33472) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1096. /CDROM/080_ARH/VH16.BIN +0x8308 (33544) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1097. /CDROM/080_ARH/VH17.BIN +0xB22C (45612) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1098. /CDROM/080_ARH/VH17.BIN +0xB23D (45629) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1099. /CDROM/080_ARH/VH17.BIN +0xB304 (45828) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1100. /CDROM/080_ARH/VH17.BIN +0xB3E1 (46049) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1101. /CDROM/080_ARH/VH17.BIN +0xB45B (46171) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1102. /CDROM/080_ARH/VH17.BIN +0xB4A3 (46243) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1103. /CDROM/080_ARH/VH17.BIN +0xB525 (46373) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1104. /CDROM/080_ARH/VH17.BIN +0xB642 (46658) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1105. /CDROM/080_ARH/VH17.BIN +0xB6BC (46780) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1106. /CDROM/080_ARH/VH17.BIN +0xB704 (46852) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1107. /CDROM/090_ARI/VI01.BIN +0xE2A1 (58017) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1108. /CDROM/090_ARI/VI01.BIN +0xE2CB (58059) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1109. /CDROM/090_ARI/VI02.BIN +0x3B94 (15252) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1110. /CDROM/090_ARI/VI08.BIN +0xA85C (43100) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1111. /CDROM/090_ARI/VI08.BIN +0xA8C4 (43204) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1112. /CDROM/090_ARI/VI08.BIN +0xA8FE (43262) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1113. /CDROM/090_ARI/VI12.BIN +0x89CC (35276) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1114. /CDROM/090_ARI/VI12.BIN +0x8A34 (35380) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1115. /CDROM/090_ARI/VI12.BIN +0x8A6E (35438) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1116. /CDROM/090_ARI/VI12.BIN +0x8B2D (35629) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1117. /CDROM/090_ARI/VI12.BIN +0x8B57 (35671) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1118. /CDROM/090_ARI/VI12.BIN +0x8E2E (36398) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1119. /CDROM/090_ARI/VI15.BIN +0x23E0 (9184) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1120. /CDROM/090_ARI/VI15.BIN +0x2448 (9288) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1121. /CDROM/090_ARI/VI15.BIN +0x2482 (9346) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1122. /CDROM/100_ARJ/VJ05.BIN +0xB588 (46472) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1123. /CDROM/100_ARJ/VJ05.BIN +0xB5F0 (46576) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1124. /CDROM/100_ARJ/VJ05.BIN +0xB62A (46634) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1125. /CDROM/100_ARJ/VJ07.BIN +0x2274 (8820) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1126. /CDROM/100_ARJ/VJ07.BIN +0x22DC (8924) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1127. /CDROM/100_ARJ/VJ07.BIN +0x2316 (8982) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1128. /CDROM/100_ARJ/VJ17.BIN +0x2860 (10336) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1129. /CDROM/100_ARJ/VJ17.BIN +0x2888 (10376) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1130. /CDROM/110_ARK/VK02.BIN +0x5484 (21636) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1131. /CDROM/110_ARK/VK02.BIN +0x54EC (21740) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1132. /CDROM/110_ARK/VK02.BIN +0x5526 (21798) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1133. /CDROM/110_ARK/VK07.BIN +0x114F4 (70900) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1134. /CDROM/110_ARK/VK07.BIN +0x1155C (71004) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1135. /CDROM/110_ARK/VK07.BIN +0x11596 (71062) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1136. /CDROM/110_ARK/VK22.BIN +0x5A00 (23040) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1137. /CDROM/110_ARK/VK22.BIN +0x5A68 (23144) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1138. /CDROM/110_ARK/VK22.BIN +0x5AA2 (23202) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1139. /CDROM/110_ARK/VK31.BIN +0x6834 (26676) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1140. /CDROM/130_SHOP/DOUGUYA1.BIN +0xAC33 (44083) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1141. /CDROM/130_SHOP/DOUGUYA1.BIN +0xACC0 (44224) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1142. /CDROM/130_SHOP/DOUGUYA2.BIN +0xAC33 (44083) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1143. /CDROM/130_SHOP/DOUGUYA2.BIN +0xACC0 (44224) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1144. /CDROM/130_SHOP/KAJIYA1.BIN +0x7474 (29812) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1145. /CDROM/130_SHOP/KAJIYA1.BIN +0x7524 (29988) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1146. /CDROM/130_SHOP/KAJIYA2.BIN +0x7474 (29812) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1147. /CDROM/130_SHOP/KAJIYA2.BIN +0x7524 (29988) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1148. /CDROM/130_SHOP/KANTEIY1.BIN +0x4A80 (19072) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1149. /CDROM/130_SHOP/KANTEIY2.BIN +0x4A80 (19072) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1150. /CDROM/130_SHOP/KOUEKI1.BIN +0x74E4 (29924) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1151. /CDROM/130_SHOP/KOUEKI2.BIN +0x74E4 (29924) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1152. /CDROM/130_SHOP/MONSYOY1.BIN +0x8B6C (35692) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1153. /CDROM/130_SHOP/MONSYOY1.BIN +0x8BFC (35836) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1154. /CDROM/130_SHOP/MONSYOY2.BIN +0x8B6C (35692) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1155. /CDROM/130_SHOP/MONSYOY2.BIN +0x8BFC (35836) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1156. /CDROM/130_SHOP/YADOYA1.BIN +0x85D0 (34256) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1157. /CDROM/130_SHOP/YADOYA2.BIN +0x85D0 (34256) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1158. /CDROM/140_HONP/BOOK.BIN +0x4EF0 (20208) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1159. /CDROM/140_HONP/BOOK.BIN +0x4F0B (20235) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1160. /CDROM/140_HONP/BOOK.BIN +0x4F21 (20257) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1161. /CDROM/140_HONP/BOOK.BIN +0x4F38 (20280) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1162. /CDROM/140_HONP/BOOK.BIN +0x4F5A (20314) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1163. /CDROM/140_HONP/BOOK.BIN +0x4F7C (20348) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1164. /CDROM/140_HONP/BOOK.BIN +0x4F96 (20374) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1165. /CDROM/140_HONP/BOOK.BIN +0x4FC0 (20416) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1166. /CDROM/140_HONP/BOOK.BIN +0x4FD6 (20438) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1167. /CDROM/140_HONP/BOOK.BIN +0x4FF1 (20465) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1168. /CDROM/140_HONP/BOOK.BIN +0x5016 (20502) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1169. /CDROM/140_HONP/BOOK.BIN +0x5037 (20535) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1170. /CDROM/140_HONP/BOOK.BIN +0x5053 (20563) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1171. /CDROM/140_HONP/BOOK.BIN +0x5071 (20593) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1172. /CDROM/140_HONP/BOOK.BIN +0x508C (20620) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1173. /CDROM/140_HONP/BOOK.BIN +0x51B1 (20913) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1174. /CDROM/140_HONP/BOOK.BIN +0x51E1 (20961) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1175. /CDROM/140_HONP/BOOK.BIN +0x521E (21022) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1176. /CDROM/140_HONP/BOOK.BIN +0x5246 (21062) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1177. /CDROM/140_HONP/BOOK.BIN +0x5269 (21097) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1178. /CDROM/140_HONP/BOOK.BIN +0x52BC (21180) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1179. /CDROM/140_HONP/BOOK.BIN +0x52EC (21228) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1180. /CDROM/140_HONP/CHIN.BIN +0x64F4 (25844) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1181. /CDROM/140_HONP/CHIN2.BIN +0x64F4 (25844) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1182. /CDROM/140_HONP/FISHING.BIN +0x7E78 (32376) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1183. /CDROM/140_HONP/FISHING.BIN +0x7F17 (32535) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1184. /CDROM/140_HONP/FUDAZUK.BIN +0x6968 (26984) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1185. /CDROM/140_HONP/FUDAZUK.BIN +0x69EC (27116) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1186. /CDROM/140_HONP/HDOUGUYA.BIN +0xB147 (45383) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1187. /CDROM/140_HONP/HDOUGUYA.BIN +0xB1D4 (45524) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1188. /CDROM/140_HONP/HKAJIYA.BIN +0x7C64 (31844) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1189. /CDROM/140_HONP/HKAJIYA.BIN +0x7D14 (32020) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1190. /CDROM/140_HONP/HMONSYOY.BIN +0x8958 (35160) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1191. /CDROM/140_HONP/HMONSYOY.BIN +0x89E8 (35304) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1192. /CDROM/140_HONP/KIKORI.BIN +0xC2AC (49836) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1193. /CDROM/140_HONP/REST.BIN +0x5144 (20804) - Currency name and number spacing
     RETAIL HEX: 201F241318676767A4000000
     v1.2 HEX:   104A1F241318676767A40000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1194. /CDROM/140_HONP/REST.BIN +0x5168 (20840) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1195. /CDROM/140_HONP/SOUKO.BIN +0x8B10 (35600) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1196. /CDROM/140_HONP/SYUGOITM.BIN +0x371F (14111) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1197. /CDROM/140_HONP/TANTEI.BIN +0xFF68 (65384) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1198. /CDROM/140_HONP/TANTEI.BIN +0x1002D (65581) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1199. /CDROM/140_HONP/TANTEI.BIN +0x10145 (65861) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1200. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0x4F9D (20381) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1201. /CDROM/150_BPRG/BUFF0/BP0_AFT.BIN +0x4FA5 (20389) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1202. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23085 (143493) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1203. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22859 (141401) - Currency name capitalization
     RETAIL HEX: 201F241318
     v1.2 HEX:   4A1F241318
     Meaning: 'potch' -> 'Potch'; equal-length sentence.

1204. /SLUS_009.58 +0x81618 (529944) - Currency name and number spacing
     RETAIL HEX: 201F241318000000
     v1.2 HEX:   104A1F2413180000
     Meaning: 'potch' -> ' Potch'; equal-length sentence.

1205. /SLUS_009.58 +0x81A00 (530944) - Currency menu width
     RETAIL HEX: 3800A4FF0B0001000200
     v1.2 HEX:   3800A4FF0C0001000200
     Meaning: Main-menu money window: 11 to 12 cells for six digits, a space, and Potch; only the documented geometry parameter changes.

1206. /CDROM/130_SHOP/KAJIYA1.BIN +0x5220 (21024) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1207. /CDROM/130_SHOP/KAJIYA2.BIN +0x5220 (21024) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1208. /CDROM/130_SHOP/KANTEIY1.BIN +0x2894 (10388) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1209. /CDROM/130_SHOP/KANTEIY2.BIN +0x2894 (10388) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1210. /CDROM/130_SHOP/KOUEKI1.BIN +0x5B18 (23320) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1211. /CDROM/130_SHOP/KOUEKI2.BIN +0x5B18 (23320) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1212. /CDROM/130_SHOP/KOUEKI1.BIN +0x5B88 (23432) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1213. /CDROM/130_SHOP/KOUEKI2.BIN +0x5B88 (23432) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1214. /CDROM/130_SHOP/MONSYOY1.BIN +0x6684 (26244) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1215. /CDROM/130_SHOP/MONSYOY2.BIN +0x6684 (26244) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Money window: 11 to 12 cells for amount and spaced Potch; only the documented geometry parameter changes.

1216. /CDROM/130_SHOP/DOUGUYA1.BIN +0x85E4 (34276) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Owned-money window:11->12; separate price/detail window +0x194 is22 columns and stays unchanged; only the documented geometry parameter changes.

1217. /CDROM/130_SHOP/YADOYA1.BIN +0x2288 (8840) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Inn owned-money window:11->12; only the documented geometry parameter changes.

1218. /CDROM/130_SHOP/DOUGUYA2.BIN +0x85E4 (34276) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Owned-money window:11->12; separate price/detail window +0x194 is22 columns and stays unchanged; only the documented geometry parameter changes.

1219. /CDROM/130_SHOP/YADOYA2.BIN +0x2288 (8840) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Inn owned-money window:11->12; only the documented geometry parameter changes.

1220. /CDROM/140_HONP/HDOUGUYA.BIN +0x8C78 (35960) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: HDOUGUYA money display:11->12; only the documented geometry parameter changes.

1221. /CDROM/140_HONP/HKAJIYA.BIN +0x5A14 (23060) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: HKAJIYA money display:11->12; only the documented geometry parameter changes.

1222. /CDROM/140_HONP/HMONSYOY.BIN +0x6460 (25696) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: HMONSYOY money display:11->12; only the documented geometry parameter changes.

1223. /CDROM/140_HONP/FUDAZUK.BIN +0x4B08 (19208) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: FUDAZUK money display:11->12; only the documented geometry parameter changes.

1224. /CDROM/140_HONP/KIKORI.BIN +0x1CC0 (7360) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: KIKORI money display:11->12; only the documented geometry parameter changes.

1225. /CDROM/140_HONP/REST.BIN +0x628 (1576) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: REST money display:11->12; only the documented geometry parameter changes.

1226. /CDROM/140_HONP/TANTEI.BIN +0x1238 (4664) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: TANTEI money display:11->12; only the documented geometry parameter changes.

1227. /CDROM/140_HONP/CHIN.BIN +0x1B9C (7068) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Chinchirorin owned-money display:11->12; only the documented geometry parameter changes.

1228. /CDROM/140_HONP/CHIN.BIN +0x1D34 (7476) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Chinchirorin result-money display:11->12; only the documented geometry parameter changes.

1229. /CDROM/140_HONP/CHIN.BIN +0x1D6C (7532) - Currency menu width
     RETAIL HEX: 10000624
     v1.2 HEX:   11000624
     Meaning: To go money display:16->17 because five prefix glyphs+six digits+six currency glyphs=17; only the documented geometry parameter changes.

1230. /CDROM/140_HONP/CHIN2.BIN +0x1B9C (7068) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Chinchirorin owned-money display:11->12; only the documented geometry parameter changes.

1231. /CDROM/140_HONP/CHIN2.BIN +0x1D34 (7476) - Currency menu width
     RETAIL HEX: 0B000624
     v1.2 HEX:   0C000624
     Meaning: Chinchirorin result-money display:11->12; only the documented geometry parameter changes.

1232. /CDROM/140_HONP/CHIN2.BIN +0x1D6C (7532) - Currency menu width
     RETAIL HEX: 10000624
     v1.2 HEX:   11000624
     Meaning: To go money display:16->17 because five prefix glyphs+six digits+six currency glyphs=17; only the documented geometry parameter changes.

1233. /CDROM/140_HONP/FISHING.BIN +0x7CE8 (31976) - Currency menu width
     RETAIL HEX: 3800A4FF0B0001000200
     v1.2 HEX:   3800A4FF0C0001000200
     Meaning: Fishing money window table width11->12; only the documented geometry parameter changes.

1234. /CDROM/140_HONP/FISHING.BIN +0x7CFC (31996) - Currency menu width
     RETAIL HEX: 3800C0FF0B0001000200
     v1.2 HEX:   3800C0FF0C0001000200
     Meaning: Fishing money window table width11->12; only the documented geometry parameter changes.

1235. /CDROM/140_HONP/CHIN.BIN +0x1D64 (7524) - Currency menu position
     RETAIL HEX: 9FFF0424
     v1.2 HEX:   97FF0424
     Meaning: Shift To go money window eight pixels left while widening16->17, preserving its original right border and preventing overlap with adjacent owned-money frame; only the documented geometry parameter changes.

1236. /CDROM/140_HONP/CHIN2.BIN +0x1D64 (7524) - Currency menu position
     RETAIL HEX: 9FFF0424
     v1.2 HEX:   97FF0424
     Meaning: Shift To go money window eight pixels left while widening16->17, preserving its original right border and preventing overlap with adjacent owned-money frame; only the documented geometry parameter changes.

1237. /CDROM/130_SHOP/KAJIYA1.BIN +0x25D4 (9684) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1238. /CDROM/130_SHOP/KAJIYA1.BIN +0x3C24 (15396) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1239. /CDROM/130_SHOP/KAJIYA1.BIN +0x4C18 (19480) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1240. /CDROM/130_SHOP/KAJIYA2.BIN +0x25D4 (9684) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1241. /CDROM/130_SHOP/KAJIYA2.BIN +0x3C24 (15396) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1242. /CDROM/130_SHOP/KAJIYA2.BIN +0x4C18 (19480) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1243. /CDROM/130_SHOP/KANTEIY1.BIN +0x2338 (9016) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1244. /CDROM/130_SHOP/KANTEIY2.BIN +0x2338 (9016) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1245. /CDROM/130_SHOP/KOUEKI1.BIN +0x2DA8 (11688) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1246. /CDROM/130_SHOP/KOUEKI1.BIN +0x2E08 (11784) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1247. /CDROM/130_SHOP/KOUEKI1.BIN +0x5714 (22292) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1248. /CDROM/130_SHOP/KOUEKI1.BIN +0x5774 (22388) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1249. /CDROM/130_SHOP/KOUEKI2.BIN +0x2DA8 (11688) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1250. /CDROM/130_SHOP/KOUEKI2.BIN +0x2E08 (11784) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1251. /CDROM/130_SHOP/KOUEKI2.BIN +0x5714 (22292) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1252. /CDROM/130_SHOP/KOUEKI2.BIN +0x5774 (22388) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1253. /CDROM/130_SHOP/MONSYOY1.BIN +0x3144 (12612) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1254. /CDROM/130_SHOP/MONSYOY1.BIN +0x4864 (18532) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1255. /CDROM/130_SHOP/MONSYOY1.BIN +0x6060 (24672) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1256. /CDROM/130_SHOP/MONSYOY2.BIN +0x3144 (12612) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1257. /CDROM/130_SHOP/MONSYOY2.BIN +0x4864 (18532) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1258. /CDROM/130_SHOP/MONSYOY2.BIN +0x6060 (24672) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Keep the full-size currency CURRENT rectangle at12columns after the constructor;6 digits plus leading-space Potch require96px, replacing later88px reset.; only the documented geometry parameter changes.

1259. /CDROM/130_SHOP/DOUGUYA1.BIN +0x3494 (13460) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Owned-money display entering purchase state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1260. /CDROM/130_SHOP/DOUGUYA1.BIN +0x6DBC (28092) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Owned-money display entering sell state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1261. /CDROM/130_SHOP/DOUGUYA1.BIN +0x7898 (30872) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Single-row six-digit currency display using reused detail window: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1262. /CDROM/130_SHOP/DOUGUYA1.BIN +0x81C0 (33216) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Alternate single-row six-digit currency display using reused detail window: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1263. /CDROM/130_SHOP/YADOYA1.BIN +0xFD8 (4056) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Inn single-row owned-money display: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1264. /CDROM/130_SHOP/DOUGUYA2.BIN +0x3494 (13460) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Owned-money display entering purchase state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1265. /CDROM/130_SHOP/DOUGUYA2.BIN +0x6DBC (28092) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Owned-money display entering sell state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1266. /CDROM/130_SHOP/DOUGUYA2.BIN +0x7898 (30872) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Single-row six-digit currency display using reused detail window: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1267. /CDROM/130_SHOP/DOUGUYA2.BIN +0x81C0 (33216) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Alternate single-row six-digit currency display using reused detail window: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1268. /CDROM/130_SHOP/YADOYA2.BIN +0xFD8 (4056) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Inn single-row owned-money display: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1269. /CDROM/140_HONP/FUDAZUK.BIN +0x2E04 (11780) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1270. /CDROM/140_HONP/FUDAZUK.BIN +0x452C (17708) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1271. /CDROM/140_HONP/HDOUGUYA.BIN +0x2FA0 (12192) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1272. /CDROM/140_HONP/HDOUGUYA.BIN +0x738C (29580) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1273. /CDROM/140_HONP/HDOUGUYA.BIN +0x7EA4 (32420) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1274. /CDROM/140_HONP/HDOUGUYA.BIN +0x87CC (34764) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1275. /CDROM/140_HONP/HKAJIYA.BIN +0x2A40 (10816) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1276. /CDROM/140_HONP/HKAJIYA.BIN +0x4274 (17012) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1277. /CDROM/140_HONP/HKAJIYA.BIN +0x5264 (21092) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1278. /CDROM/140_HONP/HMONSYOY.BIN +0x2DB4 (11700) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1279. /CDROM/140_HONP/HMONSYOY.BIN +0x45E4 (17892) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1280. /CDROM/140_HONP/HMONSYOY.BIN +0x5DDC (24028) - Currency menu active width
     RETAIL HEX: 0B000524
     v1.2 HEX:   0C000524
     Meaning: Currency-bearing single-row full-size state: current text rectangle11->12 columns, retaining constructor grid and all other states; only the documented geometry parameter changes.

1281. /CDROM/080_ARH/VH02.BIN +0x1028 (4136) - Clive Lakewest deadline removed
     RETAIL HEX: 0C006018
     v1.2 HEX:   0C000010
     Meaning: Original 11-hour elapsed-playtime check now always selects its existing on-time path; global clock, delay slot and other quest prerequisites unchanged.

1282. /CDROM/050_ARE/VE02.BIN +0x1284 (4740) - Clive Forest Village deadline removed
     RETAIL HEX: 0C006018
     v1.2 HEX:   0C000010
     Meaning: Original 13-hour elapsed-playtime check now always selects its existing on-time path; global clock, delay slot and other quest prerequisites unchanged.

1283. /CDROM/090_ARI/VI01.BIN +0x4B8 (1208) - Clive Rockaxe deadline removed
     RETAIL HEX: 0C006018
     v1.2 HEX:   0C000010
     Meaning: Original 14-hour elapsed-playtime check now always selects its existing on-time path; global clock, delay slot and other quest prerequisites unchanged.

1284. /CDROM/040_ARD/VD19.BIN +0x17F4 (6132) - Clive Radat deadline removed
     RETAIL HEX: 0C006018
     v1.2 HEX:   0C000010
     Meaning: Original 15-hour elapsed-playtime check now always selects its existing on-time path; global clock, delay slot and other quest prerequisites unchanged.

1285. /CDROM/100_ARJ/VJ17.BIN +0xBCC (3020) - Clive Sajah deadline removed
     RETAIL HEX: 0C006018
     v1.2 HEX:   0C000010
     Meaning: Original 20-hour elapsed-playtime check now always selects its existing on-time path; global clock, delay slot and other quest prerequisites unchanged.

10. NEW IN v1.2 - CLIVE ELAPSED DEADLINES
The five local callbacks accept late arrivals at Lakewest, Forest Village,
Rockaxe, Radat and Sajah. All prior edits remain unchanged. The normal clock
continues running. Story access and existing one-time quest flags remain;
already failed saves are not automatically repaired. No other Pyriel fixes
are newly bundled. Static/CPU coverage is distinct from the native Radat test.

11. RETAINED BEHAVIOR AND LIMITS
All 269 v1.0 guarded edits remain intact. v1.1 adds 1011 bounded text,
reviewed spelling and money-window width edits. No combat numbers, growth settings, rune slots, item stats, enemy/boss
stats, EXP, economy or audio changed relative to v1.0.
Chuchara special J ranks and Tuta SPD remain retail. The conditional
Fury x Double-Strike cap remains omitted; no uniform character parity is claimed.
The signed Kindness penalty is preserved; only its unsigned-wrap bug is fixed.
Use your own exact legal USA original. This patch does not migrate vanilla
save growth tables or retroactively change earned stats. A new game is recommended.
Correctly migrated v0.99/v1.0 saves need no additional table migration for v1.2.
Linux tests and selected downloaded-save routes are bounded evidence.
Full campaign difficulty, every legal recruitment/loadout/Unite scenario,
endings and real hardware remain outside the completed verification scope.
