# Hungary springboard run: report (2026-11-24)

**Run agent:** one per nation, deeper brief (accuracy and depth first), one sub-agent per sign, Aries to Pisces in order. Tuesday wave 1 (Monday's wave 3, moved by the author).
**Result:** 130/130 sheets `STATUS: done 2026-11-24, not verified` by `springboard_status.py`; whole-nation `springboard_qa.py Hungary`: **130 sheets scanned, 0 problems**. No relaunches; 5 kinds of smallest edit by the run agent (listed below); no usage-limit stop.
**Wall clock:** start 05:04 (first launch 05:05), last sub-agent back 08:59, report 09:05.
**Sub-agent tokens:** **3,020,439** (12 sign agents, 0 relaunches; 747 tool uses).

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers | Tokens | Minutes |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,172 | 1,259 (Domain) | 14-15 | 195,958 | 17.3 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,208 | 1,274 (Domain) | 14-15 | 234,741 | 19.0 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 1,171 | 1,276 (Domain) | 14-16 | 232,593 | 15.8 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,194 | 1,292 (Domain) | 14-16 | 217,033 | 13.2 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,166 | 1,256 (Domain) | 13-14 | 260,816 | 17.7 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,183 | 1,267 (Domain) | 14-16 | 225,586 | 13.8 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,228 | 1,272 (Domain) | 14-15 | 274,256 | 17.7 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,171 | 1,283 (Domain) | 13-14 | 283,424 | 23.6 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 1,222 | 1,278 (Domain) | 13-14 | 268,911 | 24.6 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1,228 | 1,283 (Domain) | 13-15 | 272,659 | 18.4 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1,198 | 1,289 (Domain) | 14 | 279,668 | 22.3 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,235 | 1,269 (Domain) | 13-15 | 274,794 | 22.5 |
| | **Total** | **130** | **12** | **0** | **0** | **1,197** | 1,292 | 13-16 (avg about 14.3) | **3,020,439** | |

Word counts by `wc -w`: 1,108 (Aries Recklessness) to 1,292 (Cancer Domain); none over 1,300. Pointers per sheet: 13 in 10 sheets, 14 in 77, 15 in 39, 16 in 4.

## Rule breaks and fixes
- **QA scan:** 0 problems in every sign and for the whole nation; no relaunch was needed.
- **Run-agent smallest edits (no content lost; status lines untouched):**
  1. Gemini *Curiosity*: a bare "Held for review: none." given its own wording. From Cancer on, the sub-agent prompt said a Held line is never a bare "none."
  2. Lands hedge outside the Domain sheets: the "working reading" / "for this run" qualifier had crept into the Target line of 7 Leo concept sheets (Recognition, Being seen, Humiliation, Generosity, Leadership, Play, Honor) and 10 Taurus concept sheets (Possession, Ownership, Self-worth, Values, Security, Stability, Wealth, Possessiveness, Stubbornness, Sensuality). Each was cut to the plain lands ("with the Hungarian communities of Transylvania and the Székely Land"). From Virgo on, the prompt said so; afterwards the hedge sits in the 12 Domain sheets only.
  3. Libra *Diplomacy*: the Held line said "section 0 of this sign"; reworded to "this sign's Domain sheet".
  4. Sagittarius *Education* and Capricorn *Ambition*: the Held lines described the set-aside South Asian item (students at the medical universities, their career aims). Both were cut to the category only. This was done by hand rather than by relaunching the sheet, because only the Held line was affected.
- **South Asian rule:** the run agent's own name scan (scholars, writers, works, religions, places, "Indo-") was clean in all 130 sheets. The category is held on 4 Held lines for real set-asides: Sagittarius *Domain* (a religious-landscape pointer), Sagittarius *Education* (a schooling pointer), Capricorn *Ambition* and Aquarius *Idealism* (a schooling pointer). No other Held line uses it. No medical-school student body and no Roma-origin or Romani-ancestry pointer appears anywhere.
- **Buddhism:** held as a category only, never named as a community, temple or text, on 6 Held lines: Scorpio *Rebirth*, Sagittarius *Domain*, Capricorn *Discipline*, Aquarius *Idealism* and *Detachment*, and Pisces *Spirituality*. The author should note these sheets (see the judgment calls).
- **Law:** the letter of the law stays in Libra (for example, *Justice* points to the decrees of Ladislaus and Coloman, the Csemegi code of 1878, the people's tribunals and Constitutional Court rulings) and the spirit in Capricorn (*Law*, *Authority*). Every other sign defers law on its Held line, each in its own words.
- **Universals, Hermes, zodiac words:** none anywhere.
- **Process note:** the sub-agents shared the nation's own `tmp/` folder across signs (the Libra agent remarked on it). It was Hungary's folder only, with no cross-nation file.

## Repeat check (whole nation, run agent's own)
- **Exact repeats:** none for any line over 40 characters, any table row, "Who to compare" bullet, Flags line or first query (the template's fixed lines aside).
- **Near matches (ratio over 0.85):** 1. Leo *Self-expression* and *Joy* each have a first query to search the folklore journals (*Ethnographia*, *Néprajzi Közlemények*), for different terms (*emlékkönyv* and *csujogató*). They are not copied, so both are kept.
- The sub-agents also swapped pointers that repeated earlier signs; Gemini reported 5 swaps.

## Thin, repetitive or generic sheets
- **Fewest pointers (13):** Leo *Dignity* and *Honor*; Scorpio *Revenge* and *Power*; Sagittarius *Domain*; Capricorn *Domain*, *Responsibility*, *Hierarchy* and *Merit*; Pisces *Domain*. None of these is thin in content.
- **Pre-modern depth:** every sheet has a pre-modern pointer or an early folk-collection pointer. However, the named classics in the prompt list are used sparingly across the nation: *Gesta*/Anonymus/Kézai 7 sheets, *Képes krónika* 6, *Tripartitum* 5, *rovás* 4, Bartók 4, Kodály 3, Vizsoly 3, *Halotti beszéd* 2, Torda 1568 2, Apáczai 2, *Ómagyar Mária-siralom* 1, Ottoman *defters* 1. The sub-agents went for variety instead: Bonfini, Bethlen Kata, the Csíksomlyó passion plays, Sárospatak college statutes, Transylvanian wills, the Várad register and others. The later research could lean on the chronicles and the *defters* more.
- No sheet reads as generic or padded on the run agent's spot reads (Aries *Identity*, Gemini *Curiosity*, Libra *Justice*, Leo *Dignity* and *Generosity*, Capricorn *Ambition*, Pisces *Empathy*, Scorpio *Control*).

## Does it exploit the nation's depth?
Largely yes. The table gives the number of sheets (of 130) that mention each item.

| Mentioned in | Items |
|---|---|
| All 130 sheets | Székely; Roma; Boyash or Beash; Slovaks; Croats (Bunjevac and Šokac); Serbs; Rusyns |
| 120 to 129 | Jewish communities 129; Vlach Roma or Lovari 129; Budapest 127; Danube Swabians 127; Neolog 121 |
| 100 to 119 | Catholics 115; Reformed 112; the Great Plain 111 |
| 75 to 99 | Romanians of Hungary 94; Kolozsvár 90; Palóc 88; Status Quo 81; 1944 and the Holocaust 81; Unitarians 75 |
| 50 to 74 | Lutherans 69; Kiskunság and Kun 68; Szeged 66; the Nyírség and Szatmár 59; Armenian-descended Hungarians 57; Kalotaszeg 56; Jász 53; Greek Catholics 53; Nagyvárad and the Partium 50 |

**Weaker spots:**
- Places: Tokaj (21 sheets), the Hortobágy (22), Lake Balaton (26), Eger (35), Miskolc (36), Sopron (38) and Pécs and Győr (41 each).
- Contested history: Trianon is pointed to in only 13 sheets and 1956 in 24.
- The Csángó (13 sheets) are rightly kept to comparison.

## Judgment calls for the author
1. **Lands:** there is no `00 - Scope.md` and no settled territory. The sheets are written for Hungary as it stands plus the Hungarian communities of Transylvania and the Székely Land, as a working reading. The note on this appears once in each Domain sheet. The Romanian majority and Romanian sources are comparison only; the Csángó of Moldavia are comparison only. Please confirm this when Stage 0 is set.
2. **Buddhism (open question):** the category is held on 6 sheets (Scorpio *Rebirth*, Sagittarius *Domain*, Capricorn *Discipline*, Aquarius *Idealism* and *Detachment*, Pisces *Spirituality*). Please confirm whether to keep it as a category or to name sources.
3. **South Asian holds:** 4 sheets hold the category: Sagittarius *Domain* and *Education*, Capricorn *Ambition* and Aquarius *Idealism*. Two of the holds (Education, Ambition) concern the medical universities' student body. Please confirm that these belong under the rule.
4. **Libra *Impartiality*:** its Held line leaves "corruption as a concept" to the author's decision (no sign owns it yet).
5. **Roma history:** no sheet discusses origins or the ancestry of the Romani language. The sub-agents were told to keep Roma history to its European record so that no South Asian place or language appears. Please confirm this is the reading you want.
6. **Kőrösi Csoma Sándor** (the Székely-born traveler and Tibetan-language scholar) is named in no sheet, because pointing to him would bring in Buddhist texts and South Asian places. He could be a Hungarian or Székely pointer if the Buddhism and South Asian rulings allow it.

## Files
- Sheets: `Targets/Europe/Hungary/Springboards/01 - Aries/` to `12 - Pisces/` (130 files).
- Run log: 13 lines appended with `>>` to `_dispatch/SPRINGBOARD_PROGRESS.md` (one per sign and one completion line).
