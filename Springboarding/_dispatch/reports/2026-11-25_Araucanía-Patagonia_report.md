# Araucanía-Patagonia: springboard run report (2026-11-25)

Run agent, deeper brief, one sub-agent per sign. Wednesday wave 2. All sheets are `STATUS: done 2026-11-25, not verified`.

## Summary
- **Sheets:** 130 of 130 done (12 signs). **Agents:** 13 (12 sign agents and 1 single-concept relaunch).
- **QA (`springboard_qa.py`, whole nation):** 130 scanned, 0 problems. The only QA flag during the run was Virgo's Domain sheet, at 1,302 words. A relaunch tightened it to 1,264 words without dropping a pointer.
- **Sub-agent tokens:** 3,134,746 in total (sign agents 3,072,178; relaunch 62,568).
- **Wall-clock:** 09:05 (first launch) to 13:36 (last check). The sub-agents ran from 09:05 to 13:28.
- **Words (`wc -w`):** average 1,243. Longest 1,299 (Aquarius Idealism), shortest 1,083 (Leo Generosity). None is over 1,300.
- **Pointers:** 1,751 in all, 12 to 15 per sheet. By count: 22 sheets have 12, 33 have 13, 67 have 14 and 8 have 15.

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA problems | Run-agent edits | Avg words | Longest | Shortest | Pointers | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 5 | 1,209 | 1,266 Domain | 1,162 Competition | 159 | 187,273 | 09:05-09:21 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 2 | 1,238 | 1,278 Ownership | 1,189 Stubbornness | 148 | 250,705 | 09:26-09:46 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 0 | 1,254 | 1,288 Learning | 1,183 Gossip | 139 | 243,219 | 09:51-10:09 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 0 | 1,242 | 1,287 Domain | 1,207 Motherhood | 138 | 230,358 | 10:12-10:30 |
| 5 | Leo | 13 | 1 | 0 | 0 | 4 | 1,198 | 1,295 Domain | 1,083 Generosity | 167 | 265,755 | 10:33-10:53 |
| 6 | Virgo | 10 | 2 | 1 | 1 (long) | 0 | 1,185 | 1,271 Service | 1,098 Perfectionism | 133 | 274,761 + 62,568 | 10:58-11:21 |
| 7 | Libra | 11 | 1 | 0 | 0 | 0 | 1,251 | 1,283 Domain | 1,187 Balance | 154 | 260,435 | 11:20-11:39 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 0 | 1,254 | 1,275 Death | 1,224 Domain | 140 | 280,655 | 11:42-12:01 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 0 | 1,269 | 1,289 Meaning | 1,237 Education | 135 | 280,548 | 12:04-12:25 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 0 | 1,279 | 1,296 Ambition | 1,237 Hierarchy | 132 | 259,091 | 12:28-12:45 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 0 | 1,274 | 1,299 Idealism | 1,235 Detachment | 138 | 277,340 | 12:49-13:06 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 0 | 1,254 | 1,282 Compassion | 1,194 Fear | 168 | 262,038 | 13:08-13:28 |

Word counts are as each sign finished. The final edge labels (below) added 2 or 3 words to 26 sheets.

## Rule breaks and fixes
- **Repeats against Chile:** 6 search-term rows came close to rows in Chile's sheets, at 0.85 to 0.94 similarity. They were the plain Spanish or Mapudungun words, with the same dictionary gloss: *werken*, *año nuevo, vida nueva*, *allegado*, *imprudente/temerario/a lo loco*, *autoestima/amor propio/dignidad*, *valores/principios/buenas costumbres* and *ayüwün*. Run-agent smallest edits gave each a gloss and a note tied to its own concept and to the south. From Gemini on, the prompt asked for this, and no further matches with Chile came up.
- **Repeats within the nation:** two "Who to compare" bullets in Leo had the same frame with one word swapped (Welsh on Generosity and Honor; Aónikenk on Play and Joy). Both were rewritten. The final check across the whole nation, and against Chile's and Argentina's sheets, found **no exact repeat** of a line, table row, compare bullet or Flags line. Three near matches were kept, all at 0.85: first queries with the same frame but different search items (two National Library of Wales catalog searches; the *Wenufoye* and Curalaba press searches).
- **South Asian rule:** Aries Domain's Held line described the held South Asian-heritage item by its type of study. It now gives the category only. Pisces Spirituality holds the category once, as a real set-aside (South Asian-derived meditation and body-practice centers). No South Asian name appears anywhere. No mobility atlas is named.
- **"Extinct":** Leo Recognition called the Selk'nam "a people long called extinct". It now reads "a people that outsiders' books had long written off". From Virgo on, the prompt barred the label even as a report of what others said.
- **Length:** Virgo Domain was at 1,302 words. The relaunch fixed it, as noted above.
- **Edges of the lands:** see the judgment calls below. The run agent labeled 26 sheets.

