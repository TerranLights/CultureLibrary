# Philippines springboard run: report (2026-11-21)

**Result:** 130 of 130 sheets done (all `STATUS: done 2026-11-21, not verified`), twelve signs, Aries to Pisces, one sub-agent per sign under the deeper brief. One usage-limit interruption (Capricorn). No QA relaunches; no hand edits. Whole-nation QA: 2 flags, both false positives (the Tagalog negator *hindi*), kept as written.

**Wall-clock:** run agent start 08:02 MST, end 12:21 MST (4 h 19 min), of which about 68 min (about 10:35 to 11:43) was the stop forced by the 5-hour usage limit; working time about 3 h 11 min.

**Total sub-agent tokens: about 2,491,566** (13 agents: 12 sign agents plus the Capricorn resume agent). The cut-off Capricorn agent's 163,967 is an estimate read from its transcript (no usage report came back after the cutoff); without it the reported total is 2,327,599. The run agent's own tokens are not included.

**Lands:** the tracker header lists no settled lands and there is no `00 - Scope.md`. Per the brief's missing-scope rule, each sign's Domain sheet says once that the nation's exact lands are still to be settled and the sheets are written for the core archipelago; no unit list was added; `Hermes_research` was not opened.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words (wc -w) | Longest | Shortest | Pointers (avg) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,171 | 1,284 Domain | 1,101 Competition | 14-16 (15.3) | 184,117 | 08:03-08:19 |
| 2 | Taurus | 11/11 | 1 | 0 | 1 false positive | 1,187 | 1,290 Domain | 1,087 Stubbornness | 14-16 (15.5) | 194,695 | 08:20-08:34 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,195 | 1,270 Domain | 1,127 Duality | 15-16 (15.1) | 185,704 | 08:34-08:47 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,203 | 1,265 Home | 1,149 Shelter | 14-15 (14.6) | 204,205 | 08:47-09:02 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,073 | 1,231 Domain | 1,023 Joy | 14-16 (15.0) | 206,497 | 09:02-09:18 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,107 | 1,193 Domain | 1,057 Criticism | 15-16 (15.6) | 194,377 | 09:18-09:32 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,214 | 1,260 Domain | 1,150 Indecision | 14-16 (14.4) | 213,018 | 09:33-09:48 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,156 | 1,275 Domain | 1,092 Betrayal | 14-16 (15.5) | 198,190 | 09:48-10:02 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,163 | 1,267 Faith | 1,064 Honesty | 15-16 (15.6) | 197,038 | 10:02-10:17 |
| 10 | Capricorn | 10/10 | 2 (cutoff + resume) | 0 | 0 | 1,224 | 1,287 Law | 1,136 Hierarchy | 14-16 (15.0) | about 163,967 + 137,747 | 10:18-10:35, 11:43-11:49 |
| 11 | Aquarius | 10/10 | 1 | 0 | 1 false positive | 1,152 | 1,251 Domain | 1,108 Friendship | 14-15 (14.7) | 207,474 | 11:50-12:04 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,127 | 1,226 Domain | 1,050 Escapism | 15-16 (15.1) | 204,537 | 12:04-12:19 |
| | **Nation** | **130/130** | **13** | **0** | **2 false positives** | **1,162** | 1,290 | 1,023 | 14-16 (about 15.1) | **about 2,491,566** | |

Pointers per sheet across the nation: 23 sheets with 14, 69 with 15, 38 with 16 (counted as table rows under "Where to look first").

## Interruption (Capricorn)
The Capricorn sign agent (launched 10:18) was stopped at about 10:35 by the 5-hour usage limit, with the Domain sheet and concepts 1 to 6 done and Merit half-written (`STATUS: in progress`). After the reset the run resumed at about 11:43: a resume agent wrote only Merit (completing the half-written sheet), Law and Order; no done sheet was redone. Merit (1,280) and Law (1,287) run over the brief's guide of about 1,200 but under the 1,300 scan limit.

## Rule breaks and fixes
- **QA flags (2), both false positives, kept as written:** Taurus `09 - Stubbornness.md` line 17 (*hindi papatalo*) and Aquarius `02 - Group.md` line 15 (*hindi ibang tao*). *Hindi* is the ordinary Tagalog negator ("not"); the scan's South Asian pattern catches it, as it caught "sikh" inside Caucasus words. **Suggestion for the author:** the scan pattern for "hindi" will catch most Filipino sheets on other concepts too (Tagalog uses it constantly); a word-boundary exception for Tagalog contexts, or a per-nation allowlist, would stop these.
- **Held for review lines:** Libra Reciprocity and Scorpio Trust each set one informal-lending pointer aside, worded as the category only ("South Asian-heritage communities in the nation's lands"). Aries Domain and Identity carry the same category line. No South Asian work, scholar, community or language appears elsewhere; sub-agents were told not to give South Asian etymologies for Philippine words.
- **No law outside Libra and Capricorn** was flagged; Capricorn's Law sheet was briefed for the spirit of law.
- **No zodiac words, no "Indian", no findings phrases** were flagged.
- **Checkpoint order:** no slips reported.

