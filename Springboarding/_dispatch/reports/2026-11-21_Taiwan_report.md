# Taiwan springboard run: report (2026-11-21)

Run agent for Taiwan, deeper brief (accuracy and depth first), one sub-agent per sign, Aries to Pisces. Sheets are in `Targets/Asia/East Asia/Taiwan/Springboards/`. None of them has been verified.

## Summary
- **Sheets:** 130 of 130 marked `STATUS: done 2026-11-21, not verified`.
- **Agents:** 12 sign agents plus 1 relaunch (Aquarius, after the usage-limit cutoff). No QA-driven relaunches.
- **QA:** `springboard_qa.py Taiwan` gives 130 sheets scanned, 0 problems. I made no hand edits.
- **Total sub-agent tokens:** about **2,350,500**. That is the sum of every sign agent and the relaunch. One figure is an estimate: the Aquarius agent that was cut off reported no usage, so its 167,500 is read from its transcript.
- **Wall-clock:** run agent started **08:02** and ended **12:04 MST**. Inside that window the 5-hour usage limit stopped the run from **about 10:35 to 11:43** (see Aquarius). Sub-agents were working for about 3 h 0 min in total.
- **Lands:** the tracker header lists no settled territory ("to be settled by the author in Stage 0"), and `00 - Scope.md` does not exist. The sheets follow the brief's missing-scope rule. Each sign's Domain sheet carries the lands note once, and no unit list was added. Nothing was taken from Hermes_research.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words (wc -w) | Longest | Shortest | Pointers | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,137 | 1,251 (Domain) | 1,103 | 16-17 | 179,418 | 08:03-08:18 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,133 | 1,264 (Domain) | 1,073 | 16-17 | 184,099 | 08:18-08:32 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,188 | 1,265 (Domain) | 1,056 | 16-17 | 178,422 | 08:32-08:44 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,103 | 1,222 (Domain) | 1,056 | 15-16 | 178,363 | 08:45-08:55 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,065 | 1,210 (Domain) | 974 (Play) | 14-16 | 208,890 | 08:56-09:12 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,170 | 1,273 (Domain) | 1,093 | 16-17 | 186,562 | 09:12-09:25 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,148 | 1,260 (Domain) | 1,107 | 16 | 205,806 | 09:25-09:40 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,167 | 1,266 (Domain) | 1,105 | 15-16 | 186,017 | 09:40-09:53 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,160 | 1,282 (Domain) | 1,096 | 16-17 | 189,182 | 09:53-10:07 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,217 | 1,274 (Domain) | 1,136 | 15-17 | 181,170 | 10:07-10:19 |
| 11 | Aquarius | 10/10 | 2 | 1 (cutoff) | 0 | 1,125 | 1,272 (Detachment) | 980 (Friendship) | 16-17 | about 273,000 (about 167,500 + 105,519) | 10:19-10:29, 11:43-11:46 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,171 | 1,246 (Domain) | 1,109 | 16-18 | 199,576 | 11:47-12:01 |
| | **Nation** | **130/130** | **13** | **1** | **0** | **1,147** | 1,282 | 974 | avg 16.2 | **about 2,350,500** | 08:02-12:04 |

Pointer counts are the rows in each sheet's "Where to look first" table. Across the nation: one sheet has 14, 13 have 15, 81 have 16, 34 have 17 and one has 18. Twenty-five sheets run over 1,200 words and none over 1,300.

## Interruption (Aquarius)
- The Aquarius sign agent hit the 5-hour usage limit at about 10:29 to 10:35 and stopped. By then 00 to 07 were done and `08 - Detachment.md` was half-written (`STATUS: in progress`).
- After the reset, I relaunched at 11:43 for concepts 8 and 9 only, per the coordinator's instruction. The relaunch was allowed to read 00 to 07 so it would not repeat them, but not to edit them. It rewrote Detachment from scratch and wrote Hope new.
- The cut-off agent reported no usage, so its token figure comes from its transcript (the context size of its last message).

## Rule breaks and fixes
- **No QA problems and no hand edits.**
- **Cancer, `01 - Home.md`:** the sub-agent spelled the place name 新店 as "Hsin-tien" (Wade-Giles) instead of "Xindian", to keep it away from the "Indian" scan. This was not needed, because the scan matches whole words only. The spelling is valid and was left as written.
- **Capricorn, Domain and `09 - Order.md`:** the sub-agent made a small wording fix to the diaspora bullet after it had set the done line. I checked both files: they are complete, and the bullets read as comparison only.
- **No zodiac words, no South Asian words, no URLs, no "Indian" and no finding phrases** in any sheet. No "sikh"-pattern false positives came up.

