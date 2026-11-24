STATUS: done 2026-11-23. Run agent's report; the sheets are unverified.

# Austro-Bavaria: springboard run report (deeper brief)

**Result:** all 130 sheets are done. Every first line reads `STATUS: done 2026-11-23, not verified`. The run used 12 sign agents and **no relaunches**. The whole-nation QA (`springboard_qa.py Austro-Bavaria`) found **1 flag in 130 sheets, a false positive** (see below). Three small hand edits were made by the run agent.

**Tokens and wall-clock:**
- **Sub-agent tokens:** **2,688,288** as reported by the harness (12 sign agents, 641 tool uses). The run agent's own tokens are not included; the main session adds them.
- **Wall-clock:** the run agent started at **05:04:24 MST**. The Aries agent launched at 05:05 and the Pisces agent finished at 08:19. The report was written by about **08:25 MST**: about 3 h 20 min in all, with no usage-limit stop.
- **Time per sign:** 12.5 to 19.0 min, one sign at a time.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Shortest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,152 | 1,257 (Domain) | 1,059 (Initiative) | 15.2 (14-16) | 189,397 | 05:05-05:22 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,181 | 1,252 (Domain) | 1,107 (Possessiveness) | 15.1 (14-16) | 200,138 | 05:23-05:36 |
| 3 | Gemini | 10/10 | 1 | 0 | 1 (false positive) | 1,174 | 1,250 (Domain) | 1,087 (Mediation) | 14.7 (14-16) | 218,721 | 05:37-05:52 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,177 | 1,281 (Domain) | 1,122 (Belonging) | 14.8 (14-15) | 212,912 | 05:52-06:05 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,173 | 1,287 (Domain) | 1,085 (Leadership) | 14.8 (14-16) | 221,721 | 06:05-06:20 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,198 | 1,288 (Domain) | 1,133 (Improvement) | 14.7 (14-15) | 202,218 | 06:21-06:34 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,234 | 1,298 (Domain) | 1,200 (Partnership) | 13.9 (13-15) | 247,157 | 06:35-06:52 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,186 | 1,271 (Death) | 1,105 (Power) | 13.5 (13-15) | 253,040 | 06:53-07:12 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,234 | 1,284 (Domain) | 1,172 (Conviction) | 13.8 (13-14) | 240,974 | 07:12-07:30 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,237 | 1,291 (Domain) | 1,162 (Discipline) | 14.1 (14-15) | 214,725 | 07:31-07:44 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,211 | 1,289 (Group) | 1,105 (Hope) | 13.8 (13-15) | 227,523 | 07:45-08:00 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,210 | 1,260 (Fear) | 1,139 (Escapism) | 14.0 (14) | 259,762 | 08:00-08:19 |
| | **Total** | **130** | **12** | **0** | **1 (false positive)** | **1,197** | **1,298** | **1,059** | **14.4 (13-16)** | **2,688,288** | **05:05-08:19** |

- **Word counts:** by `wc -w`, markup included, after the hand edits. 57 sheets are between 1,200 and 1,298 words; none is over 1,300.
- **Pointers:** the rows of section 2. Every sheet has 13 to 16.

## Rule breaks and fixes
- **QA:** one flag in the whole nation, a false positive. Gemini/Learning gives the Romani verbs *sikhol* / *sikavel* ("to learn / to teach") as search terms, and the "sikh" pattern matches them. They are words of the nation's own Roma, so they are kept as written; add them to lesson 9's list. Nothing else was flagged in any sign: no banned divination words, no "Indian", no "Indo-", no URLs and no finding phrases.
- **Hand edits by the run agent** (each the smallest edit):
  1. **Aries Domain:** cut "No `00 - Scope.md` exists yet:" from the lands note. The lands note itself was kept. From Taurus on, the prompt said not to mention a scope file, and none did.
  2. **Cancer/Protection:** a Chechen-Austrian bullet asked about "guarding family members", which implied a trait. It now asks how community associations describe the protection they sought after flight.
  3. **Capricorn/Order:** a bullet tied courtyard-noise disputes to Turkish- and BCS-speaking families. It is now a check across long-settled and newer tenants of Vienna's outer districts.
