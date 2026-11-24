# Appalachia: springboard run report (2026-11-23)

Run agent for Appalachia, deeper brief (accuracy and depth first). One sub-agent per sign, Aries to Pisces, in order. **130 of 130 sheets done** by `springboard_status.py`.

- **Wall clock:** 09:55 to 14:41 MST for the sheets and checks. The report was finished at 20:35, after a stall: the run agent stopped while the near-match check ran in the background, and the coordinator restarted it.
- **Interruptions:** the harness handed the run agent back once, at 13:41. That was not a usage limit; the run resumed at once. The Capricorn sub-agent was left running and no duplicate was launched. No HTTP 429.

## Per-sign table
Word counts are by `wc -w` after all fixes. Pointers are the rows in section 2. Tokens are sub-agent tokens.

| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers (avg) | Relaunches | Run-agent edits | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,195 | 1,286 Identity | 1,055 Competition | 13-16 (15.3) | 0 | 0 | 194,018 | 09:57-10:14 |
| 2 | Taurus | 11 | 1,174 | 1,296 Domain | 1,070 Possessiveness | 12-15 (13.5) | 0 | 11 Held lines (bare "none.") | 293,520 | 10:15-10:39 |
| 3 | Gemini | 10 | 1,268 | 1,298 Domain | 1,224 Information | 14-15 (14.6) | 0 | 0 | 198,418 | 10:41-10:56 |
| 4 | Cancer | 10 | 1,235 | 1,296 Domain | 1,148 Belonging | 13-16 (14.0) | 1 (Shelter, Held line) | 0 | 239,452 | 10:57-11:20 |
| 5 | Leo | 13 | 1,217 | 1,273 Domain | 1,165 Recognition | 14-16 (14.9) | 0 | 1 (Joy, denomination name) | 260,680 | 11:21-11:52 |
| 6 | Virgo | 10 | 1,235 | 1,279 Service | 1,125 Perfectionism | 13-16 (14.1) | 1 (Improvement, Held line) | 0 | 231,323 | 11:53-12:10 |
| 7 | Libra | 11 | 1,258 | 1,287 Reciprocity | 1,205 Indecision | 13-14 (13.5) | 0 | 0 | 245,416 | 12:11-12:28 |
| 8 | Scorpio | 11 | 1,249 | 1,295 Death | 1,187 Trust | 14-15 (14.4) | 1 (Trust, Held line) | 0 | 246,971 | 12:29-12:50 |
| 9 | Sagittarius | 11 | 1,272 | 1,294 Freedom | 1,195 Honesty | 12-14 (13.4) | 2 (Domain, Education: Held lines) | 0 | 268,234 | 12:51-13:14 |
| 10 | Capricorn | 10 | 1,236 | 1,286 Domain | 1,198 Merit | 12-14 (12.7) | 1 (Ambition, Held line) | 0 | 257,699 | 13:15-13:42 |
| 11 | Aquarius | 10 | 1,220 | 1,293 Group | 1,135 Friendship | 14-15 (14.6) | 2 (Friendship, Nonconformity: Held lines) | 0 | 210,568 | 13:43-13:56 |
| 12 | Pisces | 12 | 1,256 | 1,297 Compassion | 1,178 Intuition | 13-15 (14.3) | 2 (Compassion, Empathy: Held lines) | 0 | 280,926 | 13:56-14:21 |

**Totals:**
- **Sub-agent tokens:** 3,553,033 in all: 2,927,225 for the 12 sign agents and 625,808 for the 10 single-concept fix jobs (58,255 to 67,400 each). The run agent's own tokens are not counted here.
- **Words:** 1,234 on average across the nation (1,055 to 1,298). 102 sheets are over 1,200 words, 27 are over 1,280 and none is over 1,300.
- **Pointers per sheet:** 12 to 16, 14.1 on average. By sheet count: 12 pointers 8, 13 pointers 28, 14 pointers 44, 15 pointers 41, 16 pointers 9.

## QA, rule breaks and fixes
**Whole-nation QA (`springboard_qa.py Appalachia`):** 130 sheets, 2 hits, both false positives kept as published, in quotation marks:
- Cancer Care: the Eastern Band's own hospital name, "Cherokee Indian Hospital".
- Pisces Boundary: Charles C. Royce's published title, "Indian Land Cessions in the United States" (1899).

**South Asian rule: Held lines that identified what they held (10 sheets, all fixed by single-concept relaunch).** Several sub-agents correctly set a pointer aside, but then described it on the Held line closely enough to identify it. Examples:
- a refugee community in a named metro area;
- a congregation near a named city;
- memoirs placed by town and profession;
- county-level mobility and social-capital datasets "led by" a South Asian-heritage scholar.

These match the CSA precedent, where a mobility atlas on a Held line was relaunched. All ten Held lines now give only the brief's category, "South Asian-heritage communities in the nation's lands", each in its own concept-specific words. The ten sheets are Cancer Shelter, Virgo Improvement, Scorpio Trust, Sagittarius Domain and Education, Capricorn Ambition, Aquarius Friendship and Nonconformity, and Pisces Compassion and Empathy. Two of them (Pisces Compassion and Empathy) had also used categories of their own ("authors", "research led by scholars").

**Other South Asian checks:** the run agent's own name and term scan is clean across all 130 sheets. No South Asian scholar, writer, work, community, language or religion is named anywhere.

**Run-agent smallest edits:**
- **Taurus (11 sheets):** every Held line was a bare "none.", which repeated across the sign. Each was given concept-specific wording.
- **Leo Joy:** the sub-agent had avoided the denomination's own name, the Primitive Baptist Universalists, because the run agent's helper scan matched "universal". The name is restored. The helper scan now looks only for universals lists, and the prompt says a group's own name is fine. No sheet refers to Human Universals or any universals list.