## Thin, repetitive or generic sheets
- **At the bottom of the 12 to 16 pointer band:** Leo Dignity, Humiliation, Generosity, Play, Honor and Joy have 12 pointers each. Generosity is also the shortest sheet, at 1,083 words. Eight Sagittarius sheets also have 12, and so do Taurus Stubbornness, Scorpio Betrayal, Trust, Revenge and Secrecy, and Capricorn Law.
- **Generic Held lines:** Pisces fills its Held lines with unnamed outside items set aside to make a point: a "culture-bound syndromes" survey, a pop-psychology book on "empaths", a "places to disappear" list, business-coaching books. They are harmless, but they are filler rather than real set-asides.
- **Formulaic Held lines:** every Held line in Gemini is a law set-aside. Gemini and Taurus Held lines all follow one pattern: "Libra takes the text, Capricorn the purpose". From Cancer on, the Held lines vary in kind: restricted knowledge, private papers, sources that profile a group, closed or live files, remains under repatriation claims.
- **Leo compare bullets** are short and close in frame across sheets. Two were fixed. The rest differ in their concept word and are kept.
- **Sources that return:** a few core sources come back in later signs, each with a new angle and new wording, as the sub-agents reported: Lenz, the CEP Mapuche surveys, SENDA, the *parlamentos* edition, *Arauco domado*, González de Nájera, Río Turbio and the National Library of Wales catalog.

## Depth
On the whole, the sheets do use the nation's depth.
- **Peoples, by number of sheets:**
  - Welsh: 129
  - Croatian: 128
  - German: 128
  - Kawésqar: 121
  - Yagán: 113
  - Aónikenk: 112
  - Williche: 107
  - Selk'nam: 96
  - Pewenche: 95
  - Boer: 92
  - Gününa küne: 59
  - Lebanese: 28
  - Basque: 11
- **Regions, by number of sheets:**
  - Chiloé: 124
  - Neuquén: 123
  - Aysén: 89
  - Comodoro Rivadavia: 83
  - Santa Cruz: 82
  - Ushuaia: 41
- **Search terms:** Mapudungun with its regional forms, Welsh, German, Croatian, Afrikaans, Aonekko ʼaʼien, Kawésqar, Yagán and Selk'nam.
- **Pre-modern pointers, by number of sheets:**
  - *Y Drafod*: 15
  - Luis de Valdivia's grammar: 15
  - *La Araucana*: 10
  - Febrés: 8
  - the *parlamentos*: 7
  - *Cautiverio feliz*: 6
  - Musters: 5
  - Monte Verde: 2
  - Cueva de las Manos: 1

  Many sheets also carry their own pre-modern pointers: González de Nájera, Pigafetta, Guevara's *Folklore araucano*, the Lehmann-Nitsche cylinders, Cavada's Chilote dictionary and the colonial *tasas*.
- **Weak spots:**
  - Basque and Lebanese families appear on only a few sheets.
  - The archaeological sites (Monte Verde, Cueva de las Manos) are barely used.
  - Ushuaia and the Argentine side of Tierra del Fuego get less than the Chilean far south.
  - The record for the canoe and steppe peoples is flagged as thin and written mostly by outsiders, as the brief expects.

## Judgment calls for the author
1. **Lands (no `00 - Scope.md`).** The sheets work in the frame of Wallmapu and Patagonia on both sides of the Andes. The lands note sits once in each sign's Domain Flags, and no unit list was added. These are open for the author:
   - where the edges run: the Biobío with Alto Biobío and the Arauco coast, La Pampa and southern Buenos Aires province, southern Mendoza;
   - the Falklands / Malvinas, which the sheets treat as comparison only.
2. **Tirúa and Cañete.** Both are in the Arauco province of the Biobío region and are a center of Lafkenche life. The sub-agents for Aries to Aquarius used them freely, and the Sagittarius and Pisces sub-agents moved some of their pointers to places inside the Araucanía.
   - The run agent labeled the remaining first mention on 26 sheets "(Biobío edge, comparison)", following the instruction that edge areas are comparison only. The sheets are listed in the Run log.
   - Alto Biobío (the Ralco dam, the Pewenche) is also marked as comparison.
   - If the author puts the Arauco coast inside the nation, the labels come off.
3. **Buddhism:** held as a category on Aquarius Detachment and Pisces Spirituality. Nothing is named.
4. ***Doma india*** (Capricorn Discipline): this is the Spanish name of a gentle method of starting horses. It is kept as the practice's own name, which is the same treatment the run gives published titles. Please confirm, or ask for it to be renamed.
5. **A Chiloé title containing "indiana"** (Taurus): the sub-agent swapped it for a source-type pointer, although a published title may stay in quotation marks. Restore the title if wanted.
6. **The 'Universal' hit** on Pisces Compassion is Argentina's *Asignación Universal por Hijo*, a program name. It has nothing to do with the universals rule, so it was kept.
7. **The 'temple' hits** on Sagittarius are the neo-Pentecostal IURD's own word for its churches. They were kept.
8. **Contested ground** is handled as accounts throughout: the 'Pacification of the Araucanía', the 'Conquest of the Desert', the Selk'nam killings, *Patagonia rebelde*, the antiterrorism cases, the 2020 Curacautín events, the 2021 Comarca Andina fires, and the missions. Two held items in particular are for the author to decide on, if and how they are used:
   - an outsider's book on a death at Lake Budi in 1960 (Scorpio Crisis);
   - a jailed leader's manifestos (Sagittarius Conviction).
