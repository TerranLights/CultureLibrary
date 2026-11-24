# Midwest Republic: springboard run report (2026-11-24)

Run agent, deeper brief, one sub-agent per sign (Aries to Pisces), one at a time. Wall clock: **10:08 to 14:03 MST**. Sheets: **130/130 done** (`springboard_status.py`). Whole-nation QA: **5 flags, all false positives** (published titles containing "Indian", kept as published in quotation marks; see below). No usage-limit stop and no forced hand-back.

## Per-sign table

Words by `wc -w` after the run agent's edits; pointers counted from the "Where to look first" tables.

| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers | Sub-agent tokens | Tools | Time | Relaunches | QA |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,205 | 1,293 (Domain) | 1,087 (Competition) | 14-16 | 206,932 | 46 | 10:09-10:27 | 0 | 0 |
| 2 | Taurus | 11 | 1,238 | 1,270 (Values) | 1,186 (Possessiveness) | 14-15 | 220,780 | 43 | 10:28-10:45 | 0 | 0 |
| 3 | Gemini | 10 | 1,240 | 1,275 (Domain) | 1,181 (Mediation) | 14-15 | 228,275 | 41 | 10:47-11:05 | 0 | 3 false positives |
| 4 | Cancer | 10 | 1,204 | 1,272 (Home) | 1,145 (Shelter) | 14-15 | 218,419 | 43 | 11:06-11:22 | 0 | 0 |
| 5 | Leo | 13 | 1,173 | 1,287 (Domain) | 1,095 (Leadership) | 13-15 | 235,061 | 53 | 11:23-11:41 | 0 | 0 |
| 6 | Virgo | 10 | 1,237 | 1,276 (Work) | 1,198 (Criticism) | 14-15 | 208,828 | 46 | 11:43-11:58 | 0 | 0 |
| 7 | Libra | 11 | 1,210 | 1,284 (Domain) | 1,161 (Diplomacy) | 14-16 | 209,174 + 69,802 | 42 + 10 | 12:01-12:13; relaunch 13:08-13:09 | 1 (Impartiality) | 0 |
| 8 | Scorpio | 11 | 1,197 | 1,239 (Death) | 1,151 (Secrecy) | 14 | 217,221 | 42 | 12:15-12:31 | 0 | 0 |
| 9 | Sagittarius | 11 | 1,245 | 1,282 (Faith) | 1,194 (Domain) | 14-16 | 207,273 | 42 | 12:33-12:48 | 0 | 0 |
| 10 | Capricorn | 10 | 1,244 | 1,273 (Order) | 1,179 (Discipline) | 13-15 | 207,554 | 41 | 12:50-13:05 | 0 | 0 |
| 11 | Aquarius | 10 | 1,251 | 1,289 (Domain) | 1,190 (Nonconformity) | 13-15 | 224,566 | 43 | 13:08-13:25 | 0 | 1 false positive |
| 12 | Pisces | 12 | 1,234 | 1,272 (Boundary) | 1,185 (Escapism) | 14-15 | 245,127 | 48 | 13:27-13:48 | 0 | 1 false positive |
| | **Nation** | **130** | **1,223** | 1,293 | 1,087 | 13-16 | **2,699,012** | 540 | 10:09-13:48 | 1 | 5 false positives |

Pointers per sheet across the nation: 13 on 4 sheets, 14 on 63, 15 on 57, 16 on 6. The run agent's own tokens are not counted above.

## Rule breaks and fixes

