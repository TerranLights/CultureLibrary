STATUS: done 2026-11-21. Run agent's report; the sheets are unverified.

# Zhongyuan: springboard run report (Sat 11-21, wave 1, deeper brief)

**Result:** all 130 sheets are done, and every first line reads `STATUS: done 2026-11-21, not verified`. The run used 12 sub-agents (one per sign) and needed no relaunches. The whole-nation QA (`springboard_qa.py Zhongyuan`) found **0 problems** in 130 sheets, and no sheet needed a hand fix.

**Lands:** the sheets are written for the five units in the tracker header (Beijing, Tianjin, Hebei, Shandong, Henan). That list is still a working list for the author to confirm. Each sign's Domain sheet says once that the exact lands are still to be settled. No other sheet repeats the hedge or mentions a scope file. Nothing was taken from or cited from Hermes_research.

**Tokens and wall-clock:** the sub-agents used **2,370,337 tokens** in total (the sum of the 12 hand-back usages; there were no relaunches) and 498 tool calls. The run agent's own tokens are not included; the main session adds them. The run agent started at **05:03:46** and finished at **08:01**, about 3 h. The signs ran one after another and took 11.6 to 17.5 min each.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,094 | 1,162 (Self-assertion) | 14.8 (14-16) | 165,603 | 05:04-05:18 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,172 | 1,224 (Ownership) | 15.3 (14-16) | 189,326 | 05:18-05:31 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,142 | 1,248 (Domain) | 14.0 (13-15) | 175,911 | 05:31-05:43 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,190 | 1,254 (Domain) | 14.0 (13-15) | 194,553 | 05:43-05:56 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,180 | 1,260 (Domain) | 14.5 (13-16) | 218,583 | 05:56-06:13 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,141 | 1,199 (Service) | 15.0 (14-16) | 184,162 | 06:14-06:26 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,179 | 1,247 (Justice) | 14.6 (14-15) | 224,627 | 06:26-06:43 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,237 | 1,291 (Death) | 14.4 (14-15) | 216,322 | 06:43-06:59 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,125 | 1,254 (Domain) | 14.7 (14-16) | 188,404 | 06:59-07:12 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,183 | 1,224 (Law) | 14.6 (14-15) | 195,904 | 07:12-07:27 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,138 | 1,271 (Domain) | 14.5 (13-16) | 201,832 | 07:27-07:41 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,189 | 1,282 (Domain) | 15.1 (14-16) | 215,110 | 07:41-07:59 |
| | **Total** | **130** | **12** | **0** | **0** | **1,165** | **1,291** | **14.6 (13-16)** | **2,370,337** | **05:04-07:59** |

Word counts are by `wc -w`, markup included. Pointers are the rows of section 2.
- **Shortest sheet:** Aries/Competition, 1,033 words.
- **Over the brief's 1,200 guide:** 29 sheets, the most in Scorpio (8 of 11; sign average 1,237).
- **Over the 1,300 scan limit:** none.

## Rule breaks and fixes
- **QA:** no problems in any sign or in the whole-nation scan. That means no zodiac words, no "Indian", no URLs, no finding phrases, and no South Asian words outside the held lines.
- **Held for review:** three sheets set items aside, each as a category only: "translated scriptures of South Asian origin" in Aquarius/Detachment, Pisces/Compassion and Pisces/Spirituality. This follows the rule.
- **Law:** Libra and Capricorn carry the law.
  - I checked by hand the sheets outside those two signs that use law words.
  - The hits are "in-law" kinship terms, the imperial court or court crafts, and redirects such as "law goes to Libra and Capricorn" (for example in Taurus/Possessiveness, Virgo/Perfectionism, Scorpio/Betrayal and Pisces/Crime).
  - None of these sheets researches law.
- **Checkpoint order:** two small slips. Neither needed action, because both files are complete and pass the QA.
  - **Sagittarius:** the sub-agent reworded Travel's concept line after writing its STATUS line, to keep a "the culture regards" phrasing out.
  - **Capricorn:** the sub-agent read concept 1's block before its last rewrite of the Domain sheet.
- **False positives:** none in this nation. The "sikh" and "Indian" patterns caught nothing.

