STATUS: done 2026-11-21. Run agent's report; the sheets are unverified.

# Min: springboard run report (Sat 11-21, wave 2, deeper brief)

**Result:** all 130 sheets are done. Every first line reads `STATUS: done 2026-11-21, not verified`. The run used 13 sign agents: 12 that finished, plus one Aquarius agent that a usage limit stopped before it wrote anything, which was relaunched. The whole-nation QA (`springboard_qa.py Min`) scanned 130 sheets and found **0 problems**. One hand fix was made: six copied "Who to compare" bullets in Scorpio (see below). No pointer has been checked.

**Inputs:** the deeper brief, with the operational lessons added to every sub-agent prompt:
- no zodiac, astrolog* or horoscope words;
- the lands note once, in the Domain sheet;
- the no-reuse rule also covers the compare bullets;
- the concept is stated neutrally;
- Hermes_research is never opened;
- diaspora pointers are for comparison only;
- temporary files stay in the nation's own scratchpad `tmp/` folder.

Two run-specific lines were added:
- **Comparison only:** Taiwan (a separate target) and the Min-speaking Chaoshan (Teochew) and Leizhou areas, which lie in Guangdong (Yue), are for comparison only.
- **Hakka bullets (from Sagittarius on):** a Hakka bullet is optional. Where there is one, it gives its own concept-specific reason, never a bare "named only".

**Lands:** the sheets are written for the tracker header's provinces, Fujian and Hainan. The prompt gave these as a working list that the author still confirms. Nothing came from a `00 - Scope.md`, a unit list or Hermes_research, and no sheet mentions Hermes. The note that the lands are still to be settled appears in all 12 Domain sheets and in no concept sheet. The Hakka appear only briefly, as a separate sub-unit.

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,178 | 1,275 (Domain) | 13.8 (12-15) | 178,866 | 08:03-08:18 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,181 | 1,281 (Ownership) | 14.3 (13-15) | 196,407 | 08:19-08:34 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,161 | 1,290 (Domain) | 15.2 (14-16) | 186,828 | 08:34-08:47 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,141 | 1,239 (Domain) | 14.5 (13-16) | 192,596 | 08:47-09:01 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,133 | 1,265 (Domain) | 14.2 (13-15) | 202,649 | 09:01-09:16 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,156 | 1,264 (Domain) | 14.5 (14-15) | 188,485 | 09:16-09:29 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,227 | 1,285 (Domain) | 14.5 (13-16) | 210,561 | 09:30-09:44 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 (1 hand fix) | 1,142 | 1,240 (Domain) | 13.5 (13-14) | 186,408 | 09:45-09:57 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,185 | 1,286 (Domain) | 14.3 (14-15) | 201,942 | 09:58-10:11 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,208 | 1,272 (Domain) | 14.4 (14-16) | 191,073 | 10:12-10:25 |
| 11 | Aquarius | 10/10 | 2 | 1 (usage limit) | 0 | 1,126 | 1,255 (Domain) | 14.0 (13-15) | 196,930 (+ unreported) | 10:26-10:35; 11:42-11:55 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,128 | 1,186 (Domain) | 14.3 (13-15) | 217,264 | 11:56-12:12 |

