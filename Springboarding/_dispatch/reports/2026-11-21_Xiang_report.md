STATUS: done 2026-11-21. Run agent's report; the sheets are unverified.

# Xiang 湘: springboard run report (Sinian Federation member state, deeper brief)

**Result:** all 130 sheets are done. Every first line reads `STATUS: done 2026-11-21, not verified`. The run used 12 sign agents plus 1 relaunch (Aquarius, after a usage-limit stop). The whole-nation QA (`springboard_qa.py Xiang`) found **0 problems** in 130 sheets, and no sheet needed a hand fix.

**Lands:** written for Hunan 湖南, the one province in the tracker header, as a working list the author still confirms. The lands note is in each sign's Domain sheet and nowhere else. No unit list was added, and nothing was taken from Hermes_research; every sub-agent was told not to open it.

**Tokens and wall-clock:**
- **Sub-agent tokens:** **2,322,854** in all. That is the sum of the 11 sign agents that finished and the Aquarius relaunch (177,855). The first Aquarius agent was stopped by the usage limit, and the harness reported no usage for it, so its tokens are **not included**. It wrote one sheet and part of a second, so its share is probably about 20,000 to 40,000 tokens (an estimate). The run agent's own tokens are also not included; the main session adds them.
- **Tool uses:** 473 by the 12 agents that reported usage.
- **Wall-clock:** the run agent started at **08:02:16 MST**. The Aries agent launched at 08:03, and the Pisces agent finished at 12:09. The report was written at **12:10 MST**. The total is about 4 h 8 min, including a pause of about 1 h 8 min.
- **Interruption:** the first Aquarius agent, launched at 10:24, was stopped by the 5-hour usage limit at about 10:35. By then the Domain sheet was done, and Community was in progress (1,242 words). The run paused from about 10:35 to 11:43. On the coordinator's resume message, one relaunch at 11:42 wrote only concepts 1 to 9. It checked and finished the half-written Community sheet and left the done Domain sheet untouched.
- **Working time, not counting the pause:** about 3 h. Signs took 10.0 to 16.9 min each.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,204 | 1,240 (Self-assertion) | 15.1 (15-16) | 173,457 | 08:03-08:18 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,181 | 1,278 (Domain) | 14.2 (14-15) | 192,848 | 08:18-08:32 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,172 | 1,293 (Domain) | 14.9 (14-16) | 184,312 | 08:32-08:45 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,163 | 1,229 (Domain) | 13.9 (13-14) | 188,016 | 08:45-08:57 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,155 | 1,273 (Domain) | 13.8 (13-14) | 210,430 | 08:58-09:15 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,161 | 1,292 (Domain) | 15.4 (15-16) | 190,556 | 09:15-09:28 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,149 | 1,264 (Domain) | 15.2 (15-16) | 193,660 | 09:29-09:41 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,151 | 1,258 (Domain) | 14.1 (14-15) | 199,701 | 09:42-09:55 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,222 | 1,284 (Faith) | 15.5 (14-16) | 205,974 | 09:55-10:10 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,156 | 1,252 (Authority) | 14.0 (14) | 189,638 | 10:11-10:24 |
| 11 | Aquarius | 10/10 | 2 | 1 | 0 | 1,244 | 1,282 (Domain) | 15.0 (14-16) | 177,855 + unreported | 10:24-10:35, pause, 11:43-11:53 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,221 | 1,294 (Self-sacrifice) | 14.7 (14-16) | 216,407 | 11:53-12:09 |
| | **Total** | **130** | **13** | **1** | **0** | **1,182** | **1,294** | **14.6 (13-16)** | **2,322,854 + unreported** | **08:03-12:09** |

- **Word counts:** by `wc -w`, markup included. The shortest sheet is Leo/Joy at 1,088 words, and the longest is Pisces/Self-sacrifice at 1,294. Forty-seven sheets run 1,200 to 1,294 words, and none is over the 1,300 flag. This is within the brief's "a little over is fine". Sheets run about 40 words longer on average than Jin's.
- **Pointers:** the rows of section 2, 1,901 in all. Every sheet is within 13 to 16.

## Rule breaks and fixes
- **QA:** nothing was flagged in any sign or in the whole-nation scan.
  - No zodiac, divination-label or horoscope words.
  - No "Indian".
  - No South Asian items. The Held-for-review line reads "none" on all 130 sheets.
  - No "sikh"-pattern false positives.
  - No mention of Hermes_research.
- **Hand fixes:** none.
- **Law:** the law material is in Libra (the letter of the law) and Capricorn (the spirit). Where a sheet in another sign touches law, it only sends the question on to Libra or Capricorn. I spot-checked Aries/Anger and Taurus/Ownership to confirm this.
- **Self-caught slips:**
  - In Pisces, the sub-agent first gave every sheet the same diaspora bullet under "Who to compare". It rewrote the bullet with a concept-specific reason on each sheet, then set the STATUS lines again. The final state is clean.
  - The Aquarius relaunch fixed one typo and one gloss in the half-written Community sheet before marking it done.

