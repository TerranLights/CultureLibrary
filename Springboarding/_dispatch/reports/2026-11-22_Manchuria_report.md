# Manchuria springboard run: report (2026-11-22)

**Run agent:** one per nation, deeper brief (Priority block, binding own-terms rule). **Wall clock:** 05:03 to 07:55 MST (2 h 52 min), no usage-limit stop. **Sheets:** 130/130 `STATUS: done 2026-11-22, not verified`. **Sub-agents:** 12 (one per sign), 0 relaunches. **Sub-agent tokens:** 2,326,559 in all (about 194,000 per sign). **Whole-nation QA:** 130 sheets scanned, 0 problems.

**Lands:** the tracker header lists no settled lands and there is no `00 - Scope.md`. The sheets follow the brief's missing-scope rule. Each sign's Domain sheet says once that the exact lands are still to be settled, and the rest is written for the core lands of the old Northeast (the three northeastern provinces and the eastern Inner Mongolian leagues). No unit list was added. Manchuria is written as its own culture-nation, not as part of the Sinian Federation. Nothing was taken from `Hermes_research`.

## Per sign
| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers | Sub-agent tokens | Time | Notes |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,078 | 1,272 (Domain) | 967 (Recklessness) | 14-16 | 173,650 | 05:04-05:19 | leanest sign |
| 2 | Taurus | 11 | 1,195 | 1,242 (Domain, Possession) | 1,133 (Possessiveness) | 13-15 | 197,764 | 05:19-05:34 | |
| 3 | Gemini | 10 | 1,175 | 1,277 (Domain) | 1,094 (Gossip) | 14-15 | 176,720 | 05:34-05:46 | separateness from the Sinian Federation restated in every Target line (varied wording) |
| 4 | Cancer | 10 | 1,190 | 1,280 (Domain) | 1,082 (Nurture) | 14-15 | 194,016 | 05:46-06:00 | |
| 5 | Leo | 13 | 1,071 | 1,164 (Domain) | 1,001 (Play) | 13-16 | 202,746 | 06:00-06:15 | sub-agent rewrote one shared line itself |
| 6 | Virgo | 10 | 1,147 | 1,275 (Domain) | 1,053 (Criticism) | 14 | 197,574 | 06:15-06:29 | |
| 7 | Libra | 11 | 1,163 | 1,280 (Domain) | 1,119 (Partnership) | 14 | 207,911 | 06:30-06:44 | law kept to the letter |
| 8 | Scorpio | 11 | 1,086 | 1,240 (Domain) | 1,014 (Trust) | 14-16 | 193,815 | 06:44-06:58 | Domain edited after its done line (file complete) |
| 9 | Sagittarius | 11 | 1,119 | 1,255 (Domain) | 1,044 (Conviction) | 13-15 | 188,119 | 06:58-07:12 | 1 hand fix (below); Held line used by category |
| 10 | Capricorn | 10 | 1,211 | 1,268 (Domain) | 1,142 (Merit) | 14-15 | 195,224 | 07:12-07:26 | Law sheet written for the spirit of law |
| 11 | Aquarius | 10 | 1,146 | 1,290 (Domain) | 1,094 (Friendship) | 14-15 | 201,444 | 07:26-07:40 | |
| 12 | Pisces | 12 | 1,118 | 1,278 (Domain) | 1,065 (Intuition) | 13-15 | 197,576 | 07:40-07:54 | Held line used by category (Boundary) |

**Nation:** average 1,139 words by `wc -w` (967 to 1,290; 24 sheets over 1,200, none over 1,300). Pointers per sheet: 13 to 16, average 14.3 (7 sheets have 13, 85 have 14, 34 have 15, 4 have 16).

