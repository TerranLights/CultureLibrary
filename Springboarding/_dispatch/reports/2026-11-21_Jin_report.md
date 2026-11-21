STATUS: done 2026-11-21. Run agent's report; the sheets are unverified.

# Jin 晋: springboard run report (Sinian Federation member state, deeper brief)

**Result:** all 130 sheets are done. Every first line reads `STATUS: done 2026-11-21, not verified`. The run used 12 sub-agents (one per sign) and needed 0 relaunches. The whole-nation QA (`springboard_qa.py Jin`) found **0 problems** in 130 sheets, and no sheet needed a hand fix.

**Tokens and wall-clock:**
- **Sub-agent tokens:** **2,262,492**, the sum of the 12 sign agents' hand-back usage. There were no relaunches. The run agent's own tokens are not included; the main session adds them.
- **Tool uses:** 463 across the 12 sub-agents.
- **Wall-clock:** the run agent started at **05:03:46 MST**. The Aries agent launched at 05:04:51, and the Pisces agent finished at 07:45:28. The report was written by **07:47 MST**, for a total of about 2 h 43 min.
- **Time per sign:** 11.5 to 16.2 min. Signs ran one after another.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,122 | 1,284 (Domain) | 14.6 (14-15) | 156,234 | 05:05-05:17 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,164 | 1,245 (Possession) | 14.7 (14-15) | 189,684 | 05:17-05:31 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,209 | 1,290 (Domain) | 14.2 (14-16) | 178,834 | 05:31-05:43 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,192 | 1,267 (Home) | 14.3 (14-15) | 185,010 | 05:43-05:54 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,124 | 1,271 (Domain) | 13.7 (13-15) | 205,920 | 05:55-06:11 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,188 | 1,267 (Service) | 14.3 (14-15) | 190,292 | 06:11-06:24 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,127 | 1,224 (Domain) | 15.4 (14-16) | 203,881 | 06:24-06:39 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,108 | 1,256 (Domain) | 14.3 (13-16) | 195,591 | 06:40-06:54 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,100 | 1,211 (Domain) | 14.0 (13-15) | 190,634 | 06:54-07:07 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,123 | 1,216 (Domain) | 13.4 (13-14) | 184,657 | 07:07-07:19 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,164 | 1,211 (Domain) | 14.5 (14-15) | 194,620 | 07:20-07:33 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,103 | 1,210 (Domain) | 14.0 (14) | 187,135 | 07:33-07:45 |
| | **Total** | **130** | **12** | **0** | **0** | **1,142** | **1,290** | **14.3 (13-16)** | **2,262,492** | **05:05-07:45** |

- **Word counts:** by `wc -w`, markup included. The shortest sheet is Sagittarius/Honesty at 993 words, and the longest is Gemini/Domain at 1,290. No sheet is over the 1,300 flag. Twenty-six sheets are between 1,200 and 1,290 words (eleven of the twelve Domain sheets among them); this is within the brief's "a little over is fine".
- **Pointers:** the rows of section 2, 1,856 in all. Every sheet is within 13 to 16.

## Rule breaks and fixes
- **QA:** nothing was flagged in any sign or in the whole-nation scan.
  - No zodiac, divination-label or horoscope words.
  - No "Indian".
  - No South Asian items. The Held-for-review line reads "none" on all 130 sheets.
  - No "sikh"-pattern false positives.
  - No mention of Hermes_research.
- **Lands note:** written once in each sign's Domain sheet, and nowhere else. It says that the lands are Shanxi, as a working list the author still confirms. No sheet tells the reader to read a scope file. No unit list was added beyond the tracker header, and nothing was taken from Hermes_research.
- **Law:** the law material is in Libra (the letter of the law) and Capricorn (the spirit). The sheets in the other signs send law questions on to those two signs.
- **One correction to the Run log:** in my own Pisces line, the nation's token total was first written one too high (2,262,493). I corrected it to 2,262,492 within a minute. No other line was touched.

## Repetition
- **Lines:** no line of more than 40 characters repeats anywhere in the 130 sheets, apart from the template's fixed lines (the two italic header lines and the table headers). That includes the "Who to compare" bullets.
- **Most-reused sources** (pointer cells, out of 130 sheets):
  - Harrison, *The Missionary's Curse*: 11 sheets.
  - Gillin, *Warlord: Yen Hsi-shan in Shansi Province*: 10 (two spellings).
  - Hinton, *Fanshen* (some sheets with *Shenfan*): 10.
  - The CHARLS ageing survey: 8.
  - Edgerton-Tarpley, *Tears from Iron*: 6.
  - Johnson, *Spectacle and Sacrifice*: 6.
  - Everything else appears in 3 sheets or fewer.

  The repeats are spread across signs, and each is given a reason specific to its concept. Even so, the Catholic-village book and the Yan Xishan monograph are the nearest thing to default pointers.

