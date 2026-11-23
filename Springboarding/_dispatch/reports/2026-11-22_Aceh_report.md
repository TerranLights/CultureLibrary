# Aceh: springboard run report (2026-11-22)

**Result:** 130 of 130 sheets done (12 signs, Aries to Pisces). There was one sub-agent per sign and one single-concept relaunch. The whole-nation QA scan (`springboard_qa.py Aceh`) found 0 problems in 130 sheets. The run agent's own repeat check found no copied line, table row, Flags line or "Who to compare" bullet between sheets (details below).

- **Wall clock:** 12:30 (start) to 16:41 (end), about 4 h 11 min (the Run log completion line rounds this to 16:45). There was no usage-limit stop. The run went past the usual 15:00 window because wave 3 was launched at 12:29.
- **Sub-agent tokens:** 2,893,361 in total. The 12 sign agents used 2,831,862 and the one fix relaunch used 61,499, over 674 tool uses. The later signs cost more (Capricorn 286k, Pisces 280k), because each sub-agent skimmed the earlier sheets to avoid repeats.
- **Lands:** the tracker header lists no settled lands ("to be settled by the author in Stage 0"; pre-war land "Indonesia"), and there is no `00 - Scope.md`.
  - The missing-scope note appears once per sign, in the Domain sheet only, and each of the 12 notes is worded differently.
  - No unit list was added, and `Hermes_research` was not opened.
- **Indonesia** appears only as comparison: national averages, national identity-card categories, and neighboring provinces as a yardstick. It is never Aceh's core.

## Per-sign table
| # | Sign | Sheets | Relaunches | QA | Avg words | Longest | Pointers (range, avg) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 0 | 0 | 1,141 | 1,269 (Domain) | 13-15, 14.0 | 173,721 | 12:32-12:46 |
| 2 | Taurus | 11/11 | 0 | 0 | 1,266 | 1,288 (Domain) | 14, 14.0 | 235,614 | 12:47-13:04 |
| 3 | Gemini | 10/10 | 0 | 0 | 1,210 | 1,282 (Domain) | 13-15, 14.0 | 216,285 | 13:04-13:19 |
| 4 | Cancer | 10/10 | 0 | 0 | 1,243 | 1,280 (Domain) | 13-14, 13.8 | 257,285 | 13:19-13:41 |
| 5 | Leo | 13/13 | 0 | 0 | 1,197 | 1,268 (Domain) | 13-15, 14.0 | 225,521 | 13:42-13:59 |
| 6 | Virgo | 10/10 | 0 | 0 | 1,226 | 1,299 (Domain) | 13-14, 13.9 | 209,548 | 14:00-14:14 |
| 7 | Libra | 11/11 | 0 | 0 | 1,222 | 1,293 (Domain) | 14-15, 14.4 | 233,350 | 14:16-14:34 |
| 8 | Scorpio | 11/11 | 0 | 0 | 1,249 | 1,278 (Rebirth) | 13-15, 14.1 | 227,236 | 14:36-14:52 |
| 9 | Sagittarius | 11/11 | 0 | 0 | 1,222 | 1,269 (Truth) | 14-15, 14.1 | 258,735 | 14:53-15:17 |
| 10 | Capricorn | 10/10 | 0 | 0 | 1,268 | 1,294 (Domain) | 13-14, 13.9 | 285,699 | 15:18-15:48 |
| 11 | Aquarius | 10/10 | 0 | 0 | 1,252 | 1,299 (Domain) | 14-15, 14.4 | 228,967 | 15:48-16:08 |
| 12 | Pisces | 12/12 | 1 | 0 | 1,224 | 1,286 (Domain) | 12-14, 13.5 | 279,901 + 61,499 fix | 16:09-16:40 |
| | **Total** | **130/130** | **1** | **0** | **1,226** | **1,299** | **12-15, 14.0** | **2,893,361** | **12:30-16:41** |

- **Word counts** are by `wc -w`. None is over 1,300. The longest are Virgo Domain and Aquarius Domain (1,299 each), and the shortest is Aries Competition (1,061).
- **Pointers** are the rows in "Where to look first", 1,820 in all. One sheet has 12 (Pisces Self-sacrifice). Thirteen sheets have 13, and the rest have 14 or 15.
- **Aquarius tokens:** the Run log line gives 228,003, an interim count. 228,967 is the final count.

## Rule breaks and fixes
- **Pisces Spirituality: a South Asian religion named on the Held line.** The line named the capital's temple of South Asian-heritage residents by its religion. The QA scan does not check for that word, and my own check caught it.
  - **Fix:** a single-concept relaunch rewrote the line as a category only, and it was fixed first time.
  - **Follow-on edit:** the relaunch also added a lands note to the sheet's Data flag, outside the Domain sheet, so I removed that one sentence by hand.