- **Checkpoint slips (no action):** in Aries, the sub-agent reworded 10 Held lines after marking those sheets done. The files are complete. From Taurus on, the prompt said to reset STATUS before any late change. The Capricorn (Law, Order) and Aquarius (Nonconformity) sub-agents did that for their late fixes.
- **South Asian rule:**
  - 19 sheets carry a category-only Held line: 7 of the 11 Sagittarius sheets and all 12 Pisces sheets. Each is worded differently, and none names a community, religion or teacher.
  - The other 111 sheets read "none" plus a sheet-specific reason.
  - My own scan, wider than the QA pattern, found no South Asian name, work, religion or movement anywhere else. Its only hit was Turkish *gurur* ("pride"), which my pattern caught as "guru".
- **Lands note:** the note that Germany and Austria are read as Bavaria and Austria, with the exact lands still to be settled, is in each sign's Domain sheet (12 of 12) and in no other sheet. No unit list was added. Nothing came from Hermes_research.
- **Law:**
  - **Libra** has the letter of the law: the ABGB, Article 7, the *Höfegesetz*, court files and codes.
  - **Capricorn** has the spirit, and its Law sheet was checked by hand. It covers the Twelve Articles, Joseph II's letter to officials, Ehrlich against Kelsen, trust in justice, *Kirchenasyl*, *Pfusch* and folk outlaws.
  - The other signs point legal sides to Libra and Capricorn. Scorpio, Sagittarius, Aquarius and Pisces cite no statutes or rulings, and Pisces/Crime stays on wrongdoing as a moral and social category.
- **Universals:** no sheet mentions Brown, *Human Universals* or any universals list.

## Repetition
- **Lines:** no line of 40 characters or more repeats anywhere in the 130 sheets. That covers table rows, "Who to compare" bullets, Flags lines (including Languages needed and Held for review) and first queries, but not the template's fixed lines.
- **Pointer cells:** no named pointer is used on more than 3 sheets. Three are used on 3 sheets each: Innerhofer's *Schöne Tage*, Hohberg's *Georgica curiosa* and Handke's *Wunschloses Unglück*. Fourteen are used on 2 sheets each, among them Marienthal, *Der Herr Karl*, Ringel's *Die österreichische Seele*, Haderlap's *Engel des Vergessens* and the Urban Jarnik institute. Kirchler's tax-morale work appears twice (Sagittarius/Honesty and Capricorn/Law).
- **Group pattern:** Carinthian Slovenes, Burgenland Croats, Turkish-Austrians and Bosnian-Austrians appear in nearly every sheet. Part of this is the search-term tables, which list those languages. In Aries the same four groups ran through every "Who to compare" list. From Taurus on, each prompt asked for a wider spread, and the sheets then brought in:
  - Danube Swabians, Yenish, Viennese Czechs and Slovaks, and Serbian- and Croatian-Austrians;
  - Polish, Ukrainian and Chechen communities, and Filipino care workers;
  - Slovak and Romanian carers;
  - Deaf signers (ÖGS and DGS), LGBTQ communities and people with disabilities;
  - Old Catholics, Alevis, Orthodox parishes, Jehovah's Witnesses and the *Toleranzgemeinden*;
  - the nobility's descendants, *Beamte*, conscripts and *Zivildiener*;
  - hospice and mountain-rescue workers, and people in recovery.

## Thin, repetitive or generic sheets
- **No sheet is thin.** The shortest are:
  - Aries/Initiative: 1,059 words.
  - Leo/Leadership: 1,085.
  - Gemini/Mediation: 1,087.
  - Scorpio/Power: 1,105.
  - Aquarius/Hope: 1,105.

  All five have 13 to 15 pointers.
- **Fewer pointers:** 13 sheets have 13 pointers each:
  - Scorpio (average 13.5): Betrayal, Control, Trust, Revenge, Power and Crisis.
  - Sagittarius (average 13.8): Honesty and Fundamentalism.
  - Aquarius (average 13.8): Reform, Nonconformity and Hope.
  - Libra: Peace at any price and Projection.
