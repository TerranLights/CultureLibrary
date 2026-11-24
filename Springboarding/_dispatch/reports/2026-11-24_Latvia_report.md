# Latvia springboard run: report (2026-11-24)

**Result:** 130/130 sheets `done` by `springboard_status.py`; whole-nation QA (`springboard_qa.py Latvia`) **130 sheets scanned, 0 problems**. 12 sign agents, 0 relaunches, run-agent smallest edits in two places (below). Wall clock **05:04 to 08:35 MST** (no usage-limit stop). Sub-agent tokens **2,770,641** (683 tool uses), not counting the run agent.

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Shortest | Pointers (range, avg) | Sub-agent tokens | Minutes |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,153 | 1,279 (Domain) | 1,068 (Competition) | 14-16, 15.0 | 178,342 | 14.4 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,213 | 1,297 (Ownership) | 1,150 (Stubbornness) | 14-15, 14.8 | 215,030 | 15.9 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 1,205 | 1,288 (Domain) | 1,172 (Curiosity) | 14-16, 14.7 | 205,050 | 12.7 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,209 | 1,270 (Home) | 1,164 (Protection) | 14-16, 14.9 | 226,024 | 13.9 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,191 | 1,274 (Domain) | 1,096 (Play) | 14-15, 14.4 | 220,257 | 16.7 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,207 | 1,261 (Domain) | 1,122 (Perfectionism) | 13-15, 13.9 | 227,893 | 15.0 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,247 | 1,268 (Indecision) | 1,206 (Reciprocity) | 13-14, 13.7 | 236,733 | 17.5 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,233 | 1,284 (Domain) | 1,199 (Trust) | 14-15, 14.3 | 213,320 | 15.2 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 1,204 | 1,286 (Domain) | 1,156 (Conviction) | 13-15, 13.7 | 255,299 | 18.4 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1,154 | 1,270 (Domain) | 1,091 (Merit) | 13-14, 13.4 | 257,048 | 20.2 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1,230 | 1,271 (Community) | 1,139 (Detachment) | 13-14, 13.8 | 240,690 | 17.3 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,211 | 1,296 (Domain) | 1,121 (Intuition) | 12-14, 13.2 | 294,955 | 24.6 |
| | **All** | **130** | **12** | **0** | **0** | **1,205** | **1,297** | **1,068** | **12-16, 14.2** | **2,770,641** | |

Word counts by `wc -w` after the edits below; none over 1,300 (five sheets between 1,284 and 1,297).

## Rule breaks and fixes
- **Leo, 11 identical bare `Held for review: none.` lines** (Self-expression through Joy): fixed by run-agent smallest edits, each now giving a reason specific to its sheet. From Virgo on, every sub-agent prompt asked for a sheet-specific Held line; none repeated afterwards.
- **Two Domain-sheet lands notes copied word for word between signs** (Taurus = Gemini; Capricorn = Aquarius), found by the whole-nation check: the Gemini and Aquarius sentences reworded by hand.
- **Whole-nation repeat check after the fixes:** 0 exact repeated lines, table rows, "Who to compare" bullets, Flags lines (short Held lines included) or first queries. The shared 10-word runs that remain are the "Language(s) for searching" header field (lists of language names), short bullet openings that name the same group before differing ("the Livonian Coast and the Suiti: check ..."), the phrase "present each account as an account" from the contested-ground rule, and similar wording in four Domain sheets' lands notes (Aries, Taurus, Cancer, Leo: "exact lands in the post-war order are still to be settled"; the sentences are not identical). Kept.
- **No false positives** from the QA scan for this nation; no zodiac words, no URLs, no "Indian", no universals, no Hermes.
- An early completion notice for the Aries agent arrived before any Aries file existed; it was ignored and no duplicate agent was launched (the real completion came about 14 minutes later).

## Holds (South Asian rule and Buddhism)
- South Asian category held, each a real set-aside and category only: Sagittarius Domain (communities and religious bodies of South Asian origin in the official register), Sagittarius Education (South Asian-heritage students and staff, in place of a foreign-students pointer), Sagittarius Fundamentalism (bodies of South Asian origin turned up by "sect" coverage), Pisces Spirituality (heritage communities and their religious movements).
- Buddhism held as a category, none named: Sagittarius Domain, Sagittarius Fundamentalism, Aquarius Detachment (meditation and retreat practice), Pisces Spirituality (meditation communities).
- Name scans of every pointer cell after each sign found no South Asian scholar, writer, work, community or religion and no Buddhist body named outside these Held lines.