- **South Asian rule, named scholar (1):** Libra Impartiality named a 2004 résumé-audit field experiment by its authors, one of them a scholar of South Asian heritage. My name sweep caught it after Capricorn. The sheet was relaunched as a single-concept job: the pointer was replaced by a Minnesota judicial-speech case and the item is held as a category only. No other South Asian-heritage scholar, work, community or religion is named in any sheet. A dictionary-filtered sweep of every capitalized word in the pointer columns found only Somali, Arab American and other non-South-Asian names.
- **South Asian rule, held items described too closely (10 Held lines, smallest edits):** some Held lines tied the held category to an event (the 1893 Parliament), a vote (one city's 2024 vote), a place, or the held study's subject (public housing, an urban ethnography, unwritten codes, mobility atlases, business ownership, third-party mediation, unequal treatment, neighborhood measures). Each was cut to the bare category. The sheets are Sagittarius Domain and Conviction, Capricorn Ambition and Law, Aquarius Community and Equality, Aries Initiative, Gemini Mediation, Cancer Shelter and Leo Honor. Cancer Domain also got a place cut.
- **Routine mention of the South Asian and Buddhist rules (15 Held lines, smallest edits):** in Gemini (5) and Leo (10), Held lines added clauses like "nothing fell under the South Asian (or Buddhist) rule" where nothing was held. The clause was cut, so each line keeps only its concept-specific content. From Virgo on, the prompt asked for this.
- **The 1830 act under its popular name (1):** Sagittarius Freedom used the popular name. It was changed to the published title, in quotation marks.
- **Copied table row (1):** Hmong *ntsej muag* had the same row in Taurus Self-worth and Leo Honor. Leo's gloss and note were made specific to honor and kept neutral.
- **Near repeats (smallest edits):**
  - Taurus: three South Asian Held lines on one frame (Domain, Values, Wealth). Each was reworded for its own concept.
  - Two first queries were reworded to name their concept's question: the Amana 1932 reorganization query (Scorpio Control vs Taurus Stability) and the Illinois Attorney General's 2023 report query (Scorpio Betrayal vs Libra Peace at any price).
  - A generic Native-nations compare bullet (Scorpio Domain vs Gemini Domain) was made specific to the domain.
  - A Buddhism/South Asian Held line (Sagittarius Domain) was too close to an Appalachia Pisces line and was reworded.
- **Final repeat check across the nation and against Appalachia's 130 sheets:** 0 exact repeats (lines over 30 characters, table rows, compare bullets, Flags lines, first queries; the search-term table header is excluded). 0 near matches at 0.85 among compare bullets, Flags lines and first queries. At 0.80 the remaining pairs are different queries to the same archive (Harold Washington collections; *Hmong Studies Journal*) and were kept.
- **QA false positives kept (5):** "Indian" appears only in published titles in quotation marks:
  - Eastman, "Indian Boyhood" (Gemini Learning)
  - Sleeper-Smith, "Indian Women and French Men" (Gemini Connection)
  - Rafert, "The Miami Indians of Indiana" (Gemini Duality)
  - Deloria, "Speaking of Indians" (Aquarius Friendship)
  - the 1830 act's published title (Pisces Surrender)

  Virgo's titles (Densmore, Kappler, the 2022/2024 boarding-school report, GLIFWC's own name) use italics plus quotation marks and pass the scan.
- **Lands:** the note that the lands are still to be settled appears only in the 12 Domain sheets' Flags. No sheet tells the reader to read a scope file, no sheet adds a unit list, and nothing comes from `Hermes_research`. The Census Bureau's Midwest region appears only as the Bureau's own definition, used to pull tables.
- **Law:** Libra keeps to the letter of the law and Capricorn to its spirit. Elsewhere, law pointers were passed to Libra or Capricorn, often on the Held line.

## Thin, repetitive or generic sheets

- **Shortest:** Leo Leadership (1,095), Aries Competition (1,087), Leo Dignity (1,106), Leo Generosity (1,118), Aries Independence (1,118), Cancer Shelter (1,145). Not thin in substance (14 to 15 pointers each), but the leanest of the nation.
- **Lowest pointer counts (13):** Leo Honor, Capricorn Domain, Capricorn Merit, Aquarius Domain.
- **Held lines on one sentence frame:** in Libra, all 11 Held lines read "X studies were weighed and left out; their samples are not Midwestern". Each names a different study type, and they were kept. After Libra the prompt asked for varied frames, and Scorpio to Pisces vary.
- **Generic in places:**
  - Libra's Held lines and some of Libra's experimental-game pointers lean on national or lab literature, which the sheets themselves flag as lacking Midwestern samples.
  - Aquarius Domain sets national civic-life studies aside as too coarse.