## Thin, repetitive or generic sheets
- **Most query-heavy** (pointers given as a source type plus a query, not a named source): Gemini/Gossip (3 of 14) and Leo/Recognition (3 of 13). Ten more sheets have 2 such rows, including Gemini/Mediation, Taurus/Possessiveness, Scorpio/Secrecy and Libra/Domain.

  This is the reverse of most earlier nations, where query rows were more common. Nearly every pointer here is a named source. That is good for depth but raises the stakes for verification.
- **Self-flagged as thin in places** (the Data flag names a thin part):
  - Aries: Domain, Anger.
  - Taurus: Possession, Stubbornness, Sensuality.
  - Gemini: Communication, Gossip.
  - Virgo: Usefulness, Analysis.
  - Libra: Indecision.
  - Scorpio: Betrayal, Secrecy.
  - Sagittarius: Domain, Faith, Freedom, Conviction, Fundamentalism.

  The Sagittarius sheets say that present-day data on religion and freedom is "politically filtered". That is honest, and the research will have to rely on historical and ethnographic routes.
- **Shortest sheets** (all still over 990 words): Sagittarius/Honesty (993), Scorpio/Crisis (997) and Sagittarius/Education (1,035).
- **Generic sheets:** none found. Spot-checks of Aries/Identity, Sagittarius/Faith and Gemini/Gossip found specific Shanxi pointers. Examples:
  - Li Rong's 1985 article on the zoning of Mandarin, which set Jin apart as its own group.
  - Han Lin's 铎书 (1641).
  - The Oberlin Shansi records.
  - Katz's *Images of the Immortal*.
  - Zhao Shuli's fiction.
  - Li Rui's *Houtu*.
  - The 祁太秧歌 song-and-dance folk opera.

  All of these are real, well-known items, each marked *check*.

## Do the sheets exploit the nation's depth?
Largely yes. Counts are sheets out of 130 that mention each item:

| Item | Sheets |
|---|---|
| Jin dialect group 晋语 (subgroups named in most Domain sheets) | 123 |
| Hui Muslims | 127 |
| Classical-language or pre-modern pointer (every sheet has at least one: dynastic sources, gazetteers, steles, Northern Wei) | 130 |
| Datong and the northern frontier (Jinbei) | 113 |
| Jinzhong basin (Pingyao, Qi county) | 112 |
| Yuncheng and Hedong (Jinnan) | 109 |
| Lüliang | 107 |
| Coal and mining towns | 106 |
| Linfen | 93 |
| Catholic villages | 89 |
| Wutaishan (with Tibetan Buddhist monastics in 40 sheets) | 82 |
| Mongol | 67 |
| Shangdang (Changzhi, Jincheng) | 61 |
| County and local gazetteers 地方志 | 61 |
| Shanxi merchants 晋商 | 47 |
| Xinzhou | 41 |
| Yangquan | 41 |
| Hequ, Baode and Pianguan | 34 |
| Yan Xishan era | 32 |
| Ancient state of Jin (Zuozhuan, Guoyu) | 29 |
| Zou Xikou 走西口 | 28 |
| Guandi cult | 23 |
| Northern Wei and Yungang | 19 |
| Manchu | 18 |

- **Scripts:** search terms are in Chinese characters on all 130 sheets. Mongolian script or Cyrillic appears in 32 sheets and Tibetan script in 23, both for comparison terms.
- **Weaker spots:**
  - The Taosi and Neolithic past appears in only 6 sheets.
  - The Shanxi Provincial Archives are named in only 4 sheets and the Shanxi Museum in 11. Archives are mostly reached through county gazetteers and university collections.
  - Jin dialect phonological markers (圪 words, the entering tone 入声) appear in only 7 sheets. Most dialect pointers name the group rather than give dialect forms of the concept's words.
  - Errentai 二人台 appears in 14 sheets and Jin opera 晋剧 in 19.
  - Manchu, Mongol and Tibetan Buddhist communities inside Shanxi are small. The sheets mark them *check* where their presence is uncertain.

## Open items for the author
- **Lands:** the tracker header lists Shanxi only. The sheets treat it as a working list for you to confirm.
  - **Inner Mongolia:** it is named in 27 sheets as a comparison, mainly as the destination of 走西口 migration and the home of related Jin-speaking communities.
  - **The Jin dialect area beyond Shanxi:** it also reaches into northern Shaanxi, western Hebei and northern Henan, which belong to other member states.

  Please confirm whether these cross-border Jin-speaking areas stay comparison-only.
- **Diaspora:** Shanxi guild halls 会馆 and merchant networks elsewhere appear in 33 sheets, as comparison only.
- **Accuracy:** nothing is verified. The sheets lean on named sources more than earlier nations did, so the verification pass should check titles and dates.
