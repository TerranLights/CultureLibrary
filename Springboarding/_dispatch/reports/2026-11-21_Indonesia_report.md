# Indonesia springboard run: report (2026-11-21)

**Result:** 130 of 130 sheets done (all `STATUS: done 2026-11-21, not verified`), twelve signs, Aries to Pisces, one sub-agent per sign under the deeper brief. No relaunches, no hand edits. Whole-nation QA: **130 sheets scanned, 0 problems** (no false positives either: the sub-agents avoided "Indian", "Indo-" and the almanac words as told).

**Wall-clock:** run agent start 14:40 MST, end 17:50 MST (3 h 10 min; first sub-agent launched 14:41, last returned 17:48). No usage-limit stop.

**Total sub-agent tokens: 2,423,403** (12 sign agents, no relaunches; each figure as reported by the agent's completion notice). The run agent's own tokens are not included.

**Lands:** the tracker header lists no settled lands and there is no `00 - Scope.md`. Per the brief's missing-scope rule, each sign's Domain sheet says once that the nation's exact lands are still to be settled and the sheets are written for the core lands; no unit list was added. Aceh and West Papua appear only in flags, as separate targets (3 concept sheets: Taurus Stubbornness, Gemini Mediation, Pisces Self-sacrifice), never as Indonesia's core. `Hermes_research` was not opened.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words (wc -w) | Longest | Shortest | Pointers (avg) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,102 | 1,244 Domain | 1,027 Competition | 15-16 (15.2) | 160,283 | 14:41-14:54 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,119 | 1,267 Domain | 1,047 Possessiveness | 14-15 (14.6) | 224,967 | 14:55-15:14 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,163 | 1,287 Domain | 1,102 Gossip | 14-16 (15.3) | 178,208 | 15:15-15:26 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,163 | 1,269 Domain | 1,106 Belonging | 14-15 (14.9) | 191,303 | 15:27-15:40 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,157 | 1,275 Domain | 1,081 Humiliation | 14-16 (14.8) | 225,425 | 15:40-15:59 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,204 | 1,283 Domain | 1,145 Analysis | 16 (16.0) | 196,168 | 16:00-16:14 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,087 | 1,237 Domain | 1,048 Projection | 15-16 (15.4) | 197,545 | 16:14-16:27 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,232 | 1,290 Death | 1,167 Control | 14-15 (14.9) | 213,646 | 16:28-16:44 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,221 | 1,268 Faith | 1,110 Honesty | 16 (16.0) | 220,046 | 16:44-17:02 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,192 | 1,248 Authority | 1,127 Ambition | 15-16 (15.6) | 200,778 | 17:02-17:17 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,187 | 1,264 Community | 1,114 Friendship | 15-16 (15.6) | 205,287 | 17:18-17:32 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,203 | 1,290 Domain | 1,141 Intuition | 15-16 (15.2) | 209,747 | 17:33-17:48 |
| | **Nation** | **130/130** | **12** | **0** | **0** | **1,169** | 1,290 | 1,027 | 14-16 (15.3) | **2,423,403** | |

Words: 46 sheets over 1,200, none over 1,300. Pointers per sheet (table rows under "Where to look first"): 11 sheets with 14, 72 with 15, 47 with 16.

## Rule breaks and fixes
- **None found.** QA 0 problems for every sign and for the whole nation; no hand edits; no relaunches.
- **Held for review:** 67 sheets carry a category-only line ("South Asian-heritage communities in the nation's lands", sometimes with the reason, e.g. "for their own cleansing festivals"); a few set aside, as categories, South Asian works on the source epics behind Old Javanese poetry and the *Hasta Brata*, and Islamic movements founded in South Asia (Sagittarius Domain and Fundamentalism). No community, scholar, language or work is named. Indonesia's own Hindu-Buddhist heritage (Old Javanese kakawin, *Desawarnana*/*Nagarakretagama*, Balinese Hinduism, wayang) was kept as the nation's material.
- **Law:** Libra sheets kept to the letter (the 2023 Criminal Code, KUHAP, statutes and regulations as written, recorded adat codes such as *Simbur Cahaya*); Capricorn to the spirit; other signs point to Libra or Capricorn.
- **Lands note** once per Domain sheet; the Gemini and Leo Domain notes share the same wording (intended, the one-per-Domain note).
- **Housekeeping:** the Aquarius sub-agent's QA helper overwrote an earlier sub-agent's temporary script in the nation's scratch `tmp/` folder; harmless, nothing in the results touched.

## Repetition
- **Across all 130 sheets: 0 repeated lines** over 40 characters (table rows, sentences, "Who to compare" bullets), beyond the template's fixed lines, the Held line and the lands note. No "Who to compare" bullet is copied between sheets.
- **Most reused sources** (sheets naming them, of 130): BPS (47 as a pointer); *Kompas* (30 sheets) and *Tempo* (21); Clifford Geertz (22, mostly *The Religion of Java* and the Bali essays); Mangkunegara IV (*Serat Wedhatama*, 13), Pramoedya Ananta Toer (13), World Values Survey (13), the Indonesia Family Life Survey (13); Kartini's letters (*Habis Gelap Terbitlah Terang*, 11), *Serat Wulangreh* (11), Hildred Geertz, *The Javanese Family* (11), *Desawarnana*/*Nagarakretagama* (11); Dhofier, *Tradisi Pesantren*, and Magnis-Suseno, *Etika Jawa* (9 to 10 each). Spread over 130 sheets this is variety, though Javanese court literature recurs more than any other pre-modern tradition.

## Thin, repetitive or generic sheets
- **Shortest sheets** (still 15 pointers each, no rule breaks): Aries `09 - Competition` (1,027), `07 - Independence` (1,036), `08 - Anger` (1,047), Taurus `08 - Possessiveness` (1,047), Libra `10 - Projection` (1,048), Aries `06 - Courage` (1,056), `10 - Recklessness` (1,060), Libra `09 - Peace at any price` (1,060). **Aries and Libra are the leanest signs** (avg 1,102 and 1,087); their "What it would give" cells are shorter.
- **Pre-modern pointers:** 106 of 130 sheets carry a pre-modern or classical pointer found by keyword (kakawin, *Desawarnana*, *Babad*, *Serat*, *Hikayat*, *Tambo*, *La Galigo*, inscriptions, lontar, manuscripts). Of the other 24, spot reads show several still hold older material under other names (Gemini Gossip: Bugis-Makassar *pappaseng*; Capricorn Hierarchy: the Gowa and Talloq chronicles; Pisces Fear: *Syair Lampung Karam*, 1883; Aries Anger: wayang figures and colonial *amok* reports). The leanest on pre-modern depth are Aries Autonomy, Initiative, Independence, Competition and Recklessness, Taurus Security, Virgo Work and Usefulness, Libra Fairness and Partnership, Sagittarius Education, Capricorn Responsibility and Leo Dignity, Generosity and Joy.
- No sheet reads as generic boilerplate; none is a "thin answer" sheet.

## Does the run exploit the nation's depth?
Largely yes for the big western peoples; thinner for the eastern islands and smaller Sumatran and Sulawesi peoples.
- **Scripts:** Arabic script (Jawi or Pegon) in 102 sheets; Javanese script (aksara Jawa) in 58; Han characters for Chinese-Indonesian terms in 50; Buginese *lontara'* in 6; Balinese script in 3; Sundanese script in 2; Batak, Rejang (*ka-ga-nga*) and Makasar scripts in none, though the Batak and Lampung/Rejang scripts and Balinese script are living or recently revived and central to manuscript work.
- **Peoples and regions** (sheets naming them, approximate keyword counts): Javanese 130, Balinese 120, Minangkabau 106, Sundanese 92, Bugis 91, Batak 90 (Toba 67, Karo 22, Mandailing 16, Simalungun 4), Chinese Indonesians about 80, Makassarese 74, Malay 72, Dayak 69 (Ngaju 16, Iban 6, Kenyah 5), Maluku 60 (Ambon 37), Madurese 58, Toraja 51, Sumba 50, Flores 45, Minahasa 44, Sasak 33, Betawi 25, Riau 24, Timor 23, Mandar 23, Banjar 23, Baduy 23, Bajau or Sama 17 to 24, Orang Rimba 16, Samin 12, Lampung 12, Mentawai 11, Osing 10, Tengger 10, Bima 10, Manggarai 10, Nias 9, Hadhrami Arabs 9, Rote 7, Kei 7.
- **Gaps:** Gorontalo, Buton, Muna, Wakatobi, Tanimbar and Sikka appear once each; Kaili, Tidore, Ternate, Alor and Lamaholot two or three times; Rejang, Kerinci, Tolaki, Bolaang Mongondow, Sangihe-Talaud, Banggai and Sabu never. North Maluku, Southeast and Central Sulawesi, the interior of southern Sumatra and the smaller Nusa Tenggara islands are the thinnest regions; the research stage should add them.

## Notes for the author
- Diaspora pointers were kept as comparison only.
- Sheets are unverified; every named item is marked *check*.
- No lesson-9 false positives arose: Sanskrit-derived Indonesian and Old Javanese words were kept and none tripped the scan.
- The run agent touched only Indonesia's `Springboards/` folders, appended Run log lines with `>>`, and wrote this report.
