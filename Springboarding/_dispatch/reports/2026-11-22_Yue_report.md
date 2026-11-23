STATUS: done 2026-11-22. Run agent's report; the sheets are unverified.

# Yue: springboard run report (Sun 11-22, wave 1, deeper brief)

**Result:** all 130 sheets are done, and every first line reads `STATUS: done 2026-11-22, not verified`. The run used 12 sign agents, one per sign, with no relaunches. The whole-nation QA (`springboard_qa.py Yue`) scanned 130 sheets and found **0 problems**. There was one hand fix: two Flags lines copied between signs (see below). No pointer has been checked.

**Inputs:** the deeper brief, with the operational lessons added to every sub-agent prompt:
- no zodiac, astrolog* or horoscope words;
- the lands note goes once, in the Domain sheet;
- the no-reuse rule also covers the compare bullets;
- the concept is stated neutrally;
- Hermes_research is never opened;
- diaspora pointers are comparison only;
- temporary files stay in the nation's own scratchpad `tmp/` folder;
- the South Asian rule, the "Indian" rule and the brief's binding rule against any universals list.

Run-specific lines added to the prompts:
- **Comparison only:** Min (Fujian, Hainan), the Hakka sub-unit, Taiwan and Vietnam are separate targets. The Min-speaking Chaoshan (Teochew) and Leizhou areas lie inside Guangdong, so they count as Yue's own internal groups.
- **Hakka bullets:** optional, and where present they carry a reason specific to the concept (the Min run's lesson). The whole-nation scan found no copied Hakka bullet.
- **Law:** Libra was briefed for the letter of the law across the four legal systems (the mainland codes, Hong Kong's common law and Macau's Portuguese-derived civil law). Capricorn was briefed for the spirit of the law. Scorpio, Sagittarius, Aquarius and Pisces (for Crime) were told that law questions belong to Libra or Capricorn.
- **From Leo on:** no Flags line may be copied from an earlier sign, and the "Languages needed" line must say what each language is for in that sheet.
- **Pisces only:** a depth nudge toward the parts of the lands that earlier signs had rarely used (see "Depth").

**Lands:** the sheets are written for the tracker header's four lands: Guangdong, Guangxi, Hong Kong and Macau. The prompt gave these as a working list that the author still confirms. Nothing came from a scope file, a unit list or Hermes_research, and no sheet mentions Hermes or universals. The "exact lands still to be settled" note appears in the 12 Domain sheets and in no concept sheet. The one other hit on "to be settled", in Cancer Home, is the gloss of the idiom 安土重遷, not the note.

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Shortest | Pointers (avg, range) | Sub-agent tokens | Tool uses | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,166 | 1,288 (Domain) | 1,095 (Recklessness) | 14.7 (14-16) | 172,790 | 44 | 05:04-05:18 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,162 | 1,296 (Domain) | 1,081 (Sensuality) | 14.1 (14-15) | 199,858 | 36 | 05:19-05:32 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,191 | 1,282 (Domain) | 1,121 (Mediation) | 14.9 (14-16) | 194,789 | 39 | 05:32-05:44 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 (1 hand fix) | 1,183 | 1,265 (Domain) | 1,116 (Nurture) | 14.3 (13-15) | 225,162 | 43 | 05:45-05:59 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,144 | 1,285 (Creativity) | 1,037 (Dignity) | 13.7 (12-16) | 246,755 | 60 | 06:00-06:17 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,207 | 1,289 (Domain) | 1,143 (Criticism) | 14.1 (13-15) | 232,336 | 45 | 06:17-06:32 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,255 | 1,288 (Domain) | 1,209 (Indecision) | 13.5 (12-14) | 242,070 | 81 | 06:32-06:49 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,260 | 1,292 (Domain) | 1,205 (Crisis) | 14.0 (14) | 261,400 | 78 | 06:49-07:09 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,260 | 1,300 (Faith) | 1,168 (Honesty) | 14.1 (13-15) | 221,256 | 64 | 07:09-07:25 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,213 | 1,295 (Domain) | 1,142 (Merit) | 12.9 (12-14) | 264,849 | 76 | 07:26-07:47 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,192 | 1,291 (Domain) | 1,115 (Hope) | 13.4 (12-14) | 253,645 | 81 | 07:48-08:07 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,229 | 1,300 (Domain) | 1,134 (Intuition) | 13.0 (12-14) | 297,381 | 88 | 08:07-08:33 |

## Tokens and wall-clock
- **Sub-agent tokens: 2,812,291** in all, with 735 tool uses. These are the 12 hand-back usages, and no relaunch was needed. That is about 21,630 per sheet, above Saturday's Sinian sub-units (2.26 to 2.40M each).
- **Why it cost more:** later agents read more of the earlier sheets to avoid repeats. Tool uses rose from about 40 per sign in Aries to Virgo, to 76 to 88 per sign from Libra on. Pisces was the costliest sign (297,381).
- **Run agent:** its own tokens are not counted here; the main session adds them.
- **Wall-clock:** start 05:03 MST, last sheet 08:33 MST, report finished 08:35 MST: about 3 h 32 min, with no usage-limit stop. (The completion line in the Run log, written before the report was finished, says 08:40 and 3 h 37 min; 08:35 is correct.) Signs took 11.7 to 25.3 minutes each and got slower as the nation filled up.
- **Words:** 156,635 in all by `wc -w`, markup included.
  - The average is 1,205, and sheets run from 1,037 (Leo Dignity) to 1,300.
  - 72 sheets are over the brief's "up to about 1,200", and 40 are over 1,250.
  - None is over the scan's 1,300. Two sit exactly at 1,300 (Sagittarius Faith, Pisces Domain), and five more are at 1,295 to 1,298.
  - Per lesson 4, no length instruction was added to the prompts.

## Rule breaks and fixes
1. **QA:** 0 problems in every sign and in the whole-nation scan. That means:
   - no zodiac words;
   - no "Indian" anywhere, not even in a title;
   - no "sikh" or "hindi" pattern hit (so lesson 9's false positives did not arise);
   - no URLs and no finding phrasing.
2. **Copied Flags lines (Cancer, hand fix):** the run agent's repeat check found two "Languages needed" lines copied word for word from Gemini (Learning into Home, Siblings into Family). The QA scan does not check for this. The fix was the smallest edit: each line now says what its languages are for in that sheet, for example "Zhuang (for marriage-residence customs)". The status lines were not touched. From Leo on, the prompt forbade copied Flags lines, and none recurred.
3. **Process notes (the final files are clean):**
   - **Libra:** the agent found that its Domain sheet repeated a Gemini pointer (Zhuang sworn kin 打老同) and swapped it for another before finishing.
   - **Pisces:** the agent set all 12 status lines to done together at the end, after its own check, not one by one as the checkpoint rule asks. All 12 files are complete.
4. **South Asian rule:**
   - The "Held for review" line is category-only in all 130 sheets: 112 name South Asian-heritage communities as a category, and 18 read "none".
   - 13 sheets (all 11 in Aries, plus Taurus Domain and Self-worth) word the category line in their own way (for example "courage pointers touching South Asian-heritage communities in Hong Kong"), and every one of them names no work, person or institution.
   - No South Asian pointer appears anywhere else.

## Repetition (run agent's check across the whole nation)
- **Lines and rows:** no line over 25 characters repeats anywhere across the 130 sheets. That covers every search-term row, pointer row, compare bullet, Flags line and query, outside the template's fixed lines and the category-only Held line.
- **Compare bullets:** 1,217, and none is copied (checked at any length, case-insensitive).
- **Pointers:** 1,805 rows, and 1,800 have distinct first cells. Five sources appear in two signs each, every time in a differently worded row with its own concept-specific reason:
  - Jaschok, *Concubines and Bondservants* (Taurus Possessiveness; Sagittarius Freedom);
  - the national time-use survey (Leo Domain; Capricorn Domain);
  - Chan, Selden and Pun, *Dying for an iPhone* (Leo Dignity; Sagittarius Meaning);
  - Yang Su, *Collective Killings* (Leo Humiliation; Sagittarius Fundamentalism);
  - Sinn, *Pacific Crossing* (Libra Autonomy; Sagittarius Travel).

  The Sagittarius and Pisces agents both said that the obvious Yue sources were mostly used up by the late signs, and that a few came back in a new role. The scan found no copied row.

## Thin, repetitive or generic sheets (by name)
- **Fewest pointers (12, the brief's floor):**
  - Leo: Humiliation.
  - Libra: Peace at any price.
  - Capricorn: Duty, Merit, Order.
  - Aquarius: Hope.
  - Pisces: Dissolution, Intuition, Fear.

  **27 sheets have 13 pointers.** The late signs are the leanest: Capricorn averages 12.9, Pisces 13.0 and Aquarius 13.4, against 14.1 to 14.9 in Aries to Gemini. As the nation filled up, the agents traded pointer count for length per pointer.
- **Shortest:** Leo Dignity (1,037), Leo Humiliation (1,059), Leo Leadership (1,054), Taurus Sensuality (1,081) and Aries Recklessness (1,095). Leo is the leanest sign by words (average 1,144).
- **Repetitive or generic:** none found by the scans. The spot reads found them specific:
  - **Aries Anger** names 打小人 at the Canal Road Flyover, 涼茶 and 肝火, Zhao Ziyong's 《粵謳》 (1828), Lamley on Chaoshan lineage feuds, the 1967 riots, Macau's 12-3 incident and the 2011 Xintang unrest.
  - **Capricorn Law** names Dong 侗款 covenants, Miao 埋岩 in Rongshui, Qing 訟師, *Ng Ka Ling*, Macau's legal localization, 普法 in Zhuang areas and Chaoshan lineage mediation. It stays on the spirit of law.
  - **Sagittarius Faith:** its Flags and queries are concept-specific.
  - **Pisces Crime** routes all law questions to Libra and Capricorn.

## Pointers per sheet
- **Aries:** Domain 14; Self-assertion 14; Identity 16; Autonomy 15; Initiative 15; Beginning 15; Courage 15; Independence 15; Anger 14; Competition 15; Recklessness 14.
- **Taurus:** Domain 15; all ten concepts 14.
- **Gemini:** Domain 16; Communication 16; Information 15; Learning 15; Curiosity 15; Connection 15; Duality 14; Siblings 15; Mediation 14; Gossip 14.
- **Cancer:** Domain 15; Home 15; Family 14; Belonging 15; Nurture 14; Protection 14; Shelter 15; Care 14; Abandonment 13; Motherhood 14.
- **Leo:** Domain 14; Creativity 16; Self-expression 15; Pride 14; Recognition 14; Being seen 13; Dignity 13; Humiliation 12; Generosity 14; Leadership 13; Play 14; Honor 13; Joy 13.
- **Virgo:** Domain 13; Work 14; Service 15; Usefulness 14; Analysis 15; Discernment 13; Perfectionism 14; Criticism 14; Health 14; Improvement 15.
- **Libra:** Domain 14; Justice to Diplomacy 14 each; Reciprocity 13; Indecision 13; Peace at any price 12; Projection 13.
- **Scorpio:** all 11 sheets 14.
- **Sagittarius:** Domain 13; Faith 14; Meaning 14; Freedom 14; Truth 14; Belief 14; Conviction 14; Travel 15; Honesty 14; Education 15; Fundamentalism 14.
- **Capricorn:** Domain 14; Authority 13; Duty 12; Responsibility 13; Discipline 14; Ambition 13; Hierarchy 13; Merit 12; Law 13; Order 12.
- **Aquarius:** Domain 14; Community 14; Group 13; Equality 14; Reform 14; Idealism 14; Friendship 13; Nonconformity 13; Detachment 13; Hope 12.
- **Pisces:** Domain 13; Compassion 14; Empathy 13; Self-sacrifice 14; Dissolution 12; Boundary 13; Escapism 13; Spirituality 14; Surrender 13; Intuition 12; Crime 13; Fear 12.

**Total:** 1,805 pointers, an average of 13.9 per sheet. The spread: 12 pointers in 9 sheets, 13 in 27, 14 in 68, 15 in 22 and 16 in 4.

## Do the sheets exploit the nation's depth?
**Mostly yes, with a clear core-to-edge gradient.** The counts below are sheets out of 130 that name each item.

**Scripts and languages, strong:**
- every sheet carries Jyutping Cantonese and Portuguese for Macau;
- 126 carry Standard Zhuang;
- 117 mark traditional and simplified script forms;
- terms in Teochew, Dong (Kam) and Iu Mien occur often.

**Peoples, strong:**
- Zhuang 130, Teochew/Chaoshan 122, Yao 120 and Dong 103;
- Miao 78, Macanese 75, Jing 73, Tanka/Danjia boat people 66 and Siyi/Taishanese 62;
- Leizhou 52, Maonan 49 and Mulao 41;
- the Guangxi Yue varieties and Pinghua appear about 30 times each.

**Pre-modern pointers:** every one of the 130 sheets has at least one in section 2, among them:
- Song to Qing gazetteers;
- Nanyue and Southern Han material;
- 《粵謳》, 《赤雅》 and 《廣東新語》-type sources;
- Dong and Miao oral covenants;
- Zhuang Buluotuo texts.

**Weak spots:**
- **Sawndip (古壮字), the Zhuang character script:** in only 7 sheets.
- **Smaller Guangxi peoples:** the She (8), Shui (9), Yi (5) and Gelao (3) are rare.
- **Hong Kong:** the New Territories Indigenous villagers (原居民) and the Weitou/Punti appear in only about 6 and 19 sheets.
- **Regions:**
  - The Pearl River Delta core dominates: Hong Kong 130, Macau 130, Guangzhou 123, Shenzhen 87.
  - Northern Guangdong (Shaoguan, Qingyuan, Lianshan and Liannan) has 18.
  - Wuzhou and Yulin have 9, Guilin and Liuzhou 15, and Baise and Hechi 17.
  - Western Guangdong outside Leizhou has 38.
- **The depth nudge:** added to the Pisces prompt only, it lifted these counts noticeably within that sign. For example, northern Guangdong went from 11 to 18 sheets, Baise and Hechi from 10 to 17, and the She, Shui, Yi and Gelao together from 11 to 25. **Lesson for the next nations:** give this kind of nudge from the first sign, not the last.

**Hakka:** named in 61 sheets, always briefly and with a concept-specific reason, never as the focus.

**Diaspora:** Southeast Asian, North American and other overseas Cantonese and Taishanese communities appear only as comparison.
