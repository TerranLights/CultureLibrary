# South Africa: springboard run report (2026-11-22)

**Run agent:** one run agent, one sub-agent per sign (deeper brief), single-concept relaunches for fixes. **Wall clock:** 12:30 (start; first launch 12:32) to about 16:18 MST, about 3 h 48 min, with no usage-limit stop. **Lands:** the tracker header lists none ("to be settled by the author in Stage 0"; no `00 - Scope.md`), so the brief's missing-scope rule was followed: the lands note sits only in the Domain sheets, and no unit list was added. Nothing was taken from Hermes_research.

## Result
- **130 of 130 sheets done** (`STATUS: done 2026-11-22, not verified`), 12 sign agents and 3 single-concept relaunches (each passed the first time).
- **Whole-nation QA:** 130 sheets scanned, 1 flag, a false positive (see below).
- **Sub-agent tokens:** 2,859,038 in total (2,614,087 for the 12 sign agents plus 244,951 for the 3 fixes). The run agent's own tokens are not included.
- **Length:** average 1,210 words by `wc -w`, range 1,083 to 1,294; none over 1,300.
- **Pointers per sheet:** 13 to 16, average 14.3 (8 sheets with 13, 75 with 14, 45 with 15, 2 with 16).

## Per sign
| # | Sign | Sheets | Relaunches | QA problems and fixes | Avg words | Longest | Avg pointers | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 0 | none | 1,144 | 1,269 | 14.7 | 175,630 | 12:32-12:46 |
| 2 | Taurus | 11 | 1 | 09 Stubbornness: co-author of South Asian heritage (relaunch); 08 Possessiveness: *sikhwele* false positive (kept); 00 Domain: hand edit (below) | 1,219 | 1,277 | 14.1 | 293,675 | 12:47-13:05 |
| 3 | Gemini | 10 | 0 | none | 1,243 | 1,283 | 14.5 | 199,958 | 13:03-13:17 |
| 4 | Cancer | 10 | 1 | 07 Care: "reads like a finding" (relaunch) | 1,255 | 1,294 | 14.2 | 293,187 | 13:18-13:34 |
| 5 | Leo | 13 | 1 | 03 Pride: South Asian-origin surname (relaunch) | 1,186 | 1,260 | 14.0 | 287,932 | 13:33-13:49 |
| 6 | Virgo | 10 | 0 | none | 1,212 | 1,267 | 13.9 | 249,018 | 13:48-14:08 |
| 7 | Libra | 11 | 0 | none (law as letter only) | 1,216 | 1,254 | 14.1 | 222,823 | 14:09-14:23 |
| 8 | Scorpio | 11 | 0 | none | 1,220 | 1,280 | 15.1 | 251,192 | 14:24-14:45 |
| 9 | Sagittarius | 11 | 0 | none | 1,190 | 1,271 | 14.5 | 232,872 | 14:46-15:05 |
| 10 | Capricorn | 10 | 0 | none (law as spirit only) | 1,233 | 1,265 | 14.0 | 209,501 | 15:06-15:28 |
| 11 | Aquarius | 10 | 0 | none | 1,215 | 1,268 | 14.2 | 220,904 | 15:28-15:46 |
| 12 | Pisces | 12 | 0 | none | 1,199 | 1,270 | 14.5 | 222,346 | 15:47-16:07 |

