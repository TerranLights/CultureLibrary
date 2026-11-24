# Romania springboard run: report (2026-11-24)

**Result:** 130/130 sheets done (`springboard_status.py`). The whole-nation QA (`springboard_qa.py Romania`) finds **0 problems**. My own repeat check across the nation finds **0 exact repeats**: lines of 40 or more characters, table rows, "Who to compare" bullets, Flags lines and first queries, with the template's fixed header lines excepted. The same check against Bulgaria's and Hungary's sheets also finds 0 exact repeats.

Near matches at 0.85 in compare bullets, Flags lines and first queries: 5 remain, all in first queries. Each pair uses the same catalog with different search terms (details under "Thin, repetitive or generic sheets").

**Wall clock:** 10:08 (start) to 14:30 MST. Wave 2 of Tuesday 11-24.

**Sub-agent tokens:** 3,233,785 in all.
- 12 sign agents: 3,141,989
- 1 fix agent (Scorpio): 91,796

No usage-limit stop and no forced hand-back.

**Folder:** `Targets/Europe/Romania/Springboards/` (12 sign folders).

## Per sign

| # | Sign | Sheets | Agents | Fixes | QA | Avg words | Longest | Pointers | Tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 3 run-agent edits (short "Comparison only" bullets, near copies at 0.96) | 0 | 1,227 | 1,290 Domain | 14-16 | 175,631 | 10:09-10:24 |
| 2 | Taurus | 11 | 1 | 1 run-agent edit (the Domain's lands note named the scope file) | 0 | 1,184 | 1,296 Possession | 14-16 | 227,122 | 10:26-10:42 |
| 3 | Gemini | 10 | 1 | none | 0 | 1,241 | 1,280 Domain | 15-16 | 200,606 | 10:43-10:55 |
| 4 | Cancer | 10 | 1 | none | 0 | 1,267 | 1,289 Domain | 15-16 | 240,331 | 10:56-11:12 |
| 5 | Leo | 13 | 1 | 4 run-agent edits (Joy: two claim wordings and a 0.90 compare bullet; Self-expression: stereotype examples on its Held line) | 0 | 1,268 | 1,294 Leadership | 13-14 | 265,594 | 11:13-11:33 |
| 6 | Virgo | 10 | 1 | none | 0 | 1,279 | 1,299 Discernment | 13-14 | 309,291 | 11:34-11:58 |
| 7 | Libra | 11 | 1 | 1 run-agent edit (Reciprocity compare bullet; re-trimmed at 14:05, see below) | 0 | 1,274 | 1,295 Reciprocity | 13-15 | 283,867 | 11:59-12:21 |
| 8 | Scorpio | 11 | 1 + fix | fix agent: 6 sheets trimmed, 2 Held lines corrected | 6, then 0 | 1,287 | 1,297 Domain, Death, Secrecy | 13-15 | 302,105 + 91,796 | 12:22-12:50 |
| 9 | Sagittarius | 11 | 1 | 1 run-agent edit (Fundamentalism Held line) | 0 | 1,266 | 1,290 Faith, Belief | 13-14 | 268,115 | 12:51-13:16 |
| 10 | Capricorn | 10 | 1 | 2 run-agent edits (Ambition and Law Held lines) | 0 | 1,264 | 1,295 Law | 13-15 | 328,100 | 13:17-13:39 |
| 11 | Aquarius | 10 | 1 | 1 run-agent edit (the Domain's lands line, a 0.99 copy of Capricorn's) | 0 | 1,268 | 1,284 Group | 14-15 | 240,559 | 13:41-14:00 |
| 12 | Pisces | 12 | 1 | 1 run-agent edit (Escapism's Banat bullet) | 0 | 1,281 | 1,298 Escapism | 14-15 | 300,668 | 14:01-14:26 |

**Words (wc -w):**
- Average 1,258.
- Range 1,101 (Taurus Wealth) to 1,299 (Virgo Discernment).
- 117 sheets are over 1,200 words; none is over 1,300.

**Pointers per sheet:** 13 to 16, average 14.3.
- 18 sheets have 13
- 64 have 14
- 37 have 15
- 11 have 16

The count of pointers fell from 14-16 in the first four signs to 13-15 from Leo on, as the sheets grew wordier. A per-pointer reason ("What it would give") got longer, not thinner.

## Rule breaks and fixes

**QA flags.** QA flagged only Scorpio: 6 sheets were over 1,300 words (1,301 to 1,313).
- I relaunched the six flagged sheets as one fix agent.
- It tightened each to 1,278-1,280 words without dropping a row, bullet or query.
- In the same pass it corrected two Held lines (next item).

**False cross-references on Held lines.** In both cases the item named does not appear on the other sheet.
- Scorpio Purging said the Danube quarantine stations were "moved" to Virgo Health.
- Scorpio Power said the "parallel state" quarrel was "set out" in Purging.
- Capricorn Law said the same quarrel was "drawn on in Scorpio" (run-agent edit).
- I checked every other cross-sheet claim on a Held line by hand, and all are true: Pacepa in Leo Honor; informers in Betrayal; rich lists in the Taurus Domain; carols in Cancer Home; informal payments in Leo Dignity; the annulled election and situation testing in Libra Impartiality; the personal-space study in Taurus Sensuality.
- From Sagittarius on, the prompt said to check before claiming such a reference.

**South Asian Held lines described too closely.** Two lines were narrowed to the category only, as Hungary's run did:
- Sagittarius Fundamentalism: "one South Asian-derived movement that would have served as a high-control-group pointer"
- Capricorn Ambition: "the intergenerational income atlas named in the concept block", a South Asian-heritage scholar's dataset

**Claims and stereotypes:**
- Leo Joy: "the feast many call the year's most joyful" and "fast-growing churches" were made neutral. The sub-agent had flipped Joy to done before its own fix, and reported it.
- Leo Self-expression: its Held line quoted two regional-temperament jokes as examples. The examples are cut.
- Pisces Escapism: its Banat bullet claimed where "most *frontieriști*" aimed. It now says what to check.

**Copies:**
- Aries: three bare "Comparison only" bullets (Initiative, Competition, Recklessness; 0.96) now each give a concept-specific reason. From Taurus on, the prompt forbade bare comparison lists.
- Leo Joy's Csángó bullet (0.90 to Creativity's) is rewritten.
- Libra Reciprocity's Maramureș bullet (0.86 to the Domain's) is rewritten.
- Aquarius Domain's Lands line (0.99 to Capricorn's) is reworded.