## Tokens and wall-clock
- **Sub-agent tokens: 2,350,009** in all (the sum of the 12 completed sign agents' hand-back usages; 483 tool uses). That is about 18,080 per sheet, in line with Jin, Qin and Zhongyuan (2.26 to 2.37M).
- **Uncounted tokens:** the first Aquarius agent was cut off and reported no usage, so its partial tokens (about 9 minutes of reading) are not in the total.
- **Run agent:** its own tokens are not counted here; the main session adds them.
- **Wall-clock:** start 08:02 MST, end 12:15 MST (report finished), about 4 h 13 min.
- **Interruption:** the 5-hour usage limit stopped the first Aquarius agent at about 10:35, before it wrote any sheet. The run was paused from about 10:35 to 11:43, about 1 h 8 min. On resuming, the status script showed Aquarius at 0/10, and one relaunch wrote all ten sheets. Without the pause the run took about 3 h 5 min. Signs took 12.2 to 16.1 minutes each.
- **Words:** 151,240 in all by `wc -w`, markup included.
  - The average is 1,163, and sheets run from 1,025 (Pisces Fear) to 1,290 (Gemini Domain).
  - 34 sheets are over the brief's "up to about 1,200", 14 of them over 1,250. None is over the scan's 1,300.
  - The Domain sheets run longest. Per lesson 4, no length instruction was added to the prompts.

## Rule breaks and fixes
1. **QA:** 0 problems in every sign and in the whole-nation scan. The scan found:
   - no zodiac words;
   - no "Indian", not even in a title;
   - no "sikh"-pattern hit;
   - no URLs;
   - no finding phrasing.

   All 130 "Held for review" lines read "none".
2. **Copied compare bullet (Scorpio, hand fix):**
   - **What the run agent's own repeat check found:** the identical bullet "Hakka of western Fujian: named only." in six Scorpio sheets: Betrayal, Control, Trust, Revenge, Secrecy and Crisis. This breaks lesson 6. The QA scan does not check it.
   - **The fix:** the smallest edit. Each bullet now gives a concept-specific reason, for example "only where Min and Hakka traders give each other credit in shared market towns" (Trust). The status lines were not touched.
   - **Prompt change:** later prompts said the Hakka bullet must carry its own reason. In Sagittarius that put a Hakka bullet on every sheet, each with a distinct reason. From Capricorn on, the prompt also said the bullet is optional.
3. **Checkpoint-order breaches (process only; the final files are clean):**
   - **Libra:** the agent removed repeated lines from Fairness to Impartiality after some sheets were already marked done, then rewrote their status lines.
   - **Sagittarius Domain:** the first draft ran 1,389 words and was briefly marked done. The agent set it back to in progress and trimmed it to 1,286 with no pointer dropped.
4. **Repetition after the fix:** no line over 25 characters (outside the template's fixed lines and headings) repeats anywhere across the 130 sheets. No compare bullet is copied. Of 1,856 pointer rows, 1,784 have distinct first cells.

## Thin, repetitive or generic sheets (by name)
- **Fewest pointers:** Aries 10 Recklessness has 12. These sheets have 13:
  - Aries: Courage, Anger.
  - Taurus: Stubbornness.
  - Cancer: Abandonment.
  - Scorpio: Domain, Betrayal, Trust, Revenge, Secrecy.
  - Aquarius: Idealism, Nonconformity, Detachment.
  - Pisces: Fear.

  Scorpio is the leanest sign (13.5 average).
- **Shortest:** Pisces 11 Fear (1,025), Cancer 08 Abandonment (1,037), Aquarius 05 Idealism (1,052) and Scorpio 08 Secrecy (1,062). All are still above the brief's 1,000 aim.
- **Spot read of Aries 08 Anger: specific, not generic.** It names:
  - Zhu Xi's *Classified Conversations*;
  - Lin Zexu's 制怒 motto;
  - Hu Quan and the Five Lords Temple in Haikou;
  - the Black and White Flag feuds;
  - 斩鸡头 oath practice;
  - the Li 禁公/禁母 accusations;
  - Min and Puxian opera.
- **Weakest pre-modern coverage:** Scorpio 06 Trust. Its oldest items are oath-swearing practice and qiaopi, with no classical or dynastic source. Gemini 05 Connection and 09 Gossip lean on genealogies, proverbs and teasing songs rather than a dated pre-modern text. Every other sheet has a dynastic, classical, gazetteer or old-temple pointer.
- **Most reused works** (as a pointer's first cell):

| Work | Sheets |
|---|---|
| Kenneth Dean (any title) | 30 |
| Zheng Zhenman | 26 |
| CNKI | 24 |
| Zhu Xi | 23 |
| Michael Szonyi | 18 |
| Mazu cult and its temples | 15 |
| CGSS | 11 |

Dean and Zheng's *Ritual Alliances of the Putian Plain* is in 8 sheets, and Stübel's *Die Li-Stämme der Insel Hainan* and Doolittle's *Social Life of the Chinese* in 5 to 6 each. These are the field's standard works, so the reuse is expected, but a researcher will meet Dean and Zheng often.

## Pointers per sheet
14.3 on average (12 to 16), 1,856 pointer rows in all. By sign, the averages run from 13.5 (Scorpio) to 15.2 (Gemini).

## Do the sheets exploit the nation's depth?
Mostly yes.

**Regions and peoples (sheets that mention each group):**

| Group | Sheets |
|---|---|
| Fuzhou and Mindong | 130 |
| Hainanese Han | 130 |
| Li (Hlai) | 130 |
| Puxian (Putian and Xianyou) | 119 |
| She | 111 |
| Hui, including the Utsul (Tsat) of Sanya | 109 |
| Minbei and Minzhong uplands | 83 |
| Tanka boat people | 79 |
| Hainan Miao (Kim Mun) | 70 |
| Lingao (Be) | 37 |
| Cun | 11 |

**Search-term languages (sheets with a term row in each):**

| Language | Sheets |
|---|---|
| Hokkien, Southern Min or Minnan | 130 |
| Hainanese | 113 |
| Fuzhou or Eastern Min | 125 |
| Hlai | 86 |
| She | 50 |
| Puxian | 30 |
| Classical Chinese | 22 |
| Tsat | 5 |
| Lingao | 2 |

Church romanizations (POJ or Foochow Romanized) are cited in 58 sheets.

**Hainan's depth:** many sheets draw on Hainan sources beyond the Li:
- Wenchang emigrant families (17 pointers);
- the Five Lords Temple and Su Dongpo's exile;
- Tanmen's 108 Brothers temples;
- Tianya Club;
- the free trade port;
- the "migratory-bird" retirees of Sanya.

**Weak spots:**
- **Northern Min (Jian'ou) and Central Min:** almost never given their own search-term rows, though the Minbei uplands appear in 83 sheets.
- **Lingao, Cun and Tsat:** terms are rare. They are mostly named as compare units, with "query" routes instead of words, which is honest given how thin they are.
- **Classical Chinese terms:** in only 22 sheets, although Zhu Xi and gazetteers are frequent pointers.

The diaspora (Southeast Asian Hokkien, Hainanese and Fuzhou communities), Taiwan and Chaoshan appear as comparison only.

## For the author
- The lands (Fujian and Hainan) are a working list to confirm.
- About 1 h 8 min of the run was lost to the usage-limit pause, and the cut-off Aquarius agent's tokens are unreported.
