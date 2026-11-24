# Colorado springboard run: report (2026-11-24)

This run agent handled Colorado in Tuesday's wave 2, under the deeper brief (accuracy and depth first). It used one sub-agent per sign, Aries to Pisces, one after another. Nothing in the sheets has been verified, and every named item is marked *check*.

## Result
- **130/130 sheets done** across the 12 signs, written by 12 sign agents, with **0 relaunches**.
- **Whole-nation QA (`springboard_qa.py Colorado`):** 130 sheets scanned, 19 flags. All 19 are false positives of the "Indian" check: published titles and organizations' own names, each kept as published in quotation marks (see Rules below). There are no other flags.
- **Repeat check across the nation** (the run agent's own scripts):
  - Exact repeats: **0**. The check covered every non-template line of 40 characters or more, every table row, "Who to compare" bullet, Flags line (Held lines included) and first query.
  - Near matches at a ratio of 0.85 or above (compare bullets, Flags lines, first queries): **0** after the fixes listed below. Eleven were found during the run and fixed by the smallest edit.
  - Compare bullets for the same group at a ratio of 0.70 or above: 5 pairs remain. Each pair shares a frame but checks something different for its concept, so they were kept. The pairs are military families (Aries Recklessness / Pisces Escapism; Cancer Abandonment / Scorpio Secrecy), beet growers (Virgo Analysis / Sagittarius Honesty), the Ute cultural departments (Libra Partnership / Sagittarius Belief) and Saturday schools (Sagittarius Education / Pisces Dissolution).
- **Sub-agent tokens: 2,462,728** (514 tool uses), an average of 205,227 per sign. The main session adds the run agent's own tokens.
- **Wall clock:** the run started at 10:08 MST. The first launch was at 10:09 and the last return at 13:19, and the run ended at 13:23. The final Run log line was stamped 13:36 by mistake; the true end is 13:23.
  - There was no harness hand-back mid-sign and no HTTP 429 stop.
  - Signs took 13 to 17.5 minutes each.
- **Words by `wc -w`:** average 1,205, range 1,074 to 1,291, none over 1,300. 75 sheets run over 1,200.
- **Pointers per sheet:** 13 to 16, average 14.5 (1,886 in all).

## Per sign
| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers (avg) | Sub-agent tokens | Tools | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,234 | 1,282 Self-assertion | 1,147 Recklessness | 14-16 (15.2) | 175,634 | 45 | 10:09-10:23 |
| 2 | Taurus | 11 | 1,223 | 1,284 Ownership | 1,191 Domain | 14-15 (14.1) | 193,408 | 46 | 10:25-10:38 |
| 3 | Gemini | 10 | 1,210 | 1,251 Connection | 1,151 Domain | 14-16 (14.9) | 187,698 | 37 | 10:40-10:52 |
| 4 | Cancer | 10 | 1,240 | 1,271 Family | 1,207 Motherhood | 14-15 (14.3) | 212,214 | 41 | 10:53-11:08 |
| 5 | Leo | 13 | 1,146 | 1,218 Creativity | 1,097 Generosity | 14-15 (14.1) | 219,971 | 49 | 11:09-11:26 |
| 6 | Virgo | 10 | 1,196 | 1,279 Work | 1,156 Perfectionism | 15 (15.0) | 199,287 | 39 | 11:27-11:41 |
| 7 | Libra | 11 | 1,202 | 1,260 Justice | 1,133 Indecision | 13-15 (14.5) | 232,261 | 45 | 11:42-11:59 |
| 8 | Scorpio | 11 | 1,196 | 1,233 Domain | 1,156 Power | 14-15 (14.5) | 216,080 | 43 | 12:00-12:16 |
| 9 | Sagittarius | 11 | 1,255 | 1,291 Faith | 1,213 Meaning | 13-16 (14.5) | 206,671 | 43 | 12:17-12:33 |
| 10 | Capricorn | 10 | 1,192 | 1,277 Duty | 1,127 Discipline | 14-15 (14.4) | 194,086 | 40 | 12:34-12:46 |
| 11 | Aquarius | 10 | 1,161 | 1,263 Domain | 1,074 Friendship | 13-15 (13.9) | 204,706 | 39 | 12:47-13:01 |
| 12 | Pisces | 12 | 1,208 | 1,266 Domain | 1,148 Intuition | 14-15 (14.8) | 220,712 | 47 | 13:02-13:19 |

(The word counts above include the run agent's later edits. The Run log lines give the counts as they stood when each line was written, so a few differ by a word or two.)

## Rules, breaks and fixes
- **Lands:** the tracker lists no settled lands, and there is no `00 - Scope.md`. The pre-war lands carried are the USA.
  - Each sign's Domain sheet carries the note once, in its Flags, and no other sheet repeats it.
  - No sheet names or points to a scope file. There is no unit list and no border is settled.
  - The neighboring Mountain West (Wyoming, Utah, northern New Mexico, the Four Corners) appears only as comparison. So do the Diné and the Pueblo peoples beyond Colorado, Mesa Verde (named as Pueblo heritage), and the separate culture-nations (México, Sonora, the Prairie Federation, the Demilitarized Zone and others).
- **"Indian" (19 QA flags, all false positives):** these are published titles and organizations' own names, kept as published and in quotation marks:
  - the "Ute Indian Museum" (6 times)
  - the "Southern Ute Indian Tribe" and the joint Environmental Commission's name
  - the 1865 report "Massacre of Cheyenne Indians"
  - the "Colorado Ute Indian Water Rights Settlement Act" (1988)
  - Virginia McConnell Simmons, "The Ute Indians of Utah, Colorado, and New Mexico"
  - Richard K. Young, "The Ute Indians of Colorado in the Twentieth Century"
  - Grinnell, "The Cheyenne Indians"
  - the "Southern Ute Indian Montessori Academy"
  - the "Teller Indian School" and the "Fort Lewis Indian School" records

  In Libra, the run agent added quotation marks to four names that had been left unquoted, and from Scorpio on the prompt required them. The scan still lists quoted names, because it exempts only italics and a fixed list.

  Aries Beginning cites Elliott West's *The Contested Plains: Indians, Goldseekers, and the Rush to Colorado* in italics, and the scan passes it.

  Cancer Home names the Montrose museum by description instead of by its title. That is a judgment call; see below.
- **South Asian rule:**
  - The QA pattern found 0 hits.
  - After every sign, the run agent scanned the sheets for South Asian and Buddhist names, terms and institutions, including Boulder's contemplative institutions. Every scan was clean.
  - The category is held on 11 sheets, as a category only: Gemini Domain, Cancer Belonging, Virgo Analysis, Discernment and Health, Sagittarius Domain and Education, Capricorn Ambition, Aquarius Friendship, Pisces Domain and Spirituality.
  - Pisces Domain's wording ("South Asian religious institutions") differs slightly from the brief's phrase but stays at category level.
- **Buddhism (the author's open question):** it is held as a category only on 31 sheets, with no community, temple, school, retreat center or text named.
  - Aries: Autonomy, Beginning.
  - Taurus: Possession, Self-worth, Values, Stability, Sensuality.
  - Cancer: Domain.
  - Leo: Domain, Generosity, Joy.
  - Virgo: Domain, Service, Discernment, Health.
  - Libra: Balance, Reciprocity.
  - Scorpio: Death, Rebirth.
  - Sagittarius: Domain, Faith, Belief, Education.
  - Capricorn: Discipline.
  - Aquarius: Idealism, Nonconformity, Detachment.
  - Pisces: Domain, Compassion, Dissolution, Spirituality.

  Taurus held it on 5 sheets in what read like routine lines. From Gemini on, the prompt allowed the hold only where a real pointer had been set aside.

  The count stays high because Colorado (Boulder in particular) has many Buddhist and Buddhist-inspired bodies that a sheet would otherwise point to. See the judgment calls.
- **Universals, Hermes_research, zodiac words, the "indo-" catch:** none in any sheet.
- **Law:** Libra keeps to the letter (the 1863 and 1868 treaties and the Brunot Agreement as texts, statutes, settlement acts, acequia bylaws, decrees). Capricorn keeps to the spirit. Pisces Crime is kept to wrongdoing as a moral and social category. Other signs point legal questions to Libra or Capricorn.
- **Contested ground:** Sand Creek, the Ute removal and White River (1879), the land grants and the Taylor Ranch case, prior appropriation, Amache, Ludlow and the uranium towns are presented as accounts, with descendants' and tribes' own tellings set beside official records.
- **Stereotypes:** no compare bullet states a trait of a group. The bullets say what to check.
- **Run-agent smallest edits (no relaunch was needed):**
  - **Held lines.** Each of these was edited down to the category only or given sheet-specific wording:
    - Aries Beginning: it described the set-aside item, a New Year event at a religious site. Cut to the category.
    - Scorpio Death: a word-for-word copy of Leo Domain's Buddhism hold. Reworded for this sheet.
    - Cancer Belonging and Libra Reciprocity: near copies of other sheets' category-only holds. Given facet-specific wording.
  - **Compare bullets.** These were given concept-specific checks because they were close to bullets on other sheets:
    - Aries Independence (twice: the Volga German bullet and the Japanese American bullet)
    - Taurus Wealth
    - Gemini Connection
    - Leo Joy
    - Pisces Surrender
    - Virgo Domain and Health, which were bare "comparison only." bullets
  - **First queries.** These were given concept-specific terms because they repeated a catalog search from an earlier sheet:
    - Virgo Discernment
    - Scorpio Purging
    - Capricorn Duty (queries 3 and 4)
    - Aquarius Detachment

  From Taurus on, the prompt gained rules for each of these patterns, so the edits per sign fell to one or two.

## Thin, repetitive or generic sheets
- **Shortest and thinnest:**
  - Aquarius Friendship (1,074 words, 13 pointers)
  - Aquarius Detachment and Aquarius Domain (13 pointers each)
  - Libra Indecision (1,133 words)
  - Leo Generosity (1,097 words)

  Leo as a whole is the shortest sign (average 1,146). None of these reads as padded or generic.
- **Most-used pointers:** Amache material appears in the pointer tables of **64 sheets**: the National Historic Site, the preservation society, camp records and the camp newspaper. Other frequent pointers are History Colorado (28 sheets), the Denver Public Library collections (22), Colorado Historic Newspapers (21) and the Hermandad sources (15).

  These are the nation's core holdings, and each row gives its own reason, but Amache in particular is leaned on. The later research should not let it stand in for Japanese American life outside the camp years.
- **Groups and places that are thin across the nation**, counted as the sheets that mention them:
  - Chinese Denver and Hop Alley: 14
  - the Four Corners and Mesa Verde: 12
  - the Arkansas Valley by name: 18
  - Bent's Fort: 17
  - acequias and the People's Ditch: 28
  - the Hermandad and its *moradas*: 33
  - the Northern Ute's Colorado history (White River): 37
  - South Park and North Park: 39

## Coverage
The table counts the sheets (out of 130) that mention each region or people, by a simple text match, so a few counts run low.

| Region or people | Sheets |
|---|---|
| Nuche / Ute (any) | 129 |
| San Luis Valley / Hispanos | 128 |
| Korean | 126 |
| Ethiopian / Eritrean | 125 |
| Vietnamese | 124 |
| Somali | 119 |
| Aurora | 118 |
| Japanese Americans / Amache | 112 |
| Colorado Springs (evangelical, military) | 107 |
| Tsėhésenėstsestȯtse (Cheyenne) | 105 |
| Southern Ute / Ignacio | 101 |
| Hinóno'éí (Arapaho) | 100 |
| Volga Germans | 91 |
| Ute Mountain Ute / Towaoc | 89 |
| Central American communities | 87 |
| Black Coloradans (Five Points, Dearfield) | 75 |
| Ranching families | 75 |
| Pueblo (city) | 75 |
| Chicano / Mexican American | 68 |
| Mining and ski towns | 68 |
| Boulder | 68 |
| Western Slope / Grand Junction / North Fork | 65 |
| Eastern Plains | 62 |
| Sand Creek | 51 |
| Latter-day Saints | 47 |
| Land grants (Sangre de Cristo, Conejos) | 42 |
| South Park / North Park | 39 |
| Northern Ute / White River | 37 |
| Hermandad / moradas | 33 |
| Acequias / People's Ditch | 28 |
| Territorial newspapers | 28 |
| Ludlow | 25 |
| Arkansas Valley | 18 |
| Bent's Fort | 17 |
| Chinese Denver | 14 |
| Four Corners / Mesa Verde | 12 |

**Do the sheets use the nation's depth?** Mostly, yes.
- The sheets use the Indigenous peoples' own names and terms in Núuchi-u, Hinóno'éitíít and Tsėhésenėstsestȯtse (marked *check* where unsure), *manito* Spanish beside Mexican and Central American Spanish, Volga German, Amache-generation Japanese, Amharic, Tigrinya, Somali, Korean and Vietnamese.
- Nearly every sheet carries an early pointer: the treaties, the land grants, Bent's Fort, the Hermandad, the Sand Creek testimony, the Doris Duke oral histories, the Ute ethnographies or the territorial papers.
  - Several sheets get there only through a Ute history or ethnography (for example Taurus Security, Scorpio Power, Leo Play).
  - Pisces Escapism has nothing older than the 1890s, the weakest sheet on this count.
- The newer Aurora communities are present in almost every sheet.
- The weaker side is the older, smaller strands. The acequia culture, Chinese Denver, the Arkansas Valley, Bent's Fort and North Park appear in a minority of sheets.

## Judgment calls for the author
1. **Lands:** Colorado's lands are unsettled. It is for the author to decide how far it reaches into Wyoming, Utah, northern New Mexico and the Four Corners, and where it ends against the Prairie Federation, Sonora and the Demilitarized Zone. The sheets treat all of these only as comparison.
2. **Buddhism:** it is held as a category on 31 sheets, a high count driven by Boulder's Buddhist and Buddhist-inspired institutions and the Japanese American temples. When Buddhism is ruled on, these sheets need a pass.
3. **South Asian holds:** there are 11 category holds. The rule covers the universities', labs' and tech firms' South Asian-heritage scholars as well.
4. **Published names containing "Indian":** the run keeps them as published, in quotation marks (19 QA flags). Cancer Home instead names the Montrose museum by description. Please confirm which you prefer: the description, or the published name in quotation marks.
5. **Amache weight:** Amache appears in 64 sheets. Do you want later research to rebalance it toward Japanese American life before and after the camp years (Denver's Sakura Square, the Arkansas Valley farms)?
6. **Contested accounts:** Sand Creek, the Ute removal, Taylor Ranch, prior appropriation, Ludlow, Amache and the uranium towns are framed as accounts. Please confirm that the framing reads right to you.
7. **Pointer names reused with new reasons:** some pointers recur across signs with a different reason each time (the Hine beet-field photographs, the Centennial Farms program, the Larimer County "Code of the West", the Doris Duke oral histories), and the first queries were made distinct. Please confirm that this is acceptable.
