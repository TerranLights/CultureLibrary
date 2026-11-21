STATUS: done 2026-11-21. Run agent's report; the sheets are unverified.

# Gan 赣: springboard run report (Sinian Federation member state, deeper brief)

**Result:** all 130 sheets are done, and every first line reads `STATUS: done 2026-11-21, not verified`. The run used 12 sign agents plus 1 relaunch, for Pisces after a usage-limit stop. The whole-nation QA (`springboard_qa.py Gan`) found **0 problems** in 130 sheets. No sheet needed a hand fix.

**Lands:** the sheets are written for Jiangxi 江西, the one province in the tracker header, as a working list the author still confirms. The note on lands appears once per sign, in the Domain sheet (12 files), and nowhere else. No sheet tells the reader to read a scope file. No unit list was added, and nothing was taken from or cited to Hermes_research.

## Tokens and wall-clock
- **Sub-agent tokens:** **2,265,375**. This is the sum of the 12 sign agents' reported usage, the Pisces relaunch included. The first Pisces agent was stopped by the 5-hour usage limit, and its usage was not reported, so it is not in this sum. It wrote no sheet. The run agent's own tokens are not included either; the main session adds them.
- **Tool uses:** 425 across the agents that reported.
- **Wall-clock:** the run agent started at **08:02:16 MST**. Aries launched at 08:03, and Aquarius finished at 10:26. The first Pisces agent launched at about 10:27 and stopped at about 10:35.
- **Interruption:** the run paused from **about 10:35 to 11:43** because of the usage limit. The Pisces relaunch ran from 11:42 to 11:56. The report was finished at **about 11:58 MST**.
- **Time:** about 3 h 56 min elapsed, or about 2 h 48 min of working time without the pause. Each sign took 10.2 to 14.6 min.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,135 | 1,241 (Domain) | 14.5 (14-15) | 164,904 | 08:03-08:16 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,151 | 1,282 (Domain) | 14.3 (13-15) | 195,464 | 08:16-08:31 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,154 | 1,212 (Domain) | 14.6 (14-15) | 170,906 | 08:31-08:41 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,133 | 1,283 (Domain) | 14.2 (14-16) | 186,085 | 08:42-08:54 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,094 | 1,227 (Domain) | 14.0 (14) | 191,033 | 08:54-09:08 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,189 | 1,265 (Domain) | 13.9 (13-14) | 187,363 | 09:08-09:20 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,188 | 1,266 (Domain) | 13.9 (13-15) | 194,292 | 09:21-09:33 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,189 | 1,255 (Death) | 14.4 (14-15) | 190,667 | 09:34-09:47 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,146 | 1,219 (Faith) | 14.4 (13-15) | 199,778 | 09:48-10:01 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,162 | 1,267 (Domain) | 15.0 (14-16) | 188,352 | 10:02-10:14 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,177 | 1,250 (Domain) | 14.7 (14-16) | 191,076 | 10:15-10:26 |
| 12 | Pisces | 12/12 | 2 | 1 (usage-limit stop) | 0 | 1,125 | 1,267 (Domain) | 14.3 (13-16) | 205,455 (+ unreported) | 11:42-11:56 |
| | **Total** | **130** | **13** | **1** | **0** | **1,152** | **1,283** | **14.3 (13-16)** | **2,265,375** | |

- **Word counts:** by `wc -w`, markup included; 149,764 words in all. The shortest sheet is Leo/Play at 1,018 words, and the longest is Cancer/Domain at 1,283. No sheet is over the 1,300 flag.
- **Pointers:** the rows of section 2, 1,863 in all. Seven sheets have 13 pointers, 77 have 14, 42 have 15 and 4 have 16.

## Rule breaks and fixes
- **QA:** nothing was flagged in any sign or in the whole-nation scan.
  - No zodiac, divination-label or horoscope words.
  - No "Indian".
  - No South Asian items. The Held-for-review line reads "none" on all 130 sheets. Four of them add a pointer that sends law questions on to Libra or Capricorn.
  - No "sikh"-pattern false positives.
