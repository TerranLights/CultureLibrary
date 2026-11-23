STATUS: done 2026-11-22. Run agent's report; the sheets are unverified.

# Hakka 客家: springboard run report (non-territorial Sinian Federation sub-unit, deeper brief)

**Result:** all 130 sheets are done. Every first line reads `STATUS: done 2026-11-22, not verified`. The run used 12 sign agents, one per sign, with no relaunches. The whole-nation QA (`springboard_qa.py Hakka`) found **0 problems** in 130 sheets. My own repeat check found 3 copied lines and 2 stock bullets, all fixed by small edits (see below).

**Lands:** Hakka is non-territorial, so each sub-agent prompt carried the tracker header's framing. The sheets are written for the Hakka people and their communities: the language and its dialects, customs, lineages, migration history, and the contrast with Cantonese, Hokkien, Teochew, Gan and She neighbors. They cover the heartland (Meizhou, western Fujian around Longyan and Yongding, southern Jiangxi around Ganzhou), plus Guangxi, Sichuan, Hunan, Hainan and Hong Kong's New Territories. Taiwan's Hakka and the overseas diaspora appear only as comparison.
- **Working-list note:** each sign has exactly one note that the community list is a working list for the author to confirm, always in its Domain sheet (12 files) and never in a concept sheet.
- **Scope-file mentions:** two Domain sheets (Taurus, Capricorn) say that no scope file exists. Neither tells the reader to read or check one, so both were kept.
- **Other limits:** no unit list was added, and nothing was taken from or cited to Hermes_research.

## Tokens and wall-clock
- **Sub-agent tokens:** **2,268,380** in all, across 460 tool uses. This is the sum of the 12 sign agents' reported usage. The run agent's own tokens are not included; the main session adds them.
- **Wall-clock:** the run agent started at **05:03:30 MST**. Aries launched at 05:04 and Pisces finished at 07:47. The report was finished at **about 07:50 MST**.
- **Time:** about 2 h 47 min in all, with no interruption and no usage-limit stop. Each sign took 11.6 to 15.1 min.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,074 | 1,261 (Domain) | 15.7 (15-16) | 156,530 | 05:04-05:16 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,213 | 1,291 (Domain) | 14.0 (14) | 195,108 | 05:16-05:30 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,192 | 1,250 (Domain) | 15.7 (15-16) | 176,928 | 05:31-05:43 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,198 | 1,255 (Domain) | 13.4 (13-14) | 194,441 | 05:43-05:56 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,061 | 1,199 (Domain) | 14.4 (14-16) | 182,202 | 05:56-06:09 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,178 | 1,272 (Domain) | 14.1 (14-15) | 185,082 | 06:09-06:21 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,183 | 1,295 (Domain) | 14.1 (12-15) | 197,689 | 06:22-06:35 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,208 | 1,276 (Death) | 13.9 (13-14) | 196,996 | 06:35-06:49 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,172 | 1,264 (Faith) | 14.4 (14-15) | 188,898 | 06:50-07:04 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,124 | 1,253 (Domain) | 14.1 (13-16) | 193,343 | 07:04-07:18 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,176 | 1,268 (Community) | 14.6 (13-16) | 197,722 | 07:18-07:32 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,178 | 1,272 (Domain) | 14.1 (14-15) | 203,441 | 07:32-07:47 |
| | **Total** | **130** | **12** | **0** | **0** | **1,161** | **1,295** | **14.4 (12-16)** | **2,268,380** | |

- **Word counts:** by `wc -w`, markup included, after the fixes; 150,974 words in all. The shortest sheet is Leo/Leadership at 988 words, and the longest is Libra/Domain at 1,295. No sheet is over the 1,300 flag. Three sub-agents trimmed a sheet that first came in over 1,300 (Virgo/Domain; Scorpio/Domain and Death), setting it back to in progress before marking it done again.
- **Pointers:** the rows of section 2, 1,868 in all. One sheet has 12 pointers (Libra/Indecision), 11 have 13, 76 have 14, 23 have 15 and 19 have 16. All are within the 12 to 16 range.

## Rule breaks and fixes
- **QA:** nothing was flagged in any sign or in the whole-nation scan.
  - No zodiac, divination-label or horoscope words.
  - No "Indian".
  - No South Asian items, and no "sikh"- or "hindi"-pattern false positives.
  - No findings phrases.
