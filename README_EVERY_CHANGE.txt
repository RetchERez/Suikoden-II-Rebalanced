SUIKODEN II: COMBAT REBALANCED v1.0 Final
EVERY CHANGE FROM UNMODIFIED USA SLUS-00958
By RetchERezzed

Original BIN SHA-256: acf1c55394797c4ef33bdb297cb4fcdefeb4885be84928ed5a82a0d7d3fcd472
Final BIN SHA-256:    5e8233950e3ee0bdaf6a7fa180ea16da955e01b5b0c52f12dd769a8d357c1bde
xdelta SHA-256:       1d37961d3e003000d72e2d594a425cb08a2ac2c88d5d34fb08cdfdcfab45c5cc

This ledger enumerates every guarded manifest edit: 269 entries across 72
game files, with 1,318 differing payload bytes. 80 changed raw CD sectors
have verified EDC/ECC; 6,303 raw bytes differ including check bytes.
Every untouched sector is identical. Every guarded span keeps its original
length. Exact hexadecimal spans and file-relative offsets are authoritative.
This is a binary change ledger, not certification of every gameplay outcome.

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

8. EXACT MANIFEST EDITS - ALL 269 ENTRIES

001. /CDROM/280_GAME/ALL.BIN +0x210 (528) - Shin SPD
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

002. /CDROM/280_GAME/ALL.BIN +0x211 (529) - Shin HP
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

003. /CDROM/280_GAME/ALL.BIN +0x233 (563) - Tomo PROT
     RETAIL HEX: 44
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

004. /CDROM/280_GAME/ALL.BIN +0x235 (565) - Tomo HP
     RETAIL HEX: 44
     FINAL HEX:  45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

005. /CDROM/280_GAME/ALL.BIN +0x27C (636) - Bolgan DEX, Bolgan SPD
     RETAIL HEX: 21
     FINAL HEX:  33
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

006. /CDROM/280_GAME/ALL.BIN +0x28C (652) - Tuta MAG
     RETAIL HEX: 22
     FINAL HEX:  23
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

007. /CDROM/280_GAME/ALL.BIN +0x28F (655) - Tuta HP
     RETAIL HEX: 50
     FINAL HEX:  52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

008. /CDROM/280_GAME/ALL.BIN +0x29E (670) - Hanna STR
     RETAIL HEX: 52
     FINAL HEX:  62
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

009. /CDROM/280_GAME/ALL.BIN +0x2A0 (672) - Hanna SPD
     RETAIL HEX: 53
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

010. /CDROM/280_GAME/ALL.BIN +0x2B0 (688) - Millie MAG
     RETAIL HEX: 24
     FINAL HEX:  25
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

011. /CDROM/280_GAME/ALL.BIN +0x2B3 (691) - Millie HP
     RETAIL HEX: 73
     FINAL HEX:  74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

012. /CDROM/280_GAME/ALL.BIN +0x2F8 (760) - Gengen STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

013. /CDROM/280_GAME/ALL.BIN +0x2F9 (761) - Gengen PROT
     RETAIL HEX: 42
     FINAL HEX:  52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

014. /CDROM/280_GAME/ALL.BIN +0x2FB (763) - Gengen HP
     RETAIL HEX: 64
     FINAL HEX:  65
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

015. /CDROM/280_GAME/ALL.BIN +0x30A (778) - Gabocha STR
     RETAIL HEX: 33
     FINAL HEX:  43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

016. /CDROM/280_GAME/ALL.BIN +0x30C (780) - Gabocha SPD
     RETAIL HEX: 65
     FINAL HEX:  66
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

017. /CDROM/280_GAME/ALL.BIN +0x30D (781) - Gabocha HP
     RETAIL HEX: 63
     FINAL HEX:  64
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

018. /CDROM/280_GAME/ALL.BIN +0x32E (814) - Shilo STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

019. /CDROM/280_GAME/ALL.BIN +0x330 (816) - Shilo SPD
     RETAIL HEX: 84
     FINAL HEX:  85
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

020. /CDROM/280_GAME/ALL.BIN +0x376 (886) - Freed Y STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

021. /CDROM/280_GAME/ALL.BIN +0x379 (889) - Freed Y HP
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

022. /CDROM/280_GAME/ALL.BIN +0x3E2 (994) - Meg MAG
     RETAIL HEX: 33
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

023. /CDROM/280_GAME/ALL.BIN +0x3E5 (997) - Meg HP
     RETAIL HEX: 73
     FINAL HEX:  74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

024. /CDROM/280_GAME/ALL.BIN +0x3F4 (1012) - Gadget STR
     RETAIL HEX: 40
     FINAL HEX:  50
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

025. /CDROM/280_GAME/ALL.BIN +0x3F7 (1015) - Gadget HP
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

026. /CDROM/280_GAME/ALL.BIN +0x44E (1102) - Genshu STR
     RETAIL HEX: 53
     FINAL HEX:  63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

027. /CDROM/280_GAME/ALL.BIN +0x450 (1104) - Genshu SPD
     RETAIL HEX: 55
     FINAL HEX:  56
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

028. /CDROM/280_GAME/ALL.BIN +0x451 (1105) - Genshu HP
     RETAIL HEX: 54
     FINAL HEX:  55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

029. /CDROM/280_GAME/ALL.BIN +0x4A8 (1192) - Tsai STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

030. /CDROM/280_GAME/ALL.BIN +0x4AA (1194) - Tsai SPD
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