- **Law:** the law material is in Libra (the letter of the law) and Capricorn (the spirit). Sheets in the other signs pass law questions to those signs. For example, Gemini/Mediation keeps village mediation committees to practice only.
- **Interruption:** the Pisces folder was empty when the run resumed, so the relaunch wrote all 12 sheets from scratch. No half-written sheet had to be completed.
- **Run log:** I appended one line per sign and a completion line. The completion line gave the average pointer count as 14.4 instead of 14.3, so a correction line was appended after it. Nothing was rewritten.

## Repetition
- **Lines:** no line of more than 40 characters repeats across the 130 sheets, apart from the template's three fixed lines. That includes the "Who to compare" bullets. There is one exception: a short, generic Flags line ("Languages needed: Standard and Classical Chinese; Gan and Hakka for oral accounts.") appears in both Cancer/Abandonment and Virgo/Service. Different agents wrote those sheets, and the line was left as is.
- **Most-reused sources** (sheets out of 130):
  - Ouyang Xiu 欧阳修: 14.
  - Wang Yangming 王阳明: 13, with his 南赣乡约 in 12.
  - The Jiangxi Statistical Yearbook 江西统计年鉴: 13.
  - The Jiangyou merchant guilds 江右商帮: 12.
  - Wang Anshi, Tao Yuanming, Wen Tianxiang, Tang Xianzu, Longhushan 龙虎山, and Elizabeth Perry's *Anyuan*: 11 each.
  - The Jiangxi TV mediation program 金牌调解: 11. It is the nearest thing to a default media pointer.
  - Hymes, *Statesmen and Gentlemen* (Fuzhou elites): 9.

  The "江西卷" volumes (22 hits) are spread across several different series: folk tales, proverbs, songs and opera records. Each reuse is tied to a reason specific to its concept, but Wang Yangming's compact and the mediation program are close to default pointers.

## Thin, repetitive or generic sheets
- **Gemini is the most query-heavy sign.** Its pointers are mostly a topic plus a search query rather than a named source:
  - Mediation: 12 of 14.
  - Information: 10.
  - Gossip: 10.
  - Connection: 9.
  - Siblings: 9.
  - Learning: 8.
  - Communication and Duality: 6 each.
  - Curiosity: 5.

  This is allowed by the brief ("give the type of source and the query"), and the queries are concrete Chinese search strings. Even so, these sheets give the later research fewer named starting points than the other signs. They are the first candidates for a deeper second pass.
- **Elsewhere,** no sheet has more than 3 query-only rows (Cancer/Nurture, Pisces/Self-sacrifice and Pisces/Dissolution have 3).
- **No sheet reads as thin or generic** on a spot-check (Aries/Identity, Gemini/Mediation). The shortest sheets are Leo/Play (1,018), Aries/Competition (1,053) and Leo/Dignity (1,055), and all are still full-length.

## Whether the sheets exploit the nation's depth
- **Peoples and dialect areas** (sheets out of 130 that mention each):
  - Hakka and She: 130 each.
  - Gannan/Ganzhou: 129.
  - Huizhou-speaking Wuyuan: 106.
  - Ji'an/Luling: 98.
  - Jingdezhen: 85.
  - Gan-language terms or dialect forms: 81.
  - Poyang Lake: 78.
  - The Wu-speaking Shangrao area: 74.
  - Mandarin-speaking Jiujiang: 66.
  - Fuzhou/Linchuan: 55.
  - Pingxiang, the Xiang-speaking border: 44.
  - Lushan: 46.
  - Longhushan and the Celestial Masters: 34.
  - Jinggangshan: 29.

  Coverage is broad and goes well beyond the best-known two or three.
- **Pre-modern pointers:** every sheet has at least one. Examples are Song-Ming Jiangxi literati (Ouyang Xiu, Wang Anshi, Zhu Xi at the White Deer Grotto, Lu Jiuyuan, Wen Tianxiang, Tang Xianzu, Song Yingxing), Ming-Qing gazetteers, Huizhou documents and the Baizhang monastic code.
- **Native script:** Chinese characters are used throughout, with Gan, Hakka and She terms marked *check*.
- **Weak spots:**
  1. Hui Muslims in Jiangxi appear in only 4 sheets, and the Poyang Lake fishing and boat communities appear as a group in only 1. This is small, but they are the gaps.
  2. She terms are mostly given in Chinese. The She language, a Hakka-like variety, has few sure forms, which is right to leave marked *check*.
  3. Diaspora pointers are kept as comparison only.
