STATUS: done 2026-11-22. Run agent's report; the sheets are unverified.

# United Kingdom: springboard run report (deeper brief)

**Result:** all 130 sheets are done, and every first line reads `STATUS: done 2026-11-22, not verified`. The run used 12 sign agents and needed no relaunch. The whole-nation QA (`springboard_qa.py "United Kingdom"`) found **0 problems** in 130 sheets. The run agent made 8 small hand edits, listed below.

**Tokens and wall-clock:**
- **Sub-agent tokens:** **2,202,729**, as reported by the harness for the 12 sign agents, with 464 tool uses. The run agent's own tokens are not included; the main session adds them.
- **Wall-clock:** the run agent started at **08:36:03 MST**. The Aries agent launched at 08:37, and the Pisces agent finished at 11:38. The checks and this report were done by **about 11:52 MST**, so the run took **3 h 16 min** in all.
- **No stops:** the run hit no usage limit.
- **Time per sign:** 10.3 to 17.3 minutes, with the signs run one after another.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,219 | 1,288 (Domain) | 15.5 (15-16) | 180,426 | 08:37-08:52 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,184 | 1,276 (Possession) | 15.5 (15-16) | 200,673 | 08:53-09:07 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,207 | 1,265 (Domain) | 14.8 (14-16) | 183,639 | 09:08-09:20 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,166 | 1,269 (Domain) | 15.6 (14-16) | 195,635 | 09:21-09:34 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,227 | 1,291 (Domain) | 14.3 (14-15) | 212,199 | 09:35-09:51 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,176 | 1,290 (Domain) | 16.0 (16) | 189,535 | 09:52-10:04 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,213 | 1,280 (Domain) | 14.8 (14-15) | 213,601 | 10:05-10:19 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,219 | 1,281 (Rebirth) | 14.3 (13-16) | 217,365 | 10:20-10:36 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,224 | 1,277 (Domain) | 15.4 (14-16) | 216,850 | 10:37-10:54 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,198 | 1,263 (Law) | 14.6 (14-15) | 177,580 | 10:55-11:05 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,234 | 1,286 (Domain) | 15.0 (15) | 215,226 | 11:06-11:22 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,230 | 1,288 (Dissolution) | 15.0 (13-16) | 210,628 | 11:23-11:38 |
| | **Total** | **130** | **12** | **0** | **0** | **1,209** | **1,291** | **15.0 (13-16)** | **2,202,729** | **08:37-11:38** |

- **Word counts:** by `wc -w`, markup included, counted before the hand edits (each edit changed a sheet by only a few words).
  - The shortest sheet is Taurus/Possessiveness, at 1,107 words.
  - The longest is Leo/Domain, at 1,291.
  - 68 sheets run between 1,200 and 1,291 words, and none is over the 1,300 flag.
- **Pointers:** these are the rows of section 2.
  - 37 sheets have 16, 65 have 15, 24 have 14 and 4 have 13.
  - The four with 13 are Scorpio Betrayal, Revenge and Secrecy, and Pisces Intuition.

## Rule breaks and fixes
**QA:** the scan flagged nothing in any sign or in the whole-nation pass:
- no zodiac, divination-label or horoscope words;
- no "Indian" and no "Indo-" words;
- no URLs;
- no findings phrasing;
- nothing from Hermes_research.

**South Asian rule:** this follows the main session's correction, sent before any sub-agent launched. Every sub-agent prompt left out the original "British South Asian" item and stated the brief's rule strictly, with the India Office Records named as a case.
- No sheet names a South Asian work, scholar, community, language, archive or place outside the Held line.
- Every one of the 130 sheets carries a category-only Held line. In 65 it is the brief's bare line, and in 65 it is a concept-specific variant that still names only the category, such as "housing and home-ownership studies of South Asian-heritage communities in the nation's lands".
- Sagittarius's prompt also barred naming any South Asian religious community or temple. Its Muslim pointers are Somali, Yemeni, Arab, Turkish, Kurdish, Bosnian and Moroccan communities.