031. /CDROM/280_GAME/ALL.BIN +0x4F0 (1264) - Sid STR, Sid MAG
     RETAIL HEX: 43
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

032. /CDROM/280_GAME/ALL.BIN +0x502 (1282) - Yoshino MAG
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

033. /CDROM/280_GAME/ALL.BIN +0x505 (1285) - Yoshino HP
     RETAIL HEX: 54
     FINAL HEX:  55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

034. /CDROM/280_GAME/ALL.BIN +0x526 (1318) - Koyu STR
     RETAIL HEX: 33
     FINAL HEX:  43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

035. /CDROM/280_GAME/ALL.BIN +0x527 (1319) - Koyu PROT
     RETAIL HEX: 35
     FINAL HEX:  45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

036. /CDROM/280_GAME/ALL.BIN +0x538 (1336) - Lo Wen STR
     RETAIL HEX: 53
     FINAL HEX:  63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

037. /CDROM/280_GAME/ALL.BIN +0x53A (1338) - Lo Wen DEX
     RETAIL HEX: 44
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

038. /CDROM/280_GAME/ALL.BIN +0x580 (1408) - Vincent MAG
     RETAIL HEX: 43
     FINAL HEX:  44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

039. /CDROM/280_GAME/ALL.BIN +0x583 (1411) - Vincent HP
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

040. /CDROM/280_GAME/ALL.BIN +0x592 (1426) - Simone MAG
     RETAIL HEX: 44
     FINAL HEX:  45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

041. /CDROM/280_GAME/ALL.BIN +0x595 (1429) - Simone HP
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

042. /CDROM/280_GAME/ALL.BIN +0x5A4 (1444) - Hai Yo STR
     RETAIL HEX: 33
     FINAL HEX:  43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

043. /CDROM/280_GAME/ALL.BIN +0x5A6 (1446) - Hai Yo DEX
     RETAIL HEX: 34
     FINAL HEX:  44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

044. /CDROM/280_GAME/ALL.BIN +0x5FE (1534) - Hoi STR
     RETAIL HEX: 32
     FINAL HEX:  42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

045. /CDROM/280_GAME/ALL.BIN +0x5FF (1535) - Hoi PROT
     RETAIL HEX: 32
     FINAL HEX:  42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

046. /CDROM/280_GAME/ALL.BIN +0x601 (1537) - Hoi HP
     RETAIL HEX: 73
     FINAL HEX:  74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

047. /CDROM/280_GAME/KOTEI.BIN +0x110 (272) - Shin SPD
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

048. /CDROM/280_GAME/KOTEI.BIN +0x111 (273) - Shin HP
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

049. /CDROM/280_GAME/KOTEI.BIN +0x133 (307) - Tomo PROT
     RETAIL HEX: 44
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

050. /CDROM/280_GAME/KOTEI.BIN +0x135 (309) - Tomo HP
     RETAIL HEX: 44
     FINAL HEX:  45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

051. /CDROM/280_GAME/KOTEI.BIN +0x17C (380) - Bolgan DEX, Bolgan SPD
     RETAIL HEX: 21
     FINAL HEX:  33
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

052. /CDROM/280_GAME/KOTEI.BIN +0x18C (396) - Tuta MAG
     RETAIL HEX: 22
     FINAL HEX:  23
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

053. /CDROM/280_GAME/KOTEI.BIN +0x18F (399) - Tuta HP
     RETAIL HEX: 50
     FINAL HEX:  52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

054. /CDROM/280_GAME/KOTEI.BIN +0x19E (414) - Hanna STR
     RETAIL HEX: 52
     FINAL HEX:  62
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

055. /CDROM/280_GAME/KOTEI.BIN +0x1A0 (416) - Hanna SPD
     RETAIL HEX: 53
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

056. /CDROM/280_GAME/KOTEI.BIN +0x1B0 (432) - Millie MAG
     RETAIL HEX: 23
     FINAL HEX:  25
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

057. /CDROM/280_GAME/KOTEI.BIN +0x1B3 (435) - Millie HP
     RETAIL HEX: 73
     FINAL HEX:  74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

058. /CDROM/280_GAME/KOTEI.BIN +0x1F8 (504) - Gengen STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

059. /CDROM/280_GAME/KOTEI.BIN +0x1F9 (505) - Gengen PROT
     RETAIL HEX: 42
     FINAL HEX:  52
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

060. /CDROM/280_GAME/KOTEI.BIN +0x1FB (507) - Gengen HP
     RETAIL HEX: 64
     FINAL HEX:  65
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

061. /CDROM/280_GAME/KOTEI.BIN +0x20A (522) - Gabocha STR
     RETAIL HEX: 33
     FINAL HEX:  43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

062. /CDROM/280_GAME/KOTEI.BIN +0x20C (524) - Gabocha SPD
     RETAIL HEX: 65
     FINAL HEX:  66
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

063. /CDROM/280_GAME/KOTEI.BIN +0x20D (525) - Gabocha HP
     RETAIL HEX: 63
     FINAL HEX:  64
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

064. /CDROM/280_GAME/KOTEI.BIN +0x22E (558) - Shilo STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

065. /CDROM/280_GAME/KOTEI.BIN +0x230 (560) - Shilo SPD
     RETAIL HEX: 84
     FINAL HEX:  85
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

066. /CDROM/280_GAME/KOTEI.BIN +0x276 (630) - Freed Y STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