## Repetition and reuse
- **Within a sign:** no line is repeated in any sign.
- **Across the nation:** one short flag line appears twice: "Languages needed: modern and classical Chinese." It is in Taurus/Wealth and Gemini/Mediation, and was left as is.
- **Pointer reuse is moderate.** These pointers appear most often:

| Pointer | Sheets (of 130) |
|---|---|
| Jaschok and Shui, *The History of Women's Mosques in Chinese Islam* | 9 |
| Gottschang and Lary, *Swallows and Settlers* | 7 |
| Duara, *Culture, Power, and the State* | 6 |
| Yang, *A Chinese Village: Taitou* | 6 |
| Gladney, *Muslim Chinese* | 6 |
| Esherick, *The Origins of the Boxer Uprising* | 6 |
| CHARLS | 5 |
| Kipnis, *Producing Guanxi* | 5 |
| Meyer, *The Last Days of Old Beijing* | 5 |

  These are standard works on North China and the region's Hui. Each reuse gives a different reason in "What it would give", and no table row is copied. Some sheets in a sign lean on the same North China village ethnographies, so later research should look past them.

## Thin, repetitive or generic sheets
- **None is thin by length or by pointer count.** The leanest sheets have 13 pointers:
  - Gemini/Mediation (1,054 words)
  - Gemini/Gossip
  - Cancer/Motherhood
  - Leo/Humiliation
  - Leo/Joy (1,143 words)
  - Aquarius/Detachment
  
  Aries/Competition (1,033 words) and Aries/Initiative and Independence (1,043 each) are the shortest. They are full sheets.
- **None reads as generic.** Every sheet names places inside the five units at least 24 times, counting cities, prefectures and subregions. The lowest counts are Virgo/Analysis, Sagittarius/Honesty and Aries/Recklessness, which are still specific.
- **Recurring themes:** a few cross-sign comparisons recur in the "Who to compare" bullets, each with its own reason:
  - Qi against Lu inside Shandong
  - Henan's stigma and the "Central Plains" claim
  - north Hebei's Manchu and Mongol counties
  - the Shandong-origin communities in the Northeast and in Korea

## Pointers per sheet
- **Average:** 14.6, range 13 to 16.
- **By count:** 6 sheets have 13 pointers, 51 have 14, 58 have 15 and 15 have 16.

## Do the sheets use the nation's depth?
**Mostly yes.** Counts of sheets (of 130) that name each group, region or source type:

| Group, region or source type | Sheets |
|---|---|
| Hui (mosques, women's mosques, Cangzhou, Niujie, Kaifeng) | 126 |
| Korean residents and Shandong-origin Chinese in Korea | 110 |
| Manchu and banner people | 103 |
| Mongol counties of north Hebei | 95 |
| Christian villages and communities | 65 |
| The Jiaoliao/Jiaodong speech area | 50 |
| Cangzhou | 43 |
| Jin-speaking areas of Hebei and Henan | 22 |
| Xiong'an | 14 |
| Kaifeng Jewish descendants | 13 |
| Classical or founding texts (Confucian, Mohist, Daoist, Legalist; gazetteers, steles) | 111 |
| Pre-modern pointers of some kind | all 130 |

Search terms come in simplified characters with pinyin. Manchu, Mongolian (Cyrillic), Korean (hangul) and Hui Arabic/Persian loan terms are marked *check* where unsure.

The weaker spots:
- **Minority languages in the search terms** are thinner than the minorities in the pointers. Manchu and Mongolian forms are often a single *check* line.
- **Small non-Han peoples** (for example the Tujia or Zhuang who have moved into the cities) appear in only about 9 sheets.
- **Tianjin** is the least covered unit. All five units appear in every sheet, but Tianjin has 564 mentions, against Hebei 757, Shandong 788, Henan 952 and Beijing 1,334.

## For the author
- **The five-unit list:** Beijing, Tianjin, Hebei, Shandong, Henan is still a working list to confirm in Stage 0.
- **Diaspora pointers** (the Northeast's Shandong families, Shandong-origin Chinese in Korea) are kept as comparison only, under the ruling of 2026-11-18.