**My own slip.** My Libra Reciprocity rewrite pushed that sheet to 1,310 words. The nation-wide check caught it at 14:05, and I shortened the bullet to bring the sheet to 1,295. Libra's QA was clean before and after.

**Scope-file mention.** The Taurus Domain's lands note said "there is no scope file". That clause is cut, and from Gemini on the prompt forbade it. The lands note appears once per Domain sheet, and in no concept sheet's Target line.

**STATUS not the last write.** Two sheets were edited after their STATUS flip:
- Sagittarius Fundamentalism was flipped at 1,307 words, set back to in progress, cut to 1,285 and flipped again.
- Leo Joy is the one noted above.

Every sheet is complete and the status grid is reliable.

**Pre-modern pointers.** Every sheet has at least one. My pattern scan missed 8, which I checked by hand:
- Cancer Home: Bartók's *colinde*
- Leo Play: Paul of Aleppo, 1650s
- Virgo Improvement: Vasile Lupu's Iași press
- Scorpio Control: *solomonari* lore
- Scorpio Revenge: the *Corbea* and *Novăceștii* ballads
- Sagittarius Travel: 18th-century *proschinitare*
- Pisces Empathy: *bocete* laments
- Pisces Intuition: Cartojan on the chapbooks

Four of these rest on oral traditions (carols, ballads, laments, *solomonari* lore), which the run prompt allowed. Bulgaria's run counted only written sources, so the two nations are not strictly comparable here.