067. /CDROM/280_GAME/KOTEI.BIN +0x279 (633) - Freed Y HP
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

068. /CDROM/280_GAME/KOTEI.BIN +0x2E2 (738) - Meg MAG
     RETAIL HEX: 33
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

069. /CDROM/280_GAME/KOTEI.BIN +0x2E5 (741) - Meg HP
     RETAIL HEX: 73
     FINAL HEX:  74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

070. /CDROM/280_GAME/KOTEI.BIN +0x2F4 (756) - Gadget STR
     RETAIL HEX: 40
     FINAL HEX:  50
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

071. /CDROM/280_GAME/KOTEI.BIN +0x2F7 (759) - Gadget HP
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

072. /CDROM/280_GAME/KOTEI.BIN +0x34E (846) - Genshu STR
     RETAIL HEX: 53
     FINAL HEX:  63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

073. /CDROM/280_GAME/KOTEI.BIN +0x350 (848) - Genshu SPD
     RETAIL HEX: 55
     FINAL HEX:  56
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

074. /CDROM/280_GAME/KOTEI.BIN +0x351 (849) - Genshu HP
     RETAIL HEX: 54
     FINAL HEX:  55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

075. /CDROM/280_GAME/KOTEI.BIN +0x3A8 (936) - Tsai STR
     RETAIL HEX: 43
     FINAL HEX:  53
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

076. /CDROM/280_GAME/KOTEI.BIN +0x3AA (938) - Tsai SPD
     RETAIL HEX: 74
     FINAL HEX:  75
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

077. /CDROM/280_GAME/KOTEI.BIN +0x3F0 (1008) - Sid STR, Sid MAG
     RETAIL HEX: 43
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

078. /CDROM/280_GAME/KOTEI.BIN +0x402 (1026) - Yoshino MAG
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

079. /CDROM/280_GAME/KOTEI.BIN +0x405 (1029) - Yoshino HP
     RETAIL HEX: 54
     FINAL HEX:  55
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

080. /CDROM/280_GAME/KOTEI.BIN +0x426 (1062) - Koyu STR
     RETAIL HEX: 33
     FINAL HEX:  43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

081. /CDROM/280_GAME/KOTEI.BIN +0x427 (1063) - Koyu PROT
     RETAIL HEX: 35
     FINAL HEX:  45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

082. /CDROM/280_GAME/KOTEI.BIN +0x438 (1080) - Lo Wen STR
     RETAIL HEX: 53
     FINAL HEX:  63
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

083. /CDROM/280_GAME/KOTEI.BIN +0x43A (1082) - Lo Wen DEX
     RETAIL HEX: 44
     FINAL HEX:  54
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

084. /CDROM/280_GAME/KOTEI.BIN +0x480 (1152) - Vincent MAG
     RETAIL HEX: 43
     FINAL HEX:  44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

085. /CDROM/280_GAME/KOTEI.BIN +0x483 (1155) - Vincent HP
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

086. /CDROM/280_GAME/KOTEI.BIN +0x492 (1170) - Simone MAG
     RETAIL HEX: 44
     FINAL HEX:  45
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

087. /CDROM/280_GAME/KOTEI.BIN +0x495 (1173) - Simone HP
     RETAIL HEX: 34
     FINAL HEX:  35
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

088. /CDROM/280_GAME/KOTEI.BIN +0x4A4 (1188) - Hai Yo STR
     RETAIL HEX: 33
     FINAL HEX:  43
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

089. /CDROM/280_GAME/KOTEI.BIN +0x4A6 (1190) - Hai Yo DEX
     RETAIL HEX: 34
     FINAL HEX:  44
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

090. /CDROM/280_GAME/KOTEI.BIN +0x4FE (1278) - Hoi STR
     RETAIL HEX: 32
     FINAL HEX:  42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

091. /CDROM/280_GAME/KOTEI.BIN +0x4FF (1279) - Hoi PROT
     RETAIL HEX: 32
     FINAL HEX:  42
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

092. /CDROM/280_GAME/KOTEI.BIN +0x501 (1281) - Hoi HP
     RETAIL HEX: 73
     FINAL HEX:  74
     Meaning: Packed growth-rank byte; logical rank changes are listed in section 1.

093. /CDROM/280_GAME/ALL.BIN +0x29A (666) - Tuta head unlock
     RETAIL HEX: 23
     FINAL HEX:  19
     Meaning: Head rune slot level threshold: 35 -> 25.

094. /CDROM/280_GAME/ALL.BIN +0x2BE (702) - Millie head unlock
     RETAIL HEX: 23
     FINAL HEX:  1E
     Meaning: Head rune slot level threshold: 35 -> 30.

095. /CDROM/280_GAME/ALL.BIN +0x5B2 (1458) - Hai Yo head unlock
     RETAIL HEX: 41
     FINAL HEX:  2D
     Meaning: Head rune slot level threshold: 65 -> 45.

096. /CDROM/280_GAME/ALL.BIN +0x60C (1548) - Hoi head unlock
     RETAIL HEX: 50
     FINAL HEX:  23
     Meaning: Head rune slot level threshold: 80 -> 35.

097. /CDROM/280_GAME/MAGI.BIN +0x13FC (5116) - Personal physical damage coefficient
     RETAIL HEX: 2C01
     FINAL HEX:  AF00
     Meaning: Trick (spell 79, rune 39) coefficient: 300% -> 175%.

098. /CDROM/280_GAME/MAGI.BIN +0x14BC (5308) - Personal physical damage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Mayfly (spell 82, rune 42) coefficient: 100% -> 125%.