## Rule breaks and fixes
- **QA scan:** 0 problems in every sign and for the whole nation. No zodiac words, no "Indian", no South Asian words outside the Held line, no URLs, no finding phrases, no universals list. The known "sikh" false positive (Sikhote-Alin) did not come up.
- **Repeat check (my own, across all 130 sheets):** no repeated line, table row, "What it would give" cell or "Who to compare" reason. The template's "Held for review: none" line is excluded from the check. One flag line did repeat across signs: the bare "Languages needed" list was the same in Leo/04 Recognition and Sagittarius/09 Education. **Fix:** I rewrote it by hand in Education as a concept-specific line (a one-line edit; the status line was kept). From Capricorn on, the sub-agent prompt asked for concept-specific "Languages needed" lines.
- **Sinian Federation hedge:** Gemini's ten sheets each restated in the Target line that Manchuria is separate from the Sinian Federation (worded differently each time; not wrong, but repetitive). From Sagittarius on, the prompt limited this to the Domain sheet. The earlier lines were left as written.
- **Status line not the last write:** Scorpio/00 Domain, Sagittarius/04 Truth and Sagittarius/07 Travel were each edited slightly after being marked done. The changes were a cut Sinian Federation mention and two un-matched "Languages needed" lines. All three files are complete.
- **Held for review (category only):** Sagittarius/00 Domain (two English-language studies of Manchukuo-era religion and borderland politics) and Pisces/05 Boundary (one standard study of Manchukuo's sovereignty and borders). Both were set aside under the South Asian-scholar rule. The author may want to look at them, since the Boundary one is central to that concept.
- **Law:** Libra was written for the letter of the law and Capricorn's Law sheet for its spirit. Pisces/10 Crime keeps to bandit lore, exile writing and fiction, with no law pointers.

## Thin, repetitive or generic sheets
- **Leaner:** Aries (avg 1,078) and Leo (avg 1,071). The shortest sheets are Aries/10 Recklessness (967), Aries/09 Competition (998), Leo/10 Play (1,001) and Scorpio/06 to 10 (Trust, Revenge, Secrecy, Power, Crisis, all about 1,014 to 1,041). None is thin in substance: each has 13 to 15 pointers.
- **Pre-modern coverage weakest:** Scorpio/03 Purging, which is almost all twentieth-century. Its only older material is Khorchin shamanic healing and folk-calendar compilations. Scorpio/01 Death and Pisces/09 Intuition rely on shamanic song manuscripts, *Zhou Gong's Dream Book* and ginseng-digger cult lore rather than a dated classical text. Every other sheet has a Qing or earlier pointer (117 of 130 name Qing sources).
- **Most reused sources** (allowed, but they recur): Ching Kwan Lee, *Against the Law*, and Elliott, *The Manchu Way* (8 sheets each); Gottschang and Lary, *Swallows and Settlers*, and Kang, *The Cult of the Fox* (7 each); Park, Billingsley and Hurst (6 each). No sign leans on the same few sources throughout.

## Does it exploit the nation's depth?
Mostly yes.
- **Peoples and languages:** Korean-language terms in hangul appear in all 130 sheets, Cyrillic in 115, Manchu terms in all 130, and Mongol material in all 130. The Tungusic peoples are well covered: Oroqen in 106 sheets, Evenki in 98, Hezhe/Nanai in 94 and Daur in 60.
- **Places:** the city spread is broad (Harbin 106, Shenyang 108, Jilin 82, Changchun and Dalian 55 each). Hulunbuir and Barga appear in 60 sheets. The rust-belt layoff era appears in 42 and Manchukuo in 58.
- **Pre-modern:** Jurchen, Bohai and Goguryeo layers appear in 28 sheets and the Chuang Guandong migration in 21.

**Gaps for the research stage:**
- Manchu traditional script appears in only 18 sheets (most Manchu terms are romanized only), and Japanese kana in 8.
- Xibe appear in 21 sheets and Hui in 45. The Fuyu Kyrgyz are nearly absent (2), and the Russian-descended people of Ergun are thin (31).
- Smaller cities are rare: Yingkou 2, Tongjiang and Fuyuan 5, Mudanjiang 6, Manzhouli 7, Dandong 16, Qiqihar 16. Daqing appears in 23.
- Japanese left-behind settlers and orphans appear in 11 sheets, and yangge folk dance in 5.

Diasporas appear only as comparison bullets.