- **Romani search terms are thin in Libra.** Impartiality, Peace at any price and Projection say in their Flags lines that the Romani terms are still to be found.
- **Aries is the most formulaic sign.** It ran the same four minority groups through every sheet; see Repetition.
- **Pre-modern pointers:** 80 sheets tag a pointer "pre-modern". Most of the rest have an older pointer without the tag, such as court household records, Fischer von Erlach (1721), Mesmer, *Sühnekreuze* and the *Weistümer*. A few rely on 19th-century sources as their oldest: Libra/Diplomacy (the Congress of Vienna) and Virgo/Service.

## Pointers per sheet
- 13 pointers: 13 sheets, all in Libra, Scorpio, Sagittarius and Aquarius.
- 14 pointers: 62 sheets.
- 15 pointers: 48 sheets.
- 16 pointers: 7 sheets:
  - Aries: Domain, Beginning and Competition.
  - Taurus: Domain and Wealth.
  - Gemini: Information.
  - Leo: Creativity.

The average is 14.4. Per-sign ranges are in the table above.

## Does the run exploit the nation's depth?
Mostly yes.
- **Pre-modern sources:** they run from Late Antiquity to the 18th century. Examples are the *Vita Severini*, the *Conversio Bagoariorum et Carantanorum*, *Muspilli*, the *Wessobrunner Gebet*, the *Kaiserchronik* and the *Passauer Anonymus*. Others are the *Nibelungenlied* Danube route, Der Stricker, Walther, the *Ausbund* Passau hymns, the Vienna *Matrikel*, *Mirakelbücher*, *Weistümer*, Hohberg, Canisius and Sonnenfels.
- **Old Bavaria against the Free State's other parts:** Franconia, Swabia and the Upper Palatinate are set against Old Bavaria repeatedly. The confessional line (Lutheran Franconia against Catholic Old Bavaria) recurs as a comparison axis.
- **Austrian Länder:** all appear. East Tyrol, the Innviertel and Lower Austria are used least (in 13 to 36 sheets).
- **Minority languages:** Burgenland Croatian, Carinthian Slovene, Burgenland Hungarian, Romani, Czech and Slovak terms appear in the search-term tables throughout.
- **Weaker coverage:**
  - Burgenland Hungarians (34 sheets) and Sinti (50).
  - Sudeten German descendants (26), Polish (28) and Ukrainian (25) communities.
  - Chechen-Austrians (11), Filipino-Austrians (5), LGBTQ communities (5) and Deaf signers (8).

## Judgment calls for the author to confirm
1. **South Tyrol:** it is treated as comparison only, because Magna Lombardia is separate. It appears in only 2 sheets: Aries/Identity, and Libra/Diplomacy with the Gruber–De Gasperi Agreement. Whether it belongs to Austro-Bavaria is the author's call.
2. **Lands at the edges:** the sheets name several areas without settling them. They include Franconia and Bavarian Swabia, which are not Bavarian-speaking, as parts of the Free State, and Coburg (Aquarius/Group). They also name the Innviertel and Rupertiwinkel as lands that changed hands, and Vorarlberg's Alemannic west. The author's Stage 0 decides them.
3. **German-wide datasets:** sources such as the ESS, ISSP, the Preference Survey and Hofstede/GLOBE give Austria plus Germany, with Bavaria as a subsample (46 sheets mention Germany). They are used that way, never as Austro-Bavaria's core. Confirm this is acceptable.
4. **Romani *sikhol*:** it is kept as a QA false positive, as above.
5. **Afghan-Austrians:** they are named once, in Cancer/Shelter, about unaccompanied minors. This follows the Germany run's precedent of treating Afghan communities as outside the South Asian rule. Confirm, or move them to a Held category.
6. **Two bullets were reworded by hand** to remove implied traits (Cancer/Protection, Capricorn/Order). Confirm the wording.
7. **Hutterite and Anabaptist history** is used as Tyrol's own, with colonies abroad as comparison only. **Monte Verità** (Ticino) appears only as part of Schwabing's circle (Aquarius/Idealism).
