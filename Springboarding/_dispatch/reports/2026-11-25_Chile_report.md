# Chile springboard run: report (2026-11-25)

**Run agent:** one per nation, deeper brief (accuracy and depth first), one sub-agent per sign, Aries to Pisces in order. Wednesday wave 1.
**Result:** 130/130 sheets `STATUS: done 2026-11-25, not verified` by `springboard_status.py`; whole-nation `springboard_qa.py Chile`: **130 sheets scanned, 0 problems**. No relaunches. The run agent made 14 smallest edits by hand (listed below). No usage-limit stop and no forced hand-back.
**Wall clock:** start 05:05 (first launch 05:06), last sub-agent back 09:15, report 09:40 (MST).
**Sub-agent tokens:** **3,043,637** (12 sign agents, 0 relaunches; 742 tool uses).

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers | Tokens | Time | Run-agent edits |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,125 | 1,235 (Domain) | 14 | 167,496 | 05:06-05:19 | 1 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,192 | 1,280 (Domain) | 14-15 | 209,373 | 05:20-05:39 | 0 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 1,183 | 1,280 (Domain) | 13-16 | 192,929 | 05:40-05:51 | 0 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,182 | 1,295 (Domain) | 14-15 | 217,614 | 05:51-06:06 | 1 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,189 | 1,293 (Domain) | 14 | 261,438 | 06:07-06:31 | 0 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,248 | 1,298 (Domain) | 13-15 | 237,489 | 06:32-06:48 | 1 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,267 | 1,300 (Peace at any price) | 14-15 | 267,178 | 06:49-07:09 | 1 (at the end) |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,268 | 1,294 (Purging) | 14-15 | 274,522 | 07:10-07:35 | 1 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 1,243 | 1,294 (Faith, after edit) | 13-15 | 295,156 | 07:36-07:58 | 1 (2 passes) |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1,252 | 1,281 (Discipline) | 12-14 | 306,066 | 07:59-08:26 | 1 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1,244 | 1,279 (Group, Reform, Community) | 14 | 297,390 | 08:27-08:48 | 2 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,243 | 1,299 (Domain, after edit) | 13-14 | 316,986 | 08:50-09:15 | 5 |
| | **Total** | **130** | **12** | **0** | **0** | **1,219** | 1,300 | 12-16 | **3,043,637** | | **14** |

Word counts by `wc -w`: 1,058 (Aries Initiative) to 1,300 (Libra Peace at any price); none over 1,300. The sheets lengthen through the run (Aries 1,125 on average, Libra to Pisces about 1,245 to 1,268), and nine Domain or concept sheets sit at 1,290 to 1,300. **Pointers per sheet** (rows in section 2): 12 on 3 sheets (Capricorn Hierarchy, Law, Order), 13 on 16, 14 on 96, 15 on 14, 16 on 1 (Gemini Curiosity). Every sheet is in the 12-to-16 band; Capricorn is at its low end (12.9 on average).