## Thin, repetitive or generic sheets
- **Pointer counts slide in the late signs:** Capricorn (13.4 avg), Pisces (13.2; Dissolution at the floor of 12) against 14.7 to 15.0 in the first four signs. The Capricorn agent said many obvious sources were already used and reused two (Zolitūde in Responsibility, the 1920 land reform in Hierarchy) in new rows with new angles.
- **Source reuse across the nation:** 77 pointer lead names appear in more than one sheet, almost all twice, each time in a newly written row with a concept-specific reason. The most-used: the Central Statistical Bureau (6 sheets, mostly Domain sheets), Ernst Glück's Bible (4), Merkel's *Die Letten*, the *Livonian Rhymed Chronicle*, *Lāčplēsis*, Kalniete's memoir, the European Values Study, the Office of Citizenship and Migration Affairs and *Baigais gads* (3 each). No sign leans on the same few sources throughout.
- **Thinnest-looking sheets** (shortest, fewest pointers; still not generic): Aries Competition (1,068), Capricorn Merit (1,091), Leo Play (1,096), Pisces Dissolution (12 pointers), Pisces Intuition (1,121).
- No sheet reads generic: every sign has region-, minority- and period-specific pointers.

## Whether the sheets exploit Latvia's depth
Yes, broadly. Pre-modern pointers run through every sign (the *dainas* in Barons's and the academic editions, Henry of Livonia, the *Livonian Rhymed Chronicle*, Mancelius, Einhorn, Fürecker, Glück, Stender, Russow, the Riga guild *Schragen* and Small and Great Guild records, Courland's church order, the Swedish land revisions, the Calendar Riots, the 17th-century witch and werewolf trials). Internal regions appear across signs: Latgale (Rēzekne, Daugavpils, Aglona, Krāslava, Ludza), the Livonian Coast (Mazirbe, Košrags), the Suiti of Alsunga, Kurzeme ports (Liepāja, Karosta, Ventspils), Zemgale (Jelgava, Rundāle, Tērvete), Sēlija, Vidzeme and the Gauja valley, Jūrmala and Riga's districts (Moscow Suburb, Ķīpsala, Āgenskalns). Minorities beyond the best-known: Livonians, Suiti, Old Believers (Grebenshchikov community, Pomor church), Poles, Belarusians, Ukrainians since 2022, Lithuanians, Roma (Leksa Manušs, Roma mediators), the Jewish community (Dvinsk rabbis, Bund, *Frimorgn*, Rumbula, Žanis Lipke), Dievturi, Moravian Brethren, Baptists and Pentecostals. Search terms carry Latgalian, Livonian, Russian, Polish, Yiddish and some Romani. Fewer pointers in the later signs is the main limit.

## Judgment calls for the author
1. **Lands:** no `00 - Scope.md` and no settled lands; every sheet is written for Latvia as it stands, with one lands note per Domain sheet (one per sign) and none in the concept sheets.
2. **The holds above** (four South Asian category holds in Sagittarius and Pisces; four Buddhism holds): confirm they stay as categories.
3. **Contested items kept as accounts:** the fire cross (*ugunskrusts*) in Cancer Protection (flagged as a contested symbol); 9 May, 16 March and Riga Pride in Leo Pride; the *Kononov v. Latvia* judgment in Libra Justice; the 2014 Liepāja musical about Herberts Cukurs in Scorpio Betrayal; the Konrāds Kalējs case in Capricorn Law; the KGB card files in several sheets (with a caution never to name a person as an informer from unchecked lists).
4. **Possibly sensitive search terms kept:** Libra Projection uses the regional nickname *čangalis* as a search term for research on stereotypes of Latgalians; Aquarius Detachment lists the "Latvian potato" internet meme as a meme and the responses to it, never as a trait. Both are framed as objects of study, not claims; remove them if you'd rather not have them in the sheets.
5. **Law placement:** law as written appears only in Libra, legal culture only in Capricorn; Capricorn Authority's pointer to the 1998 Child Protection Law's ban on physical punishment is used for the spirit (norms of discipline), not the letter.