**Other scans:**
- South Asian names: none named anywhere. The South Asian category appears only on Held lines (13 sheets, below).
- False positives: Turkish *gurur* ("pride", Leo Pride) matched the "guru" pattern in my own name scan; the QA script does not flag it.
- No "Indian", no universals, no Hermes_research, no zodiac words.
- No "indo-" term: the wider language family is named another way.

**Law:**
- Libra keeps to the letter of the law: Lupu's 1646 code, the 1855-56 emancipation laws, the Constitution, the codes, the High Court and ECHR rulings, and the 1946 and 2016-17 trials.
- Capricorn Law keeps to its spirit: *ius valachicum*, socialist legality, rule-of-law perception data, discretion, pardons, the lustration debate, *descurcăreală* and Tatar *adet*.
- Every other sign routes law to those two. The Roma *kris* (Gemini Mediation) is kept as custom, not law.

## Thin, repetitive or generic sheets

**No sheet is generic.** These are thinner than the rest:
- Taurus Wealth (1,101 words)
- Taurus Possessiveness (1,104)
- Sagittarius Honesty (1,179 words, 13 pointers)
- Pisces Empathy (1,232; its oldest pointer is oral)

**Repetitive frames that remain** (kept, since the search terms differ):
- 5 first-query pairs at 0.86-0.87. Each uses one search frame on the same catalog (the Brăiloiu sound archive twice, the Academy Library, Romanian ethnology journals twice).
- Many Held lines in Taurus end on the tail "nothing was held". Each still names its own item, and from Gemini on they are varied.
- Five Cancer, three Libra and two Aquarius Held lines share the idea "an outside frame was weighed and kept back", in different words and for different items.

**Repeated pointer.** Gheorgachi's 1762 *Condica de ceremonial* is a pointer in both the Leo and the Capricorn Domain sheets, with different reasons and wording.

## Does the run use the nation's depth?

Yes, broadly. Below is the number of the 130 sheets (and of the 12 signs) that name each item.

**Regions:**

| Region | Sheets | Signs |
|---|---|---|
| Moldavia/Iași | 129 | 12 |
| Dobruja | 125 | 12 |
| Banat | 122 | 12 |
| Maramureș | 119 | 12 |
| Oltenia | 117 | 12 |
| Bucharest | 116 | 12 |
| Muntenia | 112 | 12 |
| Bukovina | 112 | 12 |
| Danube Delta | 102 | 12 |
| Crișana | 91 | 12 |
| Sibiu and the Mărginimea | 91 | 12 |
| Apuseni and the Moți | 77 | 12 |
| Cluj | 76 | 12 |
| Jiu Valley | 69 | 12 |
| Constanța | 59 | 12 |
| Brașov | 51 | 12 |
| Hunedoara | 34 | 11 |
| Făgăraș | 33 | 10 |
| Alba Iulia | 31 | 9 |
| Oaș | 13 | 7 |

**Peoples and faiths:**

| People or faith | Sheets | Signs |
|---|---|---|
| Roma | 130 | 12 |
| Lipovans | 127 | 12 |
| Turks | 127 | 12 |
| Ukrainians | 126 | 12 |
| Tatars | 123 | 12 |
| Jewish community | 111 | 12 |
| Banat Swabians | 107 | 12 |
| Saxons | 106 | 12 |
| Serbs | 102 | 12 |
| Kalderash | 86 | 12 |
| Rudari/Boyash | 79 | 12 |
| Csángó | 77 | 11 |
| Ursari | 72 | 12 |
| Banat Bulgarians | 59 | 12 |
| Hutsuls | 58 | 12 |
| Pentecostals | 53 | 12 |
| Slovaks | 52 | 11 |
| Baptists | 48 | 11 |
| Greek Catholics | 46 | 12 |
| Armenians | 40 | 10 |
| Old Believers (by that name) | 36 | 11 |
| Adventists | 29 | 10 |
| Roman Catholics (by that name) | 20 | 10 |
| Czechs | 18 | 7 |

**Pre-modern sources named:**