## Rule breaks and fixes
- **QA scan:** 0 problems in every sign and for the whole nation; no "Indian" anywhere (no published title needed it); no URL; no banned word; no universals list; no Hermes material.
- **Run-agent smallest edits (status lines untouched, no pointer dropped):**
  1. Aries Domain: the lands note named a missing scope file; cut (the lands note stays once in the Domain Flags). From Taurus on, the prompt forbade naming a scope file at all.
  2. Cancer Abandonment: the newcomers' compare bullet was 0.86 to Family's; rewritten to ask how a departure is told by the one who left and the kin who stayed.
  3. Virgo Health: the Held line described the held South Asian item's field; cut to the category only.
  4. Scorpio Rebirth: the *canuto* search-term row was 0.92 to Taurus Self-worth's; gloss and note tied to conversion testimonies.
  5. Sagittarius Faith: the Mapudungun *feyentun* row was 0.97 to Scorpio Trust's; reworded (the first wording pushed the sheet to 1,305, so it was shortened to 1,294).
  6. Capricorn Domain: the Held line said cross-national deference indexes are carried on Authority and Hierarchy; only Hierarchy carries one. Made true.
  7-8. Aquarius Community (first query on Razeto, 0.98 to Aries Initiative's) and Hope (Haitian Creole *si Bondye vle* row, 0.88 to Libra Indecision's): made concept-specific.
  9-13. Pisces: Boundary's Rapa Nui *kainga* row (0.91 to Aries Independence's) reworded; Boundary's Held line said Leo Humiliation carries the Bolivian sea rulings (it carries Peru's 2014 ruling as received in Arica), now names only Libra Diplomacy; the Held lines of Dissolution and Spirituality described their South Asian items (a meditation teaching, bodily disciplines) and the Domain called them movements: all three cut to the category only.
  14. Libra Partnership: its first query (Valdivia's letters on Memoria Chilena) was 0.85 to Aries Beginning's at the whole-nation check; given different terms (Sancho de Hoz, *compañía*).
- **Cross-references checked:** about 30 Held lines say an item is carried on another sheet; each was checked against the named sheet. Two were false (Capricorn Domain, Pisces Boundary) and were corrected; the rest are true.
- **The run agent's repeat check across the nation** (every line of 40 characters or more, including table rows, compare bullets, Flags and Held lines and first queries; exact and near matches at 0.85): **0 exact repeats, 0 near matches** after the edits above.
- **Run agent's own name scan:** no South Asian scholar, writer, work, community or religion named anywhere outside the Held lines. Two hits were false positives and are kept as written: Haitian Creole *zen* ("gossip", Gemini Gossip) and *Sen* ("holy", in *Lespri Sen*, Pisces Dissolution).

## Held lines
- **South Asian category** (category only, nothing named): Virgo Health, Scorpio Rebirth, Pisces Dissolution and Spirituality (the Pisces Domain refers to these two). Each followed a real pointer set aside under the rule.
- **Buddhism** (category only, no community, temple or text named): Cancer Belonging, Scorpio Death and Rebirth, Sagittarius Domain, Capricorn Discipline, Aquarius Detachment, Pisces Spirituality (7 sheets).
- **Empty Held lines:** every one names a concept-specific item weighed. Two weak spots: Aries puts five Held lines on one frame ("X weighed and left to Libra", each a different item), and Gemini's Held lines for Communication, Information, Connection, Duality and Gossip say only which kind of source was screened. From Cancer on the prompt asked for the specific item weighed, and the later Held lines are specific (many point to the earlier sheet that already carries the item).

## Thin, repetitive or generic sheets
- **Aries Recklessness:** no Mapudungun or Aymara terms (the sub-agent said this in the sheet's Flags as thin data).
- **Capricorn Hierarchy, Law, Order:** 12 pointers each, the band's low end.
- **Gemini Held lines** (above) and the shortest sheet, **Aries Initiative** (1,058 words), are the least developed; nothing reads as generic or copied.
- No sheet read as research or stated a finding; compare bullets say what to check.

## Do the sheets use the nation's depth?
Mostly yes. Counts across the 130 sheets: Rapa Nui on 130, Haitian on 130, Aymara on 129, Quechua 102, Venezuelan 98, Palestinian 92, Juan Fernández 90, Lickanantay (Atacameño) 86, Diaguita 85, the Pentecostal churches 76, *huaso* 78, the Central Valley regions (Maule, Ñuble, O'Higgins) 71, Kunza 49, the Norte Chico (Elqui, Coquimbo) 33, the nitrate and *salitre* towns 33, Lota and Coronel 33, Croatian 34, Jewish 28, Afro-Chileans of Arica 22, Basque 11. Pre-modern pointers named in the prompt (Valdivia, Ovalle, Molina, the Cabildo, Chinchorro, rongorongo, *encomienda*) are on 40 sheets, with other colonial and archaeological pointers on many more; the *Lira popular* broadsides only on 7. **Thinnest:** Basque families, Afro-Chileans, the Colla and Chango peoples (often flagged as thin, with where to look) and the *Lira popular*. These are the places to push in the research stage.

## Judgment calls for the author
1. **Lands:** the sheets take the north and center, from the Norte Grande to the Biobío (Concepción, Lota and Coronel inside), plus Rapa Nui and Juan Fernández, as the core. The south and Wallmapu are Araucanía-Patagonia comparison only. **Where the line runs (the Biobío or another line) and Rapa Nui's status are yours to settle;** the Domain sheets say once that the lands are still to be settled.
2. **Mapuche lines:** Mapuche families in Santiago and central Chile are written as Chile's people. Wallmapu's *lonkos* and *admapu* (Leo Leadership and Honor), the Mapuche hunger strikes (Pisces Self-sacrifice), *machi* knowledge and the 1960 Valdivia earthquake (Scorpio Crisis) are kept as Araucanía-Patagonia comparison. Confirm that split.
3. **Rapa Nui's 1888 agreement:** Pisces Surrender keeps it off the sheet so island history is not framed as a defeat (it is on Aries Independence and Libra Diplomacy). Confirm.
4. **Buddhism** held as a category on 7 sheets; **South Asian category** on 4 (above): your open rulings.
5. **Peru and Bolivia:** Hague rulings and the cross-border Aymara are given as comparison only, through Arica and Tarapacá.