- **Aries Identity: near-copy.** Its Simeulue "Who to compare" bullet was a near-copy of the Aries Domain one. I reworded it by hand to a reason specific to Identity (how islanders answer "who are you", and whether *smong* stories enter that answer).
- **Virgo Domain: two near-copies.** Its lands note nearly repeated Leo's Domain note, and its "Comparison only" bullet nearly repeated Virgo Work's. I reworded both by hand, which left the sheet at 1,299 words.
  - **Prompt change:** from Libra on, the prompt told each sub-agent to word its lands note freshly for the sign.
- **Scorpio: done marked early.** The sub-agent reworded a few bullets in Domain, Death and Secrecy after marking them done. Their status lines are still accurate.
- **South Asian rule: judgment calls applied from Taurus or Sagittarius on** (for the author to confirm):
  - **The State Islamic University in Banda Aceh** carries a South Asian-born scholar's name. It is named only by description, as "the state Islamic university (UIN) in Banda Aceh", without the eponym.
  - **The scholar himself and his works** are never named. The folk expansion of the letters A-C-E-H is never cited.
  - **The Syattariyah Sufi order as practiced in Aceh** is kept as Aceh's own material: the lineage traced to Abdurrauf of Singkil, and the Nagan Raya community. No South Asian founder, saint or text of the order is named. This follows Thailand's court-Brahmin ruling and Indonesia's Balinese Hinduism ruling.
  - **South Asian-founded preaching and reform movements**, court-era scholars born in South Asia, arrival-of-Islam theories and the old port's South Asian-heritage traders and neighborhoods appear only as categories on Held lines.
  - **Rohingya boat landings** (2015 onward) are held as a category in Cancer Shelter and in one Sagittarius line ("refugee landings from camps there"), because the camps are in South Asia. This is cautious, since the Rohingya are from Myanmar. **The author may want these landings restored as ordinary pointers** in Shelter, Compassion and Boundary.
- **Held lines.** 123 of 130 sheets have a category-only Held line, each worded for its own concept. The other 7 say "none" or "nothing", each in its own words.
- **Law.** No law pointer appears outside Libra and Capricorn: the other signs send law questions to those two signs in a flag.
  - Scorpio Betrayal uses divorce-court filings and the flag-*qanun* dispute only as data on broken trust.
  - Libra keeps to the letter: the jinayat *qanun* and its procedure *qanun*, the sultanate's written rules (*Qanun Syarak Kerajaan Aceh*), and the *adat*-hearing handbook as written.
  - Capricorn keeps to the spirit: *Safinat al-Hukkam* read for purpose, invocations of the *Qanun Meukuta Alam*, attitude surveys, "peace money", and the rebel administration's claim on obedience.
- **Other checks.** The following appear nowhere: zodiac terms, URLs, "Indian" (for peoples or the ocean), the "Indo-" prefix, Human Universals or any universals list, Hermes_research, and findings phrases.
- **False matches on my own wider South Asian name pattern.** None of these is a South Asian item, and all are kept as written:
  - Acehnese *surat* ("letter");
  - "shackling" (the *pasung* rows), which my pattern read as a trader label;
  - *madrasah*.
  - The official scan had no lesson-9 false positives.

## Repeat check (nation-wide)
- **Exact matches.** No non-template line of 25 or more characters appears in two sheets. That covers table rows, compare bullets, Flags lines (including "Languages needed" and "Held for review") and first queries.
- **Near matches.** Among bullet lines, three pairs reach a similarity of 0.85 or more. Each gives a different reason, so I left all three:
  - Gemini Learning and Virgo Usefulness, Held lines: court teaching manuals vs. practical manuals.
  - Leo Dignity and Leo Generosity, Singkil bullets: respect at funerals and feasts vs. gifts at feasts.
  - Virgo Work and Virgo Health, Held lines: credit and hiring vs. remedies and healers.
- **Pointer reasons.** Among the 1,820 "What it would give" cells, no pair reaches a similarity of 0.8.
- **Recurring sources.** Nothing appears more than 4 times in 1,820 rows. The most frequent are:
  - *Hikayat Prang Sabi* (4 rows);
  - 3 rows each: Bowen, *Muslims through Discourse*; *Taj al-Salatin*; *Tajul Muluk*; *hadih maja* collections; Alfian, *Perang di Jalan Allah*; Schulze on GAM; Snouck Hurgronje, *Het Gajōland*; Hasan di Tiro's diary; *Hikayat Akhbarul Karim*; Balai Syura Ureung Inong Aceh.

## Thin, repetitive or generic sheets
- **Fewest pointers:** Pisces 03 Self-sacrifice (12). The 13-pointer sheets are Aries Domain; Gemini Duality; Cancer Shelter and Abandonment; Leo Honor; Virgo Perfectionism; Scorpio Purging; Capricorn Domain; Pisces Surrender, Intuition, Crime and Fear.
- **Shortest:** Aries 09 Competition (1,061), 06 Courage (1,084) and 04 Initiative (1,093). Aries ran shorter overall (avg 1,141) than later signs (1,197 to 1,268).
- **Thin compare bullets:** a few short ones in Aries are concept-specific but generic in shape, for example:
  - Initiative: "check island ventures against mainland ones";
  - Anger: "check island dispute-cooling; likely thin".