| Source | Sheets |
|---|---|
| Ottoman and Phanariot records | 23 |
| Bukovina painted monasteries | 11 |
| Cantemir | 10 |
| Dosoftei and Varlaam | 9 |
| *Miorița* | 7 |
| Antim | 6 |
| Neculce | 6 |
| Miron Costin | 5 |
| Neagoe Basarab | 4 |
| Lupu's *Carte românească* | 4 |
| Transylvanian School | 4 |
| *colinde* | 4 |
| *doine* | 4 |
| Coresi | 3 |
| Ureche | 3 |
| *Supplex* | 3 |
| *Călători străini* | 3 |
| Neacșu's Letter | 2 |
| *Îndreptarea legii* and the *pravile* | 2 |

The many other pre-modern pointers are mostly charters, chronicles, travelers and oral genres given as queries.

**Weakest spots** (a future pass could push these):
- Oaș, Alba Iulia and Făgăraș as regions
- Czechs of the Banat
- Roman Catholic Romanians as a group of their own
- Armenians
- The named classics are spread thin. Neacșu's Letter and *Îndreptarea legii* appear on only 2 sheets each; most sheets reach the pre-modern through Ottoman-era records, monasteries or oral genres instead.

## Judgment calls for the author

1. **Lands:** there is no `00 - Scope.md`, and the tracker header settles nothing. So the sheets:
   - write for Romania as it stands
   - add no unit list
   - settle no borders
   - say once per Domain sheet that the lands are still to be settled

   **Open question:** the Hungarians of Transylvania and the Székely Land were treated as Hungary's row (comparison only), as the run instructions said. Please confirm this carve-out. Where Hungarian-language scholarship is one side of a contested Romanian topic (Csángó origins and language shift: Aries Identity, Pisces Dissolution), it is cited beside the Romanian side, as a claim.
2. **South Asian category, held on 13 sheets** (category only, nothing named):
   - Cancer Belonging
   - Virgo Health
   - Sagittarius Domain, Education and Fundamentalism
   - Capricorn Ambition
   - Aquarius Detachment
   - Pisces Dissolution, Escapism, Spirituality, Surrender, Intuition and Fear

   Several of these concern recently recruited foreign workers, the medical universities' students, and South Asian-derived wellness, meditation and divination practices. The Pisces sub-agent called its Escapism and Surrender holds the weakest calls. Please rule whether these topics should stay held.
3. **Buddhism (open question):** held as a category in 6 sheets: Taurus Sensuality, Scorpio Rebirth, Sagittarius Domain, Aquarius Detachment, and Pisces Dissolution and Spirituality.
4. **Items left on Held lines for the author to place:**
   - Budai-Deleanu's *Țiganiada*: it satirizes through Roma figures (Virgo Criticism).
   - Interwar far-right "spiritual renewal" texts (Virgo Improvement) and the Legionary "work camps" (Aquarius Community): how such texts are handled.
   - The *hizmet*-linked Turkish schools in Dobruja (Virgo Service).
   - The "prison saints" (Sagittarius Conviction).
   - Prophecy booklets of uncertain authorship (Virgo Discernment).
   - Hungarian-language Csángó field studies (Virgo Work).
   - The 1907 peasants' revolt: Equality or Reform (Aquarius Equality).
   - Children's-home survivors' accounts (Aquarius Friendship).
5. **Contested ground, presented as claims:**
   - the continuity and settlement accounts
   - *robie* and its records (dowry lists naming enslaved Roma are to be read as owners' papers, beside Roma accounts)
   - the Holocaust under Antonescu (the Iași pogrom trials, Transnistria)
   - Decree 770
   - Csángó identity
   - the Moldovan identity debate (comparison only)
   - the Securitate files, the 1989 revolution and the Mineriads
6. **Comparison only:** Moldova, the Aromanians, the diaspora (Italy, Spain, Germany, the UK, North America) and the neighboring culture-nations. Bulgaria's and Hungary's sheets were included in the repeat check: 0 exact repeats.
7. **False positive in my own scan:** Turkish *gurur* ("pride", Leo Pride) matched the "guru" pattern in my run-agent name scan (not the QA script). It is kept as written.