099. /CDROM/280_GAME/MAGI.BIN +0x14FC (5372) - Personal physical damage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  9600
     Meaning: Swallow (spell 83, rune 43) coefficient: 100% -> 150%.

100. /CDROM/280_GAME/MAGI.BIN +0x157C (5500) - Personal physical damage coefficient
     RETAIL HEX: C800
     FINAL HEX:  9600
     Meaning: Groundhog (spell 85, rune 45) coefficient: 200% -> 150%.

101. /CDROM/280_GAME/MAGI.BIN +0x17FC (6140) - Personal physical damage coefficient
     RETAIL HEX: 2C01
     FINAL HEX:  C800
     Meaning: Spider Slay (spell 95, rune 51) coefficient: 300% -> 200%.

102. /CDROM/280_GAME/MAGI.BIN +0x13D5 (5077) - Personal rune description
     RETAIL HEX: 51191E2520103E1F1C1C103B4E456510991024191D1500000000000000000000
     FINAL HEX:  99669F9D28103E4741104C152015112411121C15000000000000000000000000
     Meaning: Spell 79 menu text: 'Winup Doll ATK<65> 1 time' -> '1.75x DMG Repeatable'.

103. /CDROM/280_GAME/MAGI.BIN +0x1555 (5461) - Personal rune description
     RETAIL HEX: 9A10281014111D11171510991024191D15101F1E1C2900000000000000000000
     FINAL HEX:  99669D28103E4741104C152015112411121C1500000000000000000000000000
     Meaning: Spell 85 menu text: '2 x damage 1 time only' -> '1.5x DMG Repeatable'.

104. /CDROM/280_GAME/MAGI.BIN +0x17D5 (6101) - Personal rune description
     RETAIL HEX: 9B10281014111D11171510991024191D15101F1E1C2900000000000000000000
     FINAL HEX:  9A28103E4741104C152015112411121C15000000000000000000000000000000
     Meaning: Spell 95 menu text: '3 x damage 1 time only' -> '2x DMG Repeatable'.

105. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0xAE00 (44544) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 01004230
     FINAL HEX:  00004230
     Meaning: Trick rune-specific used-bit availability test mask 0x1 -> 0x0 at guest 0x80035e00; used-bit writer and other gates unchanged.

106. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0xAE0C (44556) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 02004230
     FINAL HEX:  00004230
     Meaning: Groundhog rune-specific used-bit availability test mask 0x2 -> 0x0 at guest 0x80035e0c; used-bit writer and other gates unchanged.

107. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0xAE50 (44624) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 04004230
     FINAL HEX:  00004230
     Meaning: Spider Slay rune-specific used-bit availability test mask 0x4 -> 0x0 at guest 0x80035e50; used-bit writer and other gates unchanged.

108. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0xA5B8 (42424) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 01004230
     FINAL HEX:  00004230
     Meaning: Trick rune-specific used-bit availability test mask 0x1 -> 0x0 at guest 0x800355b8; used-bit writer and other gates unchanged.

109. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0xA5C4 (42436) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 02004230
     FINAL HEX:  00004230
     Meaning: Groundhog rune-specific used-bit availability test mask 0x2 -> 0x0 at guest 0x800355c4; used-bit writer and other gates unchanged.

110. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0xA608 (42504) - Rune-specific once-per-battle availability gate
     RETAIL HEX: 04004230
     FINAL HEX:  00004230
     Meaning: Spider Slay rune-specific used-bit availability test mask 0x4 -> 0x0 at guest 0x80035608; used-bit writer and other gates unchanged.

111. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2364C (144972) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Kobold Attack record ID 3; participants [28, 29]; coefficient 100% -> 125%.

112. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2361E (144926) - description
     RETAIL HEX: 991028103E4741102623661099103F10680E4111121F131811104F1E12111C111E131500
     FINAL HEX:  99669A9D283E47411026236699103F10680E4111121F131811104F1E12111C111E131500
     Meaning: Kobold Attack record ID 3 menu text: '1 x DMG vs. 1 E <68> / Gabocha Unbalance' -> '1.25xDMG vs.1 E <68> / Gabocha Unbalance'.

113. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x237C8 (145352) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Bow Wow Attack record ID 8; participants [28, 26]; coefficient 150% -> 175%.

114. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2379A (145306) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 8 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

115. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23814 (145428) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Bow Wow Attack record ID 9; participants [29, 26]; coefficient 150% -> 175%.

116. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x237E6 (145382) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 9 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

117. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x238F8 (145656) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Bow Attack record ID 12; participants [30, 43]; coefficient 50% -> 75%.

118. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x238CA (145610) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 12 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

119. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23944 (145732) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Bow Attack record ID 13; participants [30, 67]; coefficient 50% -> 75%.

120. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23916 (145686) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 13 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

121. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23990 (145808) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Bow Attack record ID 14; participants [43, 67]; coefficient 50% -> 75%.

122. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23962 (145762) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 14 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

123. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A28 (145960) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Narcissists Attack record ID 16; participants [64, 65]; coefficient 50% -> 75%.

124. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x239FA (145914) - description
     RETAIL HEX: 98669D1028103E474110241F0E111C1C103F230000000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E474110241F0E111C1C103F2300000000000000000000000000000000
     Meaning: Narcissists Attack record ID 16 menu text: '0.5 x DMG to / all Es' -> '0.75 x DMG to / all Es'.

125. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A74 (146036) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Winger Attack record ID 17; participants [54, 56]; coefficient 150% -> 175%.

126. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A46 (145990) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A000000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A0000000000
     Meaning: Winger Attack record ID 17 menu text: '1.5 x DMG vs. 1 E / Poison <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Poison <69>30<94><6A>'.

127. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23AC0 (146112) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Dad & Daughter Attack record ID 18; participants [52, 17]; coefficient 100% -> 125%.

128. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23A92 (146066) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     FINAL HEX:  99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Dad & Daughter Attack record ID 18 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

129. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C3C (146492) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Double Kraken Attack record ID 23; participants [49, 74]; coefficient 100% -> 125%.

130. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C0E (146446) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     FINAL HEX:  99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Double Kraken Attack record ID 23 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

131. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C88 (146568) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Swordsman Attack record ID 24; participants [15, 47]; coefficient 50% -> 75%.

132. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23C5A (146522) - description
     RETAIL HEX: 98669D283E47411026236610111C1C103F230E4D251414151E101415112418109A989400
     FINAL HEX:  98669F9D283E474110262366111C1C103F230E4D251414151E101415112418109A989400
     Meaning: Swordsman Attack record ID 24 menu text: '0.5xDMG vs. all Es / Sudden death 20<94>' -> '0.75xDMG vs.all Es / Sudden death 20<94>'.

133. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23CD4 (146644) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  9600
     Meaning: Copycat Attack record ID 25; participants [1, 71]; coefficient 100% -> 150%.

134. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23CA6 (146598) - description
     RETAIL HEX: 991028103E4741102623661099103F000000000000000000000000000000000000000000
     FINAL HEX:  99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     Meaning: Copycat Attack record ID 25 menu text: '1 x DMG vs. 1 E' -> '1.5 x DMG vs. 1 E'.

135. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23D6C (146796) - percentage coefficient
     RETAIL HEX: C800
     FINAL HEX:  E100
     Meaning: Circus Attack record ID 27; participants [19, 20, 21]; coefficient 200% -> 225%.

136. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23D3E (146750) - description
     RETAIL HEX: 9A1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500000000
     FINAL HEX:  9A669A9D1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500
     Meaning: Circus Attack record ID 27 menu text: '2 x DMG vs. 1 E / Bolgan Unbalance' -> '2.25 x DMG vs. 1 E / Bolgan Unbalance'.

137. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23FCC (147404) - percentage coefficient
     RETAIL HEX: 4B00
     FINAL HEX:  6400
     Meaning: Tackle Attack record ID 35; participants [23, 46]; coefficient 75% -> 100%.

138. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x23F9E (147358) - description
     RETAIL HEX: 98669F9D1028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000
     FINAL HEX:  991028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000000000
     Meaning: Tackle Attack record ID 35 menu text: '0.75 x DMG vs. / all Es Unbalance' -> '1 x DMG vs. / all Es Unbalance'.

139. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x240B0 (147632) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Pretty Girl Attack record ID 38; participants [8, 24, 41]; coefficient 50% -> 75%.

140. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x24082 (147586) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 38 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

141. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x240FC (147708) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Pretty Girl Attack record ID 39; participants [8, 83, 41]; coefficient 50% -> 75%.

142. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x240CE (147662) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 39 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

143. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2411A (147738) - description
     RETAIL HEX: 99283E47411026236610111C1C103F230E4111121F131811104F1E12111C111E13150000
     FINAL HEX:  9B283E47411026236610111C1C103F230E3C1F2418104F1E12111C111E13150000000000
     Meaning: 100 Kobold Attack record ID 40 menu text: '1xDMG vs. all Es / Gabocha Unbalance' -> '3xDMG vs. all Es / Both Unbalance'.

144. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x241E0 (147936) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Bandit Attack record ID 42; participants [58, 59, 60]; coefficient 150% -> 175%.

145. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x241B2 (147890) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A0000
     Meaning: Bandit Attack record ID 42 menu text: '1.5 x DMG vs. 1 E / Knockdown <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Knockdown <69>30<94><6A>'.

146. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2435C (148316) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 47; participants [51, 49, 74]; coefficient 150% -> 175%.

147. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2432E (148270) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 47 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

148. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x243A8 (148392) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 48; participants [51, 49, 72]; coefficient 150% -> 175%.

149. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x2437A (148346) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 48 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

150. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x243F4 (148468) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 49; participants [51, 49, 50]; coefficient 150% -> 175%.

151. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x243C6 (148422) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 49 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

152. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x24440 (148544) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 50; participants [51, 72, 50]; coefficient 150% -> 175%.

153. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x24412 (148498) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 50 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

154. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x1EC74 (126068) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     FINAL HEX:  E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

155. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x1EC98 (126104) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     FINAL HEX:  E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

156. /CDROM/150_BPRG/BUFF0/BP0_FST.BIN +0x1ECBC (126140) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     FINAL HEX:  E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

157. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22E20 (142880) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Kobold Attack record ID 3; participants [28, 29]; coefficient 100% -> 125%.

158. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22DF2 (142834) - description
     RETAIL HEX: 991028103E4741102623661099103F10680E4111121F131811104F1E12111C111E131500
     FINAL HEX:  99669A9D283E47411026236699103F10680E4111121F131811104F1E12111C111E131500
     Meaning: Kobold Attack record ID 3 menu text: '1 x DMG vs. 1 E <68> / Gabocha Unbalance' -> '1.25xDMG vs.1 E <68> / Gabocha Unbalance'.

159. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22F9C (143260) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Bow Wow Attack record ID 8; participants [28, 26]; coefficient 150% -> 175%.

160. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22F6E (143214) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 8 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

161. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22FE8 (143336) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Bow Wow Attack record ID 9; participants [29, 26]; coefficient 150% -> 175%.

162. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x22FBA (143290) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F000000000000000000000000000000000000
     Meaning: Bow Wow Attack record ID 9 menu text: '1.5 x DMG vs. 1 E' -> '1.75 x DMG vs. 1 E'.

163. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x230CC (143564) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Bow Attack record ID 12; participants [30, 43]; coefficient 50% -> 75%.

164. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2309E (143518) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 12 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

165. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23118 (143640) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Bow Attack record ID 13; participants [30, 67]; coefficient 50% -> 75%.

166. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x230EA (143594) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 13 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

167. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23164 (143716) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Bow Attack record ID 14; participants [43, 67]; coefficient 50% -> 75%.

168. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23136 (143670) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Bow Attack record ID 14 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

169. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x231FC (143868) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Narcissists Attack record ID 16; participants [64, 65]; coefficient 50% -> 75%.

170. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x231CE (143822) - description
     RETAIL HEX: 98669D1028103E474110241F0E111C1C103F230000000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E474110241F0E111C1C103F2300000000000000000000000000000000
     Meaning: Narcissists Attack record ID 16 menu text: '0.5 x DMG to / all Es' -> '0.75 x DMG to / all Es'.

171. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23248 (143944) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Winger Attack record ID 17; participants [54, 56]; coefficient 150% -> 175%.

172. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2321A (143898) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A000000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E4A1F19231F1E10699B98946A0000000000
     Meaning: Winger Attack record ID 17 menu text: '1.5 x DMG vs. 1 E / Poison <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Poison <69>30<94><6A>'.

173. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23294 (144020) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Dad & Daughter Attack record ID 18; participants [52, 17]; coefficient 100% -> 125%.

174. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23266 (143974) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     FINAL HEX:  99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Dad & Daughter Attack record ID 18 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

175. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23410 (144400) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  7D00
     Meaning: Double Kraken Attack record ID 23; participants [49, 74]; coefficient 100% -> 125%.

176. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x233E2 (144354) - description
     RETAIL HEX: 991028103E4741102623660E16221F1E2410221F27000000000000000000000000000000
     FINAL HEX:  99669A9D1028103E4741102623660E16221F1E2410221F27000000000000000000000000
     Meaning: Double Kraken Attack record ID 23 menu text: '1 x DMG vs. / front row' -> '1.25 x DMG vs. / front row'.

177. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2345C (144476) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Swordsman Attack record ID 24; participants [15, 47]; coefficient 50% -> 75%.

178. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2342E (144430) - description
     RETAIL HEX: 98669D283E47411026236610111C1C103F230E4D251414151E101415112418109A989400
     FINAL HEX:  98669F9D283E474110262366111C1C103F230E4D251414151E101415112418109A989400
     Meaning: Swordsman Attack record ID 24 menu text: '0.5xDMG vs. all Es / Sudden death 20<94>' -> '0.75xDMG vs.all Es / Sudden death 20<94>'.

179. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x234A8 (144552) - percentage coefficient
     RETAIL HEX: 6400
     FINAL HEX:  9600
     Meaning: Copycat Attack record ID 25; participants [1, 71]; coefficient 100% -> 150%.

180. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x2347A (144506) - description
     RETAIL HEX: 991028103E4741102623661099103F000000000000000000000000000000000000000000
     FINAL HEX:  99669D1028103E4741102623661099103F00000000000000000000000000000000000000
     Meaning: Copycat Attack record ID 25 menu text: '1 x DMG vs. 1 E' -> '1.5 x DMG vs. 1 E'.

181. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23540 (144704) - percentage coefficient
     RETAIL HEX: C800
     FINAL HEX:  E100
     Meaning: Circus Attack record ID 27; participants [19, 20, 21]; coefficient 200% -> 225%.

182. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23512 (144658) - description
     RETAIL HEX: 9A1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500000000
     FINAL HEX:  9A669A9D1028103E4741102623661099103F0E3C1F1C17111E104F1E12111C111E131500
     Meaning: Circus Attack record ID 27 menu text: '2 x DMG vs. 1 E / Bolgan Unbalance' -> '2.25 x DMG vs. 1 E / Bolgan Unbalance'.

183. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x237A0 (145312) - percentage coefficient
     RETAIL HEX: 4B00
     FINAL HEX:  6400
     Meaning: Tackle Attack record ID 35; participants [23, 46]; coefficient 75% -> 100%.

184. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23772 (145266) - description
     RETAIL HEX: 98669F9D1028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000
     FINAL HEX:  991028103E4741102623660E111C1C103F23104F1E12111C111E13150000000000000000
     Meaning: Tackle Attack record ID 35 menu text: '0.75 x DMG vs. / all Es Unbalance' -> '1 x DMG vs. / all Es Unbalance'.

185. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23884 (145540) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Pretty Girl Attack record ID 38; participants [8, 24, 41]; coefficient 50% -> 75%.

186. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23856 (145494) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 38 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

187. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x238D0 (145616) - percentage coefficient
     RETAIL HEX: 3200
     FINAL HEX:  4B00
     Meaning: Pretty Girl Attack record ID 39; participants [8, 83, 41]; coefficient 50% -> 75%.

188. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x238A2 (145570) - description
     RETAIL HEX: 98669D1028103E4741102623660E111C1C103F2300000000000000000000000000000000
     FINAL HEX:  98669F9D1028103E4741102623660E111C1C103F23000000000000000000000000000000
     Meaning: Pretty Girl Attack record ID 39 menu text: '0.5 x DMG vs. / all Es' -> '0.75 x DMG vs. / all Es'.

189. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x238EE (145646) - description
     RETAIL HEX: 99283E47411026236610111C1C103F230E4111121F131811104F1E12111C111E13150000
     FINAL HEX:  9B283E47411026236610111C1C103F230E3C1F2418104F1E12111C111E13150000000000
     Meaning: 100 Kobold Attack record ID 40 menu text: '1xDMG vs. all Es / Gabocha Unbalance' -> '3xDMG vs. all Es / Both Unbalance'.

190. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x239B4 (145844) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Bandit Attack record ID 42; participants [58, 59, 60]; coefficient 150% -> 175%.

191. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23986 (145798) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E451E1F131B141F271E10699B98946A0000
     Meaning: Bandit Attack record ID 42 menu text: '1.5 x DMG vs. 1 E / Knockdown <69>30<94><6A>' -> '1.75 x DMG vs. 1 E / Knockdown <69>30<94><6A>'.

192. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B30 (146224) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 47; participants [51, 49, 74]; coefficient 150% -> 175%.

193. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B02 (146178) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 47 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

194. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B7C (146300) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 48; participants [51, 49, 72]; coefficient 150% -> 175%.

195. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B4E (146254) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 48 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

196. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23BC8 (146376) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 49; participants [51, 49, 50]; coefficient 150% -> 175%.

197. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23B9A (146330) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 49 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

198. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23C14 (146452) - percentage coefficient
     RETAIL HEX: 9600
     FINAL HEX:  AF00
     Meaning: Beastmaster Attack record ID 50; participants [51, 72, 50]; coefficient 150% -> 175%.

199. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x23BE6 (146406) - description
     RETAIL HEX: 99669D1028103E4741102623661099103F0E47111B1523101215222315221B0000000000
     FINAL HEX:  99669F9D1028103E4741102623661099103F0E47111B1523101215222315221B00000000
     Meaning: Beastmaster Attack record ID 50 menu text: '1.5 x DMG vs. 1 E / Makes berserk' -> '1.75 x DMG vs. 1 E / Makes berserk'.

200. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x1DAE0 (121568) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     FINAL HEX:  E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

201. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x1DB04 (121604) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     FINAL HEX:  E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

202. /CDROM/150_BPRG/BUFF0/BP0_SEC.BIN +0x1DB28 (121640) - Cup of the Oath coefficient instruction
     RETAIL HEX: C8000224
     FINAL HEX:  E1000224
     Meaning: Bandit Attack record ID 42, Cup of the Oath branch; instruction immediate 200% -> 225%.

203. /SLUS_009.58 +0x1E174 (123252) - Kindness signed-rating instruction
     RETAIL HEX: FFFF4332
     FINAL HEX:  21184002
     Meaning: Kindness Rune: remove the unsigned16-bit mask from the signed rating path; signed negative ratings retain their attack penalty. The no-penalty alternative is not used.

204. /CDROM/010_ARA/VA03.BIN +0x8E94 (36500) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

205. /CDROM/010_ARA/VA05.BIN +0xB904 (47364) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

206. /CDROM/010_ARA/VA06.BIN +0x9360 (37728) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

207. /CDROM/010_ARA/VA11.BIN +0x559C (21916) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

208. /CDROM/020_ARB/VB02.BIN +0x975C (38748) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

209. /CDROM/020_ARB/VB03.BIN +0x9DCC (40396) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

210. /CDROM/020_ARB/VB04.BIN +0xAE50 (44624) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

211. /CDROM/020_ARB/VB05.BIN +0xAB28 (43816) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

212. /CDROM/020_ARB/VB06.BIN +0x2938 (10552) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

213. /CDROM/020_ARB/VB11.BIN +0xA1A0 (41376) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

214. /CDROM/020_ARB/VB14.BIN +0x8E64 (36452) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

215. /CDROM/020_ARB/VB15.BIN +0x4AE8 (19176) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

216. /CDROM/020_ARB/VB18.BIN +0xA8BC (43196) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

217. /CDROM/020_ARB/VB19.BIN +0x748C (29836) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

218. /CDROM/020_ARB/VB21.BIN +0xE884 (59524) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

219. /CDROM/030_ARC/VC01.BIN +0x1111C (69916) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

220. /CDROM/030_ARC/VC03.BIN +0x27E0 (10208) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

221. /CDROM/030_ARC/VC06.BIN +0x6780 (26496) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

222. /CDROM/030_ARC/VC07.BIN +0xD0E0 (53472) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

223. /CDROM/030_ARC/VC10.BIN +0x6784 (26500) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

224. /CDROM/030_ARC/VC11.BIN +0x68A0 (26784) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

225. /CDROM/030_ARC/VC16.BIN +0x83D0 (33744) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

226. /CDROM/030_ARC/VC18.BIN +0x8224 (33316) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

227. /CDROM/030_ARC/VC21.BIN +0x170A0 (94368) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

228. /CDROM/030_ARC/VC22.BIN +0xB14 (2836) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