**Lands:** the tracker header lists no settled lands, and there is no `00 - Scope.md`.
- The lands note appears once in each sign's Domain sheet (12 of 12) and in no other sheet. Each note is worded differently.
- No sheet tells the reader to read a scope file, and no unit list was added.
- The sheets are written for Great Britain's core lands (England, Scotland, Wales and their islands).

**Northern Ireland:** it appears only as a comparison, never as the core.
- Taurus carried a Northern Ireland bullet on all 11 sheets. Each bullet gave its own reason, but the pattern was formulaic.
- From Gemini on, the prompt said to name it only where it sharpens the concept. After that it appears on 1 or 2 sheets per sign, mostly the Domain.

**Isle of Man and Channel Islands:** they are named only as nearby comparisons (Leo Leadership, and Libra's prompt), never as part of the nation.

**Law:** law content stays in Libra (the letter of the law) and Capricorn (the spirit), with Scots law kept apart from the law of England and Wales.
- In the other signs, law appears only as a redirect, for example in Virgo's Health, Improvement and Criticism flags and in Leo Recognition.

**Hand edits by the run agent (8, each the smallest edit):**
1. Aries Independence: a Gypsy, Traveller and Showpeople compare bullet stated a group attitude. It now names the threads to check by community.
2. Taurus Stability: a Gypsy, Roma and Traveller compare bullet stated a group trait. It is reworded the same way.
3. Taurus Wealth: a second Gypsy, Roma and Traveller trait bullet, reworded the same way.
4. Taurus Sensuality: a Somali and Yemeni compare bullet stated a group trait. It is reworded the same way.

   After these four edits, every prompt from Gemini on carried a no-stereotype line. It said a compare bullet names what to separate and check, never a trait.
5. Scorpio Secrecy: a bullet grouped Hong Kong arrivals with "insecure status". It now names Vietnamese arrivals and keeps the BN(O) route apart.
6. Sagittarius Meaning: a Hebridean bullet stated a trait. It is now a source of meaning to check, township by township.
7. Aquarius Community, first query 4: it copied Gemini Information's query word for word, and is rewritten for the concept.
8. Libra Reciprocity, first query 4: it nearly repeated Gemini Connection's pardner query, and is rewritten.

**Prompt hygiene:**
- Before launch, the run agent took two examples out of its own Pisces nudge list because they invited stereotypes: Traveller fortune-telling, and "drinking cultures" by region. The list now asks for alcohol and drug-harm data compared by measured figures.

## Repetition
**Exact lines:** across the 130 sheets, no line of 40 or more characters repeats, apart from:
- the template's three fixed lines;
- the brief's category-only Held line.

That covers every table row, "Who to compare" bullet and Flags line, including "Languages needed".

**Near-duplicates:** after the fixes, a 3-word-sequence check flags 7 pairs of lines at a similarity of 0.4 or more. None is a copy. They are:
- the same source given in two sheets with different reasons (for example Savage's *Social Class in the 21st Century* in Taurus Wealth and the Capricorn Domain);
- first queries that search the same catalog for different terms;
- two Northern Ireland bullets in Leo with different reasons.

**Most-reused sources** (sheets that name them, out of 130):

| Source | Sheets |
|---|---|
| Bosworth-Toller (Old English dictionary) | 45 |
| Tobar an Dualchais | 21 |
| Mass Observation | 17 |
| British Social Attitudes | 17 |
| Black Cultural Archives | 11 |
| the Opies | 10 |
| *Carmina Gadelica* | 8 |

Nothing else reaches 8. Bosworth-Toller is a search-term source, used for the Old English gloss, and is almost never a pointer row.

## Thin, repetitive or generic sheets (by name)
**Leanest pointer counts (13):**
- Scorpio Betrayal, Revenge and Secrecy;
- Pisces Intuition.

Leo (avg 14.3) and Scorpio (14.3) are the leanest signs. Virgo is the fullest (16 on every sheet).

**Pre-modern depth:** every sheet has at least one pointer from before 1800.
- **Pisces Escapism** is the weakest. Its oldest pointer is a study of "Saint Monday" from 1766 on, with nothing medieval or early modern.
- **Pisces Empathy** rests on Hume (1739) and Smith (1759). These are classical but not pre-modern in the strict sense.
- **Aries Initiative, Gemini Communication and Aquarius Community** each rest on a single pre-modern pointer: the Paston Letters in the first two, and Morebath's parish records with the Victoria County History in the third.

**Languages:**

| Language | Sheets with search-term rows |
|---|---|
| Scottish Gaelic | 130 |
| Welsh | 130 |
| Scots | 124 |
| Old English | 117 |
| Middle English | 90 |
| Cornish | 85 |
| Romani, Angloromani or Cant | 44 |
| Norn, Shetland or Orcadian dialect | 15 |

The last two are the gaps. British Sign Language (BSL) appears as a community, not as a source of terms.

**Groups and regions (sheets naming them):**
- **Well spread:** Gypsy, Roma and Traveller communities (about 70), British Caribbean (67), Shetland (64), Irish in Britain (61), Jewish communities (61), Cornwall (54), British Chinese (54), Orkney (51), Polish (45), the Welsh valleys (40), Hong Kong arrivals (38).
- **Thin:** Yemeni (8), Tyneside (9), Deaf communities (11), Cypriot (13), Nigerian (14), Vietnamese (14), the North East named as such (18).

**Formulaic patterns:**
- The Taurus Northern Ireland bullets, fixed from Gemini on.
- Every sheet's Held line. It is always category-only, but it appears on all 130 sheets, where other nations' runs used "none" on most.

## Pointers per sheet
| Pointers | Sheets |
|---|---|
| 16 | 37 |
| 15 | 65 |
| 14 | 24 |
| 13 | 4 |

The average is 15.0, and every sheet is within the brief's 12 to 16. The per-sign averages are in the table above.

## Do the sheets exploit the nation's depth?
**Mostly yes.**

**Where the sheets are strong:**
- **The four language traditions:** English (with Old and Middle English), Scots, Scottish Gaelic and Welsh are worked on almost every sheet, with Cornish on two thirds.
- **Regional splits:** England's regions are split finely, for example the Black Country, the Fens, Teesside, the Potteries and Cumbria. Scotland is split Highland, Lowland and island (Lewis and Harris against Barra and South Uist, Orkney against Shetland). Wales is split north-west against the valleys, and along the Landsker line.
- **Pre-modern pointers:** these run across the record. Examples are the Anglo-Saxon law codes, *Y Gododdin*, the *Mabinogion*, *Cyfraith Hywel*, *Regiam Majestatem*, the Paston Letters, the Border March laws, the Flyting of Dunbar and Kennedy, the Lyke-Wake Dirge and the Survey of Scottish Witchcraft.
- **Two legal systems:** the separate Scots legal system is handled correctly in Libra and Capricorn.
- **Minority coverage:** it goes well beyond the best-known groups. It reaches Romanichal, Irish Traveller, Scottish Traveller, Showpeople and New Traveller communities kept apart, Haredi and Sephardi communities, Butetown and South Shields seafarers, Hong Kong arrivals since 2021, Ukrainian arrivals since 2022, Kurdish and Alevi communities, Cypriots and Deaf BSL users.

**Where depth could still be added later:**
- Norn and Shetland or Orcadian dialect terms.
- Angloromani and Cant vocabulary.
- The North East and Tyneside as a region in their own right.
- Yemeni, Vietnamese and West African communities beyond a few sheets each.
- A medieval or early-modern pointer for Pisces Escapism.