- **The same groups on almost every sheet:** Dearborn (128 of 130 sheets), Hmong (126), Polish (125), Anishinaabeg/Ojibwe (121), Somali (120), Mexican (114), Amish (111) and Dutch (110). That spread follows the brief, but a researcher may find the compare sections of different concepts look alike in whom they name. The bullets themselves are not copied: each names a concept-specific check.

## Pointers per sheet and use of the nation's depth

- Pointers: 13 to 16 per sheet, 1,885 in all, with search terms in Midwestern English and the region's community and Native languages (Pennsylvania Dutch, German, Polish, Czech, Norwegian, Swedish, Finnish, Dutch, Spanish, Arabic, Hmong, Somali, Anishinaabemowin, Dakota, Ho-Chunk, Menominee, Meskwaki). Each is marked *check* where unsure.
- Pre-modern pointers appear throughout: the *Jesuit Relations* (12 sheets), Black Hawk's *Life* (14), treaty records, French colonial Detroit and Kaskaskia, the Northwest Ordinance, Cahokia, county histories, Hull-House, and Moravian and Harmony Society papers.
- **Depth is used well for:**
  - Native nations: Dakota on 88 sheets, Ho-Chunk 70, Menominee 64, Meskwaki 48, Potawatomi 36, Myaamia 32, Oneida 27, Shawnee 24, Odawa 16.
  - Plain communities: Amish on 111 sheets, Mennonite 75.
  - Upper Midwest Nordic communities: Norwegian 86, Finnish 79, Swedish 63.
  - Chaldeans (68), Bosnians of St. Louis (47), the Upper Peninsula (56) and the Iron Range (47).
- **Less used:** the Red River Valley (5 sheets), the Driftless Area (11), Kansas City (23), Cleveland (24), Irish-descended (23) and Italian-descended (26) Midwesterners, and the Odawa (16). Out-migrant Appalachians appear in 24 sheets, as Midwesterners where they live.

## Judgment calls for the author

1. **Lands.** Kansas City and St. Louis, southern Illinois and Indiana (Upland South settlement), Appalachian Ohio and the Red River Valley (shared with the Plains) sit at edges that are yours to settle. The sheets point to the Appalachian, Prairie Federation and CSA sides only as comparison. Utopias outside the core (the Oneida Community of New York, the Hutterite colonies of the Plains) were left to the nations whose lands hold them.
2. **A South Asian-heritage dataset in the concept block itself.** Capricorn Ambition's concept block names two mobility atlases led by a scholar of South Asian heritage, so every nation's run will meet them. You may want to rule on the avenue file. The same 2004 field experiment (Libra Impartiality) is a well-known pointer that other nations' sheets may also name.
3. **South Asian category held on 19 sheets:**
   - Aries: Domain, Initiative
   - Taurus: Domain, Values, Wealth
   - Gemini: Mediation
   - Cancer: Domain, Shelter
   - Leo: Domain, Honor
   - Libra: Impartiality
   - Sagittarius: Domain, Conviction
   - Capricorn: Ambition, Law
   - Aquarius: Community, Equality
   - Pisces: Spirituality, Crime

   Each is now worded as a category only.
4. **Buddhism held as a category on 7 sheets:** Aries Domain, Taurus Possession, Leo Domain, Sagittarius Domain, Capricorn Discipline, Aquarius Detachment and Pisces Spirituality. These are mostly Southeast Asian-heritage refugee communities' practice and urban meditation teaching. No community, temple or text is named.
5. **Kept with cautions on the Held lines:**
   - Ella Deloria's account (from Dakota communities farther west) kept, with its fit to Minnesota's Dakota left for the researcher to judge.
   - The Serenity Prayer's attribution, held until checked.
   - The 2020 Minneapolis protests, held for a pass built on local archives.
   - Somali clan bodies, kept out until community sources say whether and how they wish to be studied.
   - Dearborn informant cases and the 2001 Minneapolis remittance-office closures, kept back as contested accounts.
6. **Contested ground** is presented as accounts throughout: 1862 and Mankato, the 1830s removals, Detroit 1967, redlining in Chicago and Milwaukee, the Rust Belt account and the Dearborn debates.