## Repetition
- **Within signs:** 0 shared lines between sheets of any sign, beyond the template's fixed lines and the held-for-review category line.
- **Across the nation:** 2 shared table rows, both search-term glosses repeated between Aries `07 - Independence` and Sagittarius `03 - Freedom` (Ilocano *wayawaya* and Hiligaynon *kahilwayan*, "freedom"). Different agents, overlapping concepts; minor, not edited.
- **Most reused sources** (sheets naming them, of 130): William Henry Scott, *Barangay* (11); Fenella Cannell, *Power and Intimacy in the Christian Philippines* (9); Philippine Center for Investigative Journalism (7); World Values Survey, Wilfredo Magno Torres III (ed.), *Rido*, Pedro Chirino, *Relación*, and Michael L. Tan on *usog*/*pasma*/*kulam* (6 each); then about twenty sources at 4 or 5 (Ileto, *Pasyon and Revolution*; Majul, *Muslims in the Philippines*; Morga, *Sucesos*; Plasencia; the Boxer Codex; Blair and Robertson; Enriquez; Constantino; Parreñas; Hart, *Compadrinazgo*; the YAFS and LSAHP surveys; the CBCP; PITAHC; Balagtas). Spread over 130 sheets, this is variety, not a few sources filling every sheet.

## Thin, repetitive or generic sheets
- **Leo is the thinnest sign** (avg 1,073 words; every concept sheet 1,023 to 1,202). Its "What it would give" cells are shorter and lean on festivals and popular media; `12 - Joy`, `03 - Pride`, `11 - Honor`, `07 - Humiliation` and `08 - Generosity` give the least reason per pointer. Still 14 to 16 pointers each and no rule breaks; a later researcher should expect to widen them first.
- **Virgo** (avg 1,107) is the next shortest; `07 - Criticism` and `06 - Perfectionism` are the leanest.
- No sheet reads as generic boilerplate; none is a "thin answer" sheet.

## Does the run exploit the nation's depth?
Mostly yes, with gaps worth naming.
- **Scripts:** Baybayin forms in 129 of 130 sheets (all but Taurus `02 - Ownership`), marked as the revived modern rendering, *check*; Arabic-script (Jawi) terms for Maranao, Maguindanaon and Tausug in 63 sheets; Han characters for Philippine Hokkien in 92. Hanunoo Mangyan script appears in only 1 sheet, Buhid and Tagbanwa scripts in none, though all three are living Philippine scripts. Caution: Baybayin spellings of modern Tagalog (and especially of other languages) are a revival convention, not period usage.
- **Pre-modern:** 98 of 130 sheets carry a marked pre-modern or classical pointer (the Boxer Codex, Plasencia, Chirino, Alcina, Morga, Loarca, the *Doctrina Christiana*, the early *Vocabulario* dictionaries, the Laguna Copperplate, and epics such as *Hudhud*, *Darangen*, *Biag ni Lam-ang*, *Hinilawod*, *Ibalong*).
- **Minorities and regions** (sheets naming them): Cebuano 129, Ilocano 121, Maranao 119, Hiligaynon 116, Tagalog 113, Tausug 107, Lumad 101, Hokkien/Chinese Filipinos 96, Maguindanaon 91, Sama 70, Ifugao 58, Mangyan 53, Kapampangan 52, Bikol 46, Waray 45, Agta 45, Kalinga 43, Bontoc 34, Kankanaey 30, Manobo 28, T'boli 26, Palawan 25, Aeta 24, Pangasinan 23, Yakan 21, Subanen 21, Ibaloi 20, Ivatan 20, Teduray 16, Higaonon 16, Chavacano 13, Bajau 13, Kinaray-a 12, Ati 11, Bugkalot/Ilongot 10, Mandaya 9, Batak 8, Bagobo 8, Tagbanwa 7, Isneg 5, Itneg/Tingguian 5, Blaan 3, Sambal 2.
- **Gaps:** the Cagayan Valley peoples (Ibanag, Gaddang, Yogad, Isinai), Kalanguya, Surigaonon, Mansaka, Tagakaulo and Matigsalug are never named; eastern Mindanao and the northeast of Luzon are the thinnest regions. The research stage should add them.

## Notes for the author
- Diaspora pointers were kept as comparison only.
- Sheets are unverified; every named item is marked *check*.
- The run agent touched only the Philippines `Springboards/` folders, appended Run log lines with `>>`, and wrote this report.