## Repetition
- **Lines:** no line of more than 40 characters repeats anywhere in the 130 sheets, apart from the template's three fixed lines (the two italic header lines and the pointer-table header). That includes the "Who to compare" bullets.
- **Most-reused sources** (pointer cells, out of 130 sheets):
  - Kuhn, *Rebellion and Its Enemies in Late Imperial China*: 11, under two spellings of the author's name.
  - Platt, *Provincial Patriots*: 7.
  - Perdue, *Exhausting the Earth*: 5.
  - Hunan University of Chinese Medicine: 4.
  - Ling Chunsheng and Rui Yifu, 湘西苗族调查报告 (1947): 3.
  - The CHARLS ageing survey: 3.
  - Zhangguying village: 3.
  - Everything else appears in 2 sheets or fewer.

  Kuhn and Platt are the nearest thing to default pointers. Each use carries a reason specific to its concept.

## Thin, repetitive or generic sheets
- **Most query-heavy** (pointers given as a CNKI or search query, not a named source): the **Cancer** sign. Abandonment, Care and Protection have 4 such rows out of 14. Shelter, Nurture, Belonging and Family have 3. In no other sign does a sheet have more than 2. The Cancer sheets also have the lowest pointer counts (13 to 14). This is the thinnest sign of the twelve, although each query is concrete and can be run.
- **Self-flagged as thin in places** (the Data flag names a thin part):
  - Taurus: Possession, Stubbornness.
  - Virgo: Discernment.
  - Libra: Peace at any price.
  - Capricorn: Authority, Responsibility, Ambition, Order.

  Most of these name the minority communities' own voices as the thin part.
- **Shortest sheets** (all still over 1,080 words): Leo/Joy (1,088), Capricorn/Merit (1,088), Libra/Reciprocity (1,095) and Capricorn/Discipline (1,099).
- **Generic sheets:** none found. Spot-checks of Aries/Identity, Sagittarius/Faith and Cancer/Care found specific Hunan pointers. Examples:
  - The Yao charter scrolls (过山榜 / 评皇券牒).
  - Laosicheng 老司城 and the Tujia hand-waving halls 摆手堂.
  - The Waxiang 瓦乡人 classification debate.
  - The Feishan 飞山 cult of Yang Zaisi.
  - The Dong Sa altars of Tongdao.
  - The Xinhuang 咚咚推 nuo drama.
  - Taoyuan's Uyghur and Hui township.
  - The Weishan Miyin Temple.
- **One small gap:** Sagittarius/Fundamentalism is the only sheet with no minority-language term in its search-terms table. The other 129 have one.

## Do the sheets exploit the nation's depth?
Yes, broadly. Here is how often each area appears across the 130 sheets:

- **Peoples:**
  - Tujia: 127.
  - Miao: 128.
  - Dong: 124.
  - Yao: 109.
  - Hui: 83.
  - Bai of Sangzhi: 36.
  - Taoyuan Uyghur community: 23.
- **Language varieties:**
  - Old Xiang (Loudi and Shaoyang): 96.
  - Southwestern Mandarin: 89.
  - Hakka: 66.
  - Gan of the eastern counties: 58.
  - Waxiang: 53.
  - Tuhua: 43.
- **Regions:**
  - Changsha: 130.
  - Xiangxi: 124.
  - Changde and Yiyang: 93.
  - Yueyang and Dongting: 81.
  - Xiangnan (Chenzhou and Yongzhou): 76.
  - Hengyang and Nanyue: 75.
  - Zhangjiajie and Sangzhi: 65.
  - Huaihua: 51.
- **Pre-modern and classical:**
  - Chu, the Chuci and Qu Yuan: 46.
  - Zeng Guofan and the Xiang Army: 40.
  - The Meishan 梅山 tradition: 30.
  - Yuelu Academy: 30.
  - Mawangdui: 24.
  - Wang Fuzhi: 19.
  - The Liye and Yuelu Qin slips, and the Zoumalou Wu slips.
- **Nüshu of Jiangyong:** 51.
- **Local gazetteers:** 66.

**Weak spots:**
- **Minority languages in Chinese characters:** most Tujia, Miao (Xong) and Dong terms are given as romanized or Chinese-character forms marked *check*. This is right for languages without a settled script, but a researcher will need the specialist dictionaries.
- **Provincial archives:** the Hunan Provincial Archives are named in only 6 sheets.
- **Huagu opera and nuo:** these performance traditions appear in only about 14 sheets each, so they may be under-used.
- **Diaspora:** pointers appear in 16 sheets, as comparison only.
