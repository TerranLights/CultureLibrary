# Qin springboards: run report (2026-11-21, wave 1)

**Result:** all 130 sheets are marked `STATUS: done 2026-11-21, not verified`. The run used 12 sign agents and no relaunches. The whole-nation QA (`springboard_qa.py Qin`) scanned 130 sheets and found 0 problems. No pointer has been checked; the sheets are unverified.

**Inputs:** the deeper brief, which puts accuracy and depth first, with the operational lessons added to every sub-agent prompt:
- no zodiac, astrolog* or horoscope words;
- the lands note once, in the Domain sheet;
- the no-reuse rule also covers the compare bullets;
- the concept is stated neutrally, never as what the culture believes or values;
- Hermes_research is never opened;
- diaspora pointers are for comparison only;
- temporary files stay in the nation's own scratchpad `tmp/` folder.

Every prompt also told the agent to read one concept block, write that sheet, and only then read the next.

**Lands:** the sheets were written for the tracker header's provinces: Shaanxi, Gansu, Ningxia and Qinghai. The prompt gave these as a working list that the author still has to confirm. Nothing came from a `00 - Scope.md`, a unit list or Hermes_research, and no sheet mentions Hermes. The note that the lands are still to be settled appears in all 12 Domain sheets and in no concept sheet.

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA problems | Avg words | Longest | Pointers per sheet | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,215 | 1,276 (Self-assertion) | 14-16 | 179,760 | 05:04-05:20 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,187 | 1,285 (Domain) | 13-15 | 196,679 | 05:20-05:35 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,211 | 1,289 (Domain) | 14 | 192,093 | 05:35-05:50 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,161 | 1,284 (Domain) | 14-16 | 186,050 | 05:50-06:03 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,134 | 1,267 (Domain) | 13-15 | 197,053 | 06:03-06:17 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,217 | 1,279 (Domain) | 14-15 | 178,580 | 06:17-06:29 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,118 | 1,272 (Domain) | 14 | 209,422 | 06:29-06:44 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,158 | 1,265 (Domain) | 14-16 | 196,513 | 06:44-06:58 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,125 | 1,249 (Domain) | 13-15 | 185,247 | 06:58-07:12 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,218 | 1,271 (Law) | 14-16 | 185,012 | 07:12-07:24 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,138 | 1,237 (Domain) | 13-15 | 199,124 | 07:24-07:37 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,163 | 1,277 (Domain) | 14-16 | 214,893 | 07:37-07:55 |

## Tokens and wall-clock
- **Sub-agent tokens:** 2,320,426 in all. That is 12 sign agents and no relaunches, about 17,850 per sheet. This is in line with Days 3 and 4 (2.23 to 2.50M per nation). The run agent's own tokens are not counted here; the main session adds them.
- **Wall-clock:** the run agent started at 05:03 and launched Aries at 05:04. Pisces returned at 07:55, and the report was finished at 07:57, so the run took about 2 h 55 min. Signs took 11.6 to 16.8 minutes each. The run went in parallel with the other wave-1 nations (Zhongyuan, Bashu and Jin).
- **Words:** 151,976 in all by `wc -w`, markup included. The average is 1,169, and sheets run from 1,046 to 1,289. 39 sheets are over the brief's "up to about 1,200", and 19 of those are over 1,250. None is over the scan's 1,300 line. The Domain sheets run longest (1,237 to 1,289). This nation runs about 80 to 90 words a sheet longer than the Day 4 nations (Ingushetia averaged 1,083). Per lesson 4, no length instruction was added to the prompts.

## Rule breaks and fixes
1. **No QA problems in any sign, and nothing was relaunched or edited by hand.** The scan found no zodiac words and no "Indian", not even in a title. It found no "sikh"-pattern hit and no law outside Libra and Capricorn. It flagged no finding phrasing.
2. **Self-corrected over-length Domain sheets (process notes, final state clean):**
   - **Leo Domain:** the first draft ran 1,384 words. The agent set the sheet back to in progress and cut it to 1,267, keeping 13 pointers.
   - **Capricorn Domain:** the agent briefly marked the sheet done at 1,416 words, then cut it to 1,270 and marked it done again. This is a small breach of the checkpoint order, because the done line should be the very last write. The final file is correct.
3. **Held for review:** all 130 sheets read "none". No South Asian material appears anywhere.

## Thin, repetitive or generic sheets (by name)
- **Fewest pointers (13):** Taurus 09 Stubbornness, Leo 00 Domain (after its cut), Sagittarius 05 Belief and 06 Conviction, and Aquarius 05 Idealism, 07 Nonconformity and 09 Hope.
  - A spot read of Conviction and Hope found them specific, not generic. Conviction names Li Yong of Zhouzhi, the Jahriyya memorial rites, Hu Songshan of Tongxin, Gendun Chöphel of Rebkong, Döndrup Gyal, the Babusha "six old men" and the *Spark* samizdat. Hope names the Hexi precious scrolls, Shandao at Xiangji Temple, Xihaigu literature, Huining as the "exam county" and the Mothers' Water Cellar records.
  - These are abstract concepts, and they lean more on modern literature and campaign history than on surveys.