## Rule breaks and fixes
1. **Taurus 09 Stubbornness (South Asian rule; the scan does not catch names):** a Cape Muslim pointer (the book on Imam Abdullah Haron) had a co-author of South Asian heritage. Single-concept relaunch: the Haron story now comes through a Cape Muslim oral-history and archive route, given as a source type and a query.
2. **Cancer 07 Care (findings):** a "Who to compare" bullet ended "as fiction and labor studies show it". Relaunched: the bullet now names only what to check, and other cells that took a result for granted were reworded.
3. **Leo 03 Pride (South Asian rule, a conservative call):** a standard work on Coloured identity by a scholar whose surname is of South Asian origin. Relaunched and replaced by another real pointer on Coloured identity (*check*). The author may want to decide whether such surnames fall under the rule.
4. **Taurus 00 Domain (scope-file rule):** its Data flag said "No scope file exists yet". Hand edit: that clause was cut, and the lands note stays.
5. **False positive kept:** Taurus 08 Possessiveness, siSwati/isiZulu *sikhwele* ("jealousy"), matches the scan's "sikh" pattern. It is kept as written, and it is the whole-nation QA's only flag.
6. **After each sign I read every pointer name** for South Asian-heritage scholars, writers, communities and religions. Nothing else was found. Each sheet has exactly one "Held for review" line, worded as a category with its own concern (130 lines). The words "Indian", "Bushmen", "Hottentot", the universals lists and the banned divination words appear nowhere.
7. **Law:** law material appears only in Libra (statutes, cases, commissions as written) and Capricorn (legal culture, obedience, discretion). Other signs refer to those two signs.

## Repeat check (whole nation)
- **Verbatim repeats:** no line, table row, "Who to compare" bullet or Flags line appears in two sheets. Every line of 25 characters or more was compared across all 130 sheets.
- **Near-repeats:** a fuzzy pass over all compare and Flags bullets found one pair above 0.75 similarity: Taurus 05 Security and Cancer 05 Protection (0.82). Both point at the same Cape Flats neighborhoods, but each says what to check for its own concept, so the pair was left as is. The Aquarius sub-agent's own stricter scan found 5 reworded lines at 0.60 to 0.68 similarity to lines in other signs. Each gives its own reason.
- **Sources:** standard works recur across signs, but never as a copied row. Seven sources appear in 5 sheets each: Afrobarometer, World Values Survey, District Six Museum, Stayt's *The Bavenda*, Yap and Leong Man's *Colour, Confusion and Concessions*, Krog's *Country of My Skull*, and the Carnegie poor-white report (4 sheets). This is acceptable, but the later research should not read these as the core canon for every concept.

## Thin, repetitive or generic sheets
- **Shortest (still between 1,083 and 1,130 words):** these are all Aries sheets (03 Autonomy, 04 Initiative, 08 Anger, 09 Competition, 07 Independence), written under the first sign, before the later signs grew longer. They are compact, not thin.
- **13 pointers:** Taurus 08 Possessiveness, Leo 11 Honor, Virgo 06 Perfectionism and Virgo 09 Improvement, and the Domain sheets of Cancer, Virgo, Sagittarius and Aquarius.
- **Formulaic:** the Held lines share one sentence shape by necessity ("... of South Asian-heritage communities in the nation's lands, ..."), though each names its own concern.

## Whether the sheets use the nation's depth
Mostly, yes. Every sheet has terms in isiZulu, isiXhosa and Afrikaans, and nearly every one in Sesotho, Setswana and Kaaps (124 of 130). Sepedi, Xitsonga and Tshivenda appear in 115 to 120 sheets. The pre-modern layer recurs: the Bleek and Lloyd notebooks, the James Stuart Archive, izibongo and lithoko, rock art, Mapungubwe, Blombos, the VOC *Daghregister* and Cape slave records, and Callaway and Junod. Khoe and San pointers are in about 100 sheets, Nama in 60 and Griqua in 27. Jewish South Africans are in 70 sheets, Chinese in 60 and Portuguese in 48.

**Weaker spots (sheets of 130 that name the group or place):**
- amaSwati: 15
- English-speaking South Africans, as a named group: 20
- amaNdebele: 22
- Cape Malay by that name: 23 (Cape Muslim: 53)
- Mpumalanga: 48
- North West: 54

Limpopo, Gauteng and the Eastern Cape are the most covered. These gaps should get attention when the research starts.

## For the author
- **Lands:** still to be settled in Stage 0. The sheets are written for the present-day provinces.
- **The surname call:** see fix 3. Should a scholar with a South Asian-origin surname but no known community tie fall under the strict rule? This run treated such scholars as covered.