## Repetition
- Within each sign, no line over 40 characters is shared between sheets beyond the template's own three lines.
- Across the whole nation, one line repeats. It is the Flags line "Languages needed: Mandarin, Hokkien, Hakka, Japanese, classical Chinese, Indigenous ...", which appears in Gemini `02 - Information`/`03 - Learning` and in Pisces `10 - Crime`. It is a flags line, not a pointer or a compare bullet. It is not worth a relaunch.
- **Recurring sources** are spread thinly. Across the 130 sheets, Academia Sinica appears in 46, PTS/TITV in 51, the Taiwan Social Change Survey in 22 and TEDS in 7. No single source fills a sign.

## Thin, repetitive or generic sheets (by name)
- **Shortest sheets,** all still full and specific:
  - Leo: `10 - Play` (974 words), `09 - Leadership` (990), `12 - Joy` (1,002), `11 - Honor` (1,012), `07 - Humiliation` (1,041).
  - Aquarius: `06 - Friendship` (980), `07 - Nonconformity` (1,042).
  - Leo is the sign that comes out lightest (13 concepts, avg 1,065). On a spot check, `Play` is concrete rather than generic: the Yilan children's folkgame festival, Shih Fu-chen and Chien Shang-jen's song collections, the 民俗臺灣 folklore journal, claw-machine shops, the National Indigenous Peoples' Games, 電音三太子.
- **Weak spot: Indigenous-language search terms.** 29 of 130 sheets have no Indigenous-language row in their search-terms table, though most still give Indigenous pointers in sections 2 and 3. They cluster in psychological and abstract concepts:
  - Aries: Anger, Competition, Recklessness.
  - Taurus: Security, Possessiveness.
  - Gemini: Duality, Gossip.
  - Cancer: Care, Abandonment.
  - Leo: Recognition, Humiliation, Play.
  - Virgo: Usefulness, Analysis, Perfectionism, Criticism, Improvement.
  - Libra: Impartiality.
  - Scorpio: Control, Revenge, Secrecy, Crisis.
  - Capricorn: Ambition.
  - Aquarius: Reform, Friendship, Nonconformity.
  - Pisces: Empathy, Dissolution, Escapism.

  These were not relaunched (they are not QA flags). The later research should add Amis, Atayal, Paiwan, Bunun and Tao terms for them from the Council of Indigenous Peoples' online dictionaries.
- No sheet reads as generic boilerplate on the spot checks (Aries Identity, Leo Play).

## Do the sheets exploit the nation's depth?
Largely yes. Counts below are sheets out of 130 that mention each item.
- **Languages:**
  - Every sheet gives Mandarin in traditional characters, Taiwanese Hokkien (Taigi, usually with Tâi-lô romanization) and Hakka.
  - Japanese colonial-era terms appear where they are relevant.
- **Indigenous peoples:**
  - The big peoples appear widely: Amis/Pangcah 90, Tao/Yami 99, Paiwan 87, Atayal 83, Bunun 66, Truku/Seediq 65, Rukai 56.
  - The smaller recognized peoples appear less often: Puyuma 37, Tsou 31, Saisiyat 21, Kavalan 20, Thao 12, Sakizaya 8, Hla'alua/Kanakanavu 8.
  - The Pingpu peoples (Siraya, Makatao, Taivoan, Pazeh, Kaxabu) appear in 39.
- **Other groups:**
  - Post-1949 mainlander families and military villages (外省, 眷村): 34.
  - New immigrants and migrant workers: 86 (with Vietnamese, Indonesian or Filipino named in 36).
  - Diaspora appears as comparison only.
- **Regions:**
  - Outlying islands: Kinmen 47, Matsu 43, Penghu 36, Lanyu/Orchid Island 57.
  - Hakka areas: Hsinchu/Miaoli/Taoyuan 64, Pingtung/Liudui 41.
  - Tainan 58.
  - The east coast is mentioned less often than its Indigenous weight would suggest (Hualien/Taitung by name 31, Yilan 9).
- **Pre-modern pointers:**
  - Dutch-era and Formosan-language material 83.
  - Japanese colonial customs and ethnographic surveys 89.
  - Classical Chinese texts 73.
  - Qing local gazetteers (府志, 縣志) 29.
- **Gaps for the later research:**
  - The Indigenous search terms in abstract concepts (above).
  - The smaller peoples and Yilan and the east coast are named less often.
  - Japanese kana appears in only 6 sheets; colonial terms are mostly given in kanji.

## Files touched
- Only `Targets/Asia/East Asia/Taiwan/Springboards/` (12 sign folders, 130 sheets).
- Thirteen lines appended with `>>` to the Run log in `_dispatch/SPRINGBOARD_PROGRESS.md`. The first line was not edited and nothing was rewritten in place.
- This report.