- **Shortest:** Sagittarius 06 Conviction (1,046), Libra 08 Indecision (1,074), Scorpio 09 Power (1,076), and Leo 06 Dignity and 12 Joy (1,080 each). All are still above the brief's 1,000 aim.
- **Weakest pre-modern coverage:** Sagittarius 03 Freedom is the only sheet with no pointer older than the 19th century. Its oldest items are the Tongzhi-era Hui uprising records and the 走西口 (*zou xikou*) migration songs. A classical pointer would fit there, for example Zhuangzi or the Zhongnan hermit tradition before the modern craze.
- **Repetition:** no line over 25 characters (outside the template's fixed lines) repeats anywhere across the 130 sheets. No "Who to compare" bullet is copied between sheets. Of 1,867 pointer rows, 1,784 have distinct first cells.
- **Most reused works** (sheets naming them anywhere):

| Work | Sheets |
|---|---|
| CNKI | 129 |
| Lu Yao | 21 |
| Jia Pingwa | 26 |
| CFPS | 15 |
| Lipman, *Familiar Strangers* | 14 |
| Gladney, *Muslim Chinese* | 11 |
| Chen Zhongshi, 《白鹿原》 (*White Deer Plain*) | 11 |
| Zhang Chengzhi, 《心灵史》 | 11 |
| Schram, *The Monguors* | 10 |
| Ekvall | 9 |
| Chau, *Miraculous Response* | 7 |
| World Values Survey | 7 |
| Makley | 6 |

  These are standard and fitting, but CNKI is close to a crutch: it is named in nearly every sheet as the route to the modern Chinese scholarship.
- **Formulaic compare roster:** the bullets' wording and reasons differ, but the roster is close to fixed. Counts out of 130 compare sections:

| Group | Sheets |
|---|---|
| Hui | 130 |
| Amdo Tibetans | 129 |
| Guanzhong | 125 |
| Mongols | 124 |
| Salar | 123 |
| Shaanbei | 123 |
| Tu | 116 |
| Kazakhs | 116 |
| Dongxiang | 113 |
| Bao'an | 100 |
| Hexi | 95 |
| Yugur | 85 |
| Shaannan | 85 |
| Longdong | 82 |
| Xihaigu | 49 |
| women as a group to separate | 12 |

  So gender variation is rarely named as a unit to separate.

## Pointers per sheet
The average is 14.4, with a range of 13 to 16: 7 sheets have 13, 79 have 14, 34 have 15 and 10 have 16. Every sheet is inside the brief's 12 to 16 band.

## Do the sheets use the nation's depth?
Largely yes for regions and peoples, less so for native scripts. These are counts of sheets out of 130:

| Feature | Sheets |
|---|---|
| **Peoples** | |
| Hui | 130 |
| Amdo Tibetan material | 130 |
| Tibetan script in the search terms | 130 |
| Mongols | 128 |
| Salar | 126 |
| Kazakhs | 118 |
| Tu (Monguor) | 117 |
| Dongxiang | 116 |
| Bao'an | 107 |
| Yugur | 97 |
| **Regions and places** | |
| Guanzhong | 129 |
| Shaanbei | 123 |
| Hexi Corridor | 104 |
| Linxia | 101 |
| Shaannan (Hanzhong, Ankang, Shangluo) | 90 |
| Longdong and Tianshui | 86 |
| Golok | 64 |
| Yushu | 60 |
| Xihaigu | 59 |
| Rebkong | 46 |
| Labrang | 41 |
| Kumbum | 30 |
| **Pre-modern and classical** | |
| At least one pre-modern or classical marker | 129 |
| Dunhuang | 42 |
| Classical Chinese titles | 30 |
| Local gazetteers | 30 |
| *Shiji* | 23 |
| Tibetan classics (Gesar, Milarepa, Tsongkhapa, Shantideva) | 19 |
| Qin bamboo slips (Shuihudi, Liye) | 7 |
| Islamic classics (Qur'an, hadith, Han Kitab, Liu Zhi, Ma Mingxin) | 8 |
| Western Xia (Tangut) | 4 |
| **Islam and folk forms** | |
| Sufi orders (*menhuan*) | 51 |
| Yan'an | 40 |
| Qinqiang opera | 29 |
| hua'er | 18 |
| xintianyou | 14 |
| Dungan, as comparison | 19 |

**Weak spots for the author:**
1. **The scripts of the Kazakh and Mongolian terms.** 77 of 118 Kazakh term rows and 74 of 111 Mongolian rows give Cyrillic forms, which are the forms used in Kazakhstan and Mongolia. Kazakhs in Aksay and Haixi write an Arabic-based script, and the Mongols of Haixi and Henan write the traditional vertical script. Only 20 Kazakh rows give Arabic script, and only 2 sheets (Cancer Domain and Family) give traditional Mongolian. Some rows already say "*check* Arabic-script form". The Cyrillic terms still find outside dictionaries and scholarship, but local sources will need the China-side scripts. Research should add them.
2. **Smaller languages are thin in the search terms.** Salar, Tu, Dongxiang, Bao'an and Yugur appear in the compare sections and pointers on most sheets. As search-term rows, though, they are rare: about 46 rows in all, with Salar in 7 and Dongxiang (Santa) in almost none. These languages are mostly unwritten or newly written, so this is partly honest thinness.
3. **Little Arabic and Persian vocabulary for Hui Islam.** Arabic script appears in 28 sheets, and Xiao'erjing in 1.
4. **Some classical layers are barely used:** the Qin legal and administrative slips (7 sheets; Libra and Capricorn are where they belong), Western Xia (4 sheets) and the Guanxue school of Zhang Zai (16 sheets).
5. **No Hakka or other migrant-Han pointer for Shaannan.** None was required by the prompt; the Hakka run separately.

**Data for the author:** whole-nation QA clean. Run log lines are appended, one per sign. The status grid reads 130/130.