- **Universals:** no sheet mentions universals, Human Universals or Brown.
- **Law:** law material stays in Libra (the letter of the law) and Capricorn (the spirit).
- **Fixes from my repeat check:** all five were small edits by the run agent, logged in the Run log.
  - **Aries:** two short "Languages needed" Flags lines each appeared word for word in two sheets: Initiative and Recklessness, and Courage and Competition. I gave Recklessness and Competition a reason tied to their own concept.
  - **Virgo:** the Domain sheet's last "Who to compare" bullet ("Taiwan's Hakka and the overseas diaspora: comparison only.") copied the Gemini Domain sheet's word for word. I gave it a work-specific reason.
  - **Scorpio:** the bare bullet "Comparison only: Taiwan's Hakka and the overseas diaspora." appeared in both the Scorpio and the Aries Domain sheets. I gave each a reason tied to its sign: identity and self-naming for Aries, reburial and ancestral rites for Scorpio.
  - **Prompt change:** from Libra on, the sub-agent prompt also said that the Taiwan-and-diaspora bullet must carry a reason tied to the sheet's concept. No repeat came up after that.
- **Kept as published:** Libra/Peace at any price names the "Universities Service Centre for China Studies" (CUHK). It is the institution's own name, so its British spelling stays.
- **Run log:** one line per sign, plus one appended correction for Virgo, whose Domain word count changed after my fix (1,272, not 1,269). Nothing was rewritten.

## Repetition (my nation-wide check)
- **Lines:** after the fixes, no line of more than 40 characters repeats across the 130 sheets, apart from the template's three fixed lines. That covers table rows, "Who to compare" bullets, Flags lines and first-query lines, all compared after normalizing case and punctuation.
- **Most-reused sources:** sheets that mention each, anywhere in the sheet.
  - Basel Mission archives and romanized publications: 35. This is the nearest thing to a default pointer, though it is used for different questions: names, hymns, schooling and church records.
  - Nicole Constable (*Christian Souls and Chinese Spirits*, *Guest People*): 21.
  - Luo Xianglin 羅香林 (*客家研究導論*): 21.
  - Ellen Oxfeld (*Drink Water, but Remember the Source*; *Bitter and Sweet*): 19.
  - CFPS: 17.
  - "Guest People" (the title): 15.
  - CGSS: 14.
  - Sow-Theng Leong: 13.
  - Myron Cohen: 13.
  - The China Hakka Museum, Meizhou: 13.
  - Mary Erbaugh: 11.
  - Xu Xuzeng 徐旭曾, *豐湖雜記* (1808): 10.
  - Hong Xiuquan and Taiping material: 10.

  Each reuse is tied to a reason specific to its concept. Even so, the small English-language Hakka canon (Constable, Oxfeld, Leong, Cohen, Erbaugh) recurs more than a nation with a larger literature would need.
- **Recurring heritage forms:** tulou 土樓 (64 sheets), mountain songs 山歌 (43) and genealogies 族譜 (25) run through the sign sets as recurring heritage forms.

## Thin, repetitive or generic sheets
- **Leo is the lightest sign** (average 1,061 words).
  - **Play** and **Joy** lean on heritage-listed festivals and dances plus "search X" queries. They have few named scholarly works and no clearly pre-modern text pointer: the festivals are old, but no early source is named.
  - **Leadership** (988 words, the shortest sheet) leans on revolutionary-era memorial sites and biographies. Its pre-modern side is only genealogy officer titles.
- **Libra/Reciprocity** names no dated pre-modern source. Its old material comes through gift books, lineage charity fields (義田) and rites. It also uses two national panels (CFPS, CHARLS) and a northern-village gift ethnography (Yan) as comparison.
- **Libra/Indecision** is the only sheet with 12 pointers.
- **Capricorn/Hierarchy** names the fewest communities (4 of the listed areas); the rest of its pointers are general.
- **Surveys:** national surveys (CFPS, CGSS, CHARLS) recur as "filter to Hakka-majority prefectures" proxies. That is honest, since mainland surveys do not record Hakka identity, but it makes the survey rows of many sheets alike in kind.

## Do the sheets exploit the culture's depth?
Largely yes.
- **Language terms:** every sheet has Hakka-language terms in section 1, some with Pha̍k-fa-sṳ or other romanization marked *check* (14 sheets name romanized Hakka), beside Standard Chinese and often Cantonese.
- **Pre-modern sources:** Xu Xuzeng's 1808 notes, Qing gazetteers and genealogies, Taiping-era sources and Hamberg (1854) supply pre-modern pointers in nearly every sheet.
- **Communities:** they reach well past Meizhou and Yongding: Gannan counties (Ningdu, Xingguo, Yudu, Ruijin), western Fujian (Changting, Shanghang, Liancheng, Ninghua), Huizhou and Heyuan, Shaoguan, Guangxi (Bobai, Luchuan, Hezhou), Sichuan (Luodai, the Dongshan area of Chengdu), Hainan and the New Territories. The She 畲 appear as a distinct neighboring people, not merged with the Hakka.
- **Sensitive topics:** the sheets flag contested origin narratives (northern descent against southern fusion), the Punti-Hakka feuds and dialect decline. They read Hakka heritage-promotion writing as promotion, not description.
- **Main limit:** the small English-language canon noted above. Later research should widen the Chinese-language county and lineage literature, which the sheets mostly reach through search queries rather than named works.