**Other rules:**
- **Lands note:** once per Domain sheet, nowhere else. No unit list anywhere and no borders settled. The ARC county definition is named only as a source's definition.
- **Law:** Libra keeps to the letter of the law (county order books, statutes, federal mine-disaster prosecutions, the Cherokee Code and Cherokee Court opinions, broad form deeds). Capricorn keeps to the spirit. Other signs point law to Libra and Capricorn; Pisces Crime keeps to the moral and social side.
- **Banned terms and files:** no zodiac words, no Hermes, no "Indian" outside a published name.
- **Outside images:** every "hillbilly", feud or reality-TV image sits on a Sensitive line or in a source description and is named as an outside image or slur. No "Who to compare" bullet states a trait of a group. This was checked by hand.

## Repeat check
**Within the nation:** the run agent's exact check over all 130 sheets finds no repeated line, table row, "Who to compare" bullet, Flags line or first query. The section headings and the template's fixed lines are excluded. The same holds against the CSA's 130 sheets: nothing is copied from them.

**Near matches** (difflib ratio of 0.85 or more, run over sections 2 to 5 of Appalachia's 130 sheets plus the CSA's 130). The check finished at 14:41, and no sheet changed between then and the one fix below. It found 9 near matches and none against the CSA:
- **Cancer Home and Pisces Dissolution:** both carry a row for Katrina M. Powell's *The Anguish of Displacement* (2007), with the same "What it is" cell and different reasons. The run agent made a smallest edit at 20:34 and reworded the Dissolution cell. Dissolution is now 1,284 words.
- **Eight pairs among the ten fixed Held lines:** each pair shares the brief's set category phrase, "South Asian-heritage communities in the nation's lands", and its framing ("set aside under the standing rule ... only as a category"), but opens in its own concept-specific words. No two of these lines are identical. They are kept as written, because the category wording is prescribed.

**Sources that recur with their own reasons:** these are pointers, not copied rows. Examples are *Who Owns Appalachia?* (Ownership and Aquarius), Loyal Jones's *Appalachian Values* (Values), the Frank C. Brown Collection (different volumes), *Cherokee Women* and *The Budget*.

## Thin, repetitive or generic sheets
**Thinner (12 pointers, all real and concept-specific; spot-checked Merit):**
- Taurus: Self-worth, Possessiveness, Stubbornness.
- Capricorn: Authority, Merit, Law, Order.
- Sagittarius: Honesty.

**Shortest:** Aries Competition (1,055 words, 13 pointers) and Taurus Possessiveness (1,070 words).

**Repetitive:** none found. **Generic:** none found by spot-check.

**Running long:** most sheets run near the scan's 1,300-word ceiling, with the Gemini to Pisces averages at 1,217 to 1,272. That is above the brief's aim of about 1,000 and up to about 1,200, but under the flag.

## Does the run exploit the nation's depth?
Mostly yes. Sheets that name each group or source (of 130):
- **Native and Black Appalachia:** Cherokee 130 (with the syllabary or syllabary terms in 78); Black Appalachians or Affrilachian writers 103.
- **Northern and ethnic communities:** Pennsylvania German 124; Amish or Mennonite 119; Italian, Polish, Hungarian, Slovak, Rusyn or Welsh communities 114; Pittsburgh 102; Melungeons 73; Lebanese or Syrian families 44; New York's Southern Tier 27.
- **Latino newcomers:** Spanish or Latino terms in all 130.
- **Places:** Asheville or Knoxville 65; the Smokies 45; the Shenandoah 43; the Cumberland Plateau 16.
- **Pre-modern pointers:** church minutes 45; Moravian records 29; Child ballads or Jack tales 25; shape-note books 16; WPA life histories 15; county order books 9.

**A weakness the author should know about (the run agent's own doing):** from Taurus on, the prompt told sub-agents not to lean on the same few sources, and named the *Encyclopedia of Appalachia*, Foxfire and Appalshop as examples. The sub-agents then all but dropped these core regional works:
- the *Encyclopedia of Appalachia*: 1 sheet;
- Foxfire: 3 sheets;
- Appalshop: 3 sheets;
- the *Journal of Appalachian Studies* or the Appalachian Studies Association: 3 sheets.

Berea College's collections still appear in 26 sheets. The sheets are more varied for it, but a researcher should open the *Encyclopedia of Appalachia*, the *Journal of Appalachian Studies*, the Foxfire volumes and Appalshop's archive for nearly every concept, whether or not a sheet names them.

## Judgment calls for the author
1. **Lands and the CSA:** southern Appalachia's overlap with the CSA (east Tennessee, western North Carolina, north Georgia, north Alabama, and southwest Virginia) is open. The sheets write for the Appalachian region of the pre-war USA and settle no border. How far north (New York's Southern Tier, Appalachian Ohio) and south the nation reaches is the author's call.
2. **Buddhism:** held as a category, with nothing named, on three Held lines: Sagittarius Domain, Aquarius Detachment and Pisces Spirituality.
3. **South Asian holds:** ten sheets hold one real set-aside pointer each, as category only (listed above). Most are US mobility and social-capital datasets and memoirs by regional physicians and writers. The author may want to rule on whether those datasets can ever be used under another name.
4. **Titles containing "Indian":**
   - Gemini Duality gives Circe Sturm's 2011 book by author and search phrase rather than by its published title. That is allowed, but the author may prefer the title in quotation marks.
   - "Cherokee Indian Hospital" and Royce's "Indian Land Cessions" are kept as published.
5. **Out-migrants and other culture-nations:** out-migrants to Midwestern cities are comparison only throughout. The CSA, Midwest Republic and New England appear only as comparison.