229. /CDROM/030_ARC/VC24.BIN +0xB3E0 (46048) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

230. /CDROM/030_ARC/VC25.BIN +0x1C14 (7188) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

231. /CDROM/030_ARC/VC27.BIN +0x3780 (14208) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

232. /CDROM/030_ARC/VC28.BIN +0xF7C8 (63432) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

233. /CDROM/030_ARC/VC30.BIN +0x8038 (32824) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

234. /CDROM/040_ARD/VD01.BIN +0xE9B8 (59832) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

235. /CDROM/040_ARD/VD03.BIN +0x6D98 (28056) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

236. /CDROM/040_ARD/VD17.BIN +0x82C8 (33480) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

237. /CDROM/040_ARD/VD19.BIN +0x610C (24844) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

238. /CDROM/050_ARE/VE01.BIN +0xED2C (60716) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

239. /CDROM/050_ARE/VE02.BIN +0x7B20 (31520) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

240. /CDROM/050_ARE/VE05.BIN +0x1A70 (6768) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

241. /CDROM/050_ARE/VE10.BIN +0x6D40 (27968) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

242. /CDROM/050_ARE/VE13.BIN +0xFF80 (65408) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

243. /CDROM/060_ARF/VF01.BIN +0x943C (37948) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

244. /CDROM/060_ARF/VF03.BIN +0x9F4C (40780) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

245. /CDROM/060_ARF/VF05.BIN +0xD008 (53256) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

246. /CDROM/070_ARG/VG03.BIN +0x76FC (30460) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

247. /CDROM/070_ARG/VG06.BIN +0x6704 (26372) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

248. /CDROM/070_ARG/VG07.BIN +0x8770 (34672) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

249. /CDROM/070_ARG/VG08.BIN +0x8C38 (35896) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

250. /CDROM/070_ARG/VG13.BIN +0xA7A8 (42920) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

251. /CDROM/070_ARG/VG18.BIN +0x9F4C (40780) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

252. /CDROM/080_ARH/VH01.BIN +0xA820 (43040) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

253. /CDROM/080_ARH/VH02.BIN +0x8B20 (35616) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

254. /CDROM/080_ARH/VH03.BIN +0xD224 (53796) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

255. /CDROM/080_ARH/VH05.BIN +0xABDC (43996) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

256. /CDROM/080_ARH/VH06.BIN +0x802C (32812) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

257. /CDROM/080_ARH/VH11.BIN +0xA2D8 (41688) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

258. /CDROM/080_ARH/VH12.BIN +0x5334 (21300) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

259. /CDROM/080_ARH/VH13.BIN +0x8250 (33360) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

260. /CDROM/080_ARH/VH14.BIN +0x8A58 (35416) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

261. /CDROM/080_ARH/VH16.BIN +0x707C (28796) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

262. /CDROM/080_ARH/VH17.BIN +0xA298 (41624) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

263. /CDROM/090_ARI/VI01.BIN +0xE558 (58712) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

264. /CDROM/090_ARI/VI02.BIN +0x9CD4 (40148) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

265. /CDROM/090_ARI/VI12.BIN +0x90E0 (37088) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

266. /CDROM/090_ARI/VI14.BIN +0x1F28 (7976) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

267. /CDROM/100_ARJ/VJ17.BIN +0x2D40 (11584) - NPC name spelling
     RETAIL HEX: 47152213151E112229104D1F1C19141522
     FINAL HEX:  47152213151E112229104D1F1C14191522
     Meaning: NPC label: 'Mercenary Solider' -> 'Mercenary Soldier'; equal length, exactly2 differing glyph bytes.

268. /CDROM/110_ARK/VK01.BIN +0x2098 (8344) - Headquarters world-map preload boundary
     RETAIL HEX: 013B6702889BFFFE
     FINAL HEX:  013B6702889DFFFE
     Meaning: Headquarters exit: extend the shared background world-map preload from inclusive Y155 to157, covering the two exit rows. This prevents the lower-wall route from using a cached bar with world-map texture geometry and corrupting live collision data. X bounds, neighboring preloads, destination, story flags and combat data remain unchanged.

269. /CDROM/110_ARK/VK34.BIN +0x2478 (9336) - Headquarters world-map preload boundary
     RETAIL HEX: 013B6702889BFFFE
     FINAL HEX:  013B6702889DFFFE
     Meaning: Headquarters exit: extend the shared background world-map preload from inclusive Y155 to157, covering the two exit rows. This prevents the lower-wall route from using a cached bar with world-map texture geometry and corrupting live collision data. X bounds, neighboring preloads, destination, story flags and combat data remain unchanged.

9. INTENTIONAL NON-CHANGES AND COVERAGE
Chuchara special J ranks and Tuta SPD remain retail. The conditional
Fury x Double-Strike cap is omitted: native Fury changes ATK before DEF,
and the tested optimized build retains its incoming Double-Strike cost.
No new balance coefficients beyond the prior 202-edit configuration
were added during Final verification. The 67 additional edits are the
signed-Kindness instruction, 64 spelling copies and two HQ preload spans.
Enemy/boss combat stats, EXP, economy and audio remain unchanged.
The HQ preload extent changes field routing readiness, preserving its
destination and story flags. NPC spelling resources are the documented
exception to an otherwise unchanged text scope.
A full campaign test was waived. Bounded native/save results and their
remaining limits are recorded in TEST_RESULTS.txt and KNOWN_ISSUES.txt.
Binary audit: reports/v100_final_text.json.