- **Formulaic Held lines:** the "... by South Asian-born scholars at the court, as a category only" pattern recurs in shape across many sheets. Each is worded for its concept, but the pattern is visible.
- **No Arabic script:** Gemini 03 Learning is the only sheet with no Jawi or Arabic-script term (129 of 130 have one).
- **Pre-modern pointers:** an automatic pass found 7 sheets without an obvious one. On reading, six have one under another spelling or form, for example:
  - Ma Huan, 1433, in Shelter; the Gunongan in Sensuality;
  - *Hikajat Potjoet Moehamat* in Anger and Group; the *Atu Belah* tale in Motherhood;
  - colonial bondage reports in Freedom.

  **Leo Play** has only oral and old-game pointers (*hiem* riddles, kites, tops), with no written pre-modern source.
- **No invented-looking names** turned up in the spot-checks (Aries Domain, Taurus Wealth, Libra Justice, Capricorn Law). Named items are well-known real works and institutions, for example:
  - Snouck Hurgronje, Siegel, Durie, Djajadiningrat's dictionary and Bowen;
  - Reid, Schulze and Aspinall;
  - Drewes's *Hikajat Potjoet Moehamat* and Teuku Iskandar's *Hikayat Aceh*;
  - Ma Huan and Tomé Pires;
  - Baitul Mal Aceh, Universitas Syiah Kuala, and *Serambi Indonesia*.

  All are marked *check*. Several studies are given as queries in Indonesian rather than as titles, as the brief asks when unsure.

## Does it exploit the nation's depth?
Largely yes for regions and the main peoples; thinner for the small minorities and settler groups.

- **Script and terms.** Jawi or Arabic script appears in 129 of 130 sheets. Acehnese terms appear in every sheet, and Gayo terms in most.
- **Regions.** Counts are sheets naming the region:

  | Region | Sheets |
  |---|---|
  | Banda Aceh / Aceh Besar | 130 |
  | Pidie | 128 |
  | North coast (Lhokseumawe, Aceh Utara, Bireuen, Pasai) | 124 |
  | West coast (Meulaboh, Calang, Nagan Raya, Aceh Jaya) | 115 |
  | Gayo highlands | 130 |
  | Alas / Southeast Aceh | 130 |
  | Singkil / Subulussalam | 128 |
  | Simeulue | 128 |
  | Sabang / Weh | 7 |

- **Peoples.** Counts are sheets naming the group:

  | Group | Sheets |
  |---|---|
  | Aneuk Jamee | 130 |
  | Tamiang | 125 |
  | Devayan / Sigulai | 114 |
  | Kluet | 100 |
  | Javanese settlers | 45 |
  | Chinese Acehnese (mostly Peunayong) | 41 |
  | Haloban / Pulau Banyak | 36 |
  | Batak and Pakpak in Southeast Aceh and Singkil | 16 |

- **Pre-modern and classical.** Counts are sheets naming the source:

  | Source | Sheets |
  |---|---|
  | *hadih maja* | 46 |
  | Snouck Hurgronje | 30 |
  | Abdurrauf of Singkil | 28 |
  | Hamzah Fansuri | 18 |
  | *Hikayat Prang Sabi* | 14 |

  Other pre-modern sources recur across the signs: *Hikayat Aceh*, *Tajul Muluk*, *Taj al-Salatin*, *Batu Aceh* gravestones, Pasai inscriptions, the *keuneunong* calendar, and the Chinese and Portuguese travel accounts.
- **Diaspora.** Acehnese in Malaysia and Scandinavia appear in 80 sheets, always as comparison only.
- **Weak spots:**
  - Sabang and Pulau Weh are almost absent.
  - Javanese settlers, Chinese Acehnese, and the Batak and Pakpak of the southern districts appear in under a third of the sheets.
  - Haloban appears in few sheets.
  - The *keuneunong* and other almanac material sits mostly in a few signs.
  - Siegel (5 sheets) is used sparingly, which suits variety but leaves Pidie's classic ethnography under-cited.
- **Scarcity.** The sheets flag thin data honestly for Simeulue, Kluet, Singkil, Alas and Tamiang, and point to the Acehnese and Gayo dictionaries, the Universitas Syiah Kuala and UIN repositories, and Aceh's manuscript collections. They do not pad with Indonesian material.

## Files touched
Only Aceh's `Springboards/` folders (12 sign folders, 130 sheets), Run log lines appended to `SPRINGBOARD_PROGRESS.md` with `>>`, and this report. Temporary files stayed in the run agent's own scratchpad folder.
