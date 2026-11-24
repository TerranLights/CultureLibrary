# Quebec springboard run: report (2026-11-24)

**Run agent:** one per nation, deeper brief (accuracy and depth first), one sub-agent per sign, Aries to Pisces in order. Tuesday wave 2.
**Result:** 130/130 sheets `STATUS: done 2026-11-24, not verified` by `springboard_status.py`; whole-nation `springboard_qa.py Quebec`: **130 sheets scanned, 0 problems**. No relaunches. The run agent made 7 small edits by hand (listed below). No usage-limit stop and no forced hand-back.
**Wall clock:** start 10:08 (first launch 10:11), last sub-agent back 14:05, report 14:10.
**Sub-agent tokens:** **3,126,389** (12 sign agents, 0 relaunches; 827 tool uses).

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers | Tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,201 | 1,277 (Domain) | 15-16 | 178,584 | 10:11-10:24 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,232 | 1,285 (Domain) | 14-16 | 199,586 | 10:26-10:38 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 1,254 | 1,286 (Communication) | 13-16 | 212,603 | 10:37-10:50 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,270 | 1,299 (Abandonment) | 14-15 | 269,982 | 10:51-11:12 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,197 | 1,299 (Domain) | 13-16 | 237,193 | 11:13-11:29 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,220 | 1,268 (Domain) | 13-14 | 239,351 | 11:30-11:46 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,221 | 1,276 (Domain) | 12-14 | 254,974 | 11:46-12:02 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,224 | 1,277 (Domain, Death) | 12-13 | 255,477 | 12:03-12:25 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 1,238 | 1,276 (Faith) | 13-15 | 251,379 | 12:25-12:45 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1,225 | 1,282 (Duty) | 12-15 | 345,863 | 12:46-13:13 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1,220 | 1,264 (Reform) | 12-14 | 331,396 | 13:14-13:37 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,228 | 1,252 (Self-sacrifice) | 13-14 | 350,001 | 13:38-14:05 |
| | **Total** | **130** | **12** | **0** | **0** | **1,227** | 1,299 | 12-16 | **3,126,389** | |

Word counts by `wc -w`: 1,095 (Aries Competition) to 1,299 (Cancer Abandonment, Leo Domain); none over 1,300, but most sheets sit above the brief's "about 1,200" guide (Cancer averages 1,270). Pointers per sheet (table rows in section 2): 12 in 8 sheets, 13 in 42, 14 in 42, 15 in 26, 16 in 12. **The count drifts down through the run:** 15-16 in Aries, 12-14 from Libra on. Every sheet still meets the 12-to-16 band, but the later signs are at its low end.

## Rule breaks and fixes
- **QA scan:** 0 problems in every sign and for the whole nation; no relaunch was needed.
- **Run-agent smallest edits (no content lost; status lines untouched):**
  1. Libra *Partnership* and *Reciprocity*: the Held lines described the topic of the set-aside South Asian item (a marriage-formation topic; a savings-circle and elder-support topic). Both were cut to the category only. From Scorpio on, the prompt said the Held line gives no topic, study type or practice.
  2. Capricorn *Ambition*: the Held line named two US mobility datasets known by a South Asian-heritage scholar's project, while explaining why they were left out. It was cut to "work by scholars of South Asian heritage (category only)". The names appear nowhere else in the nation's sheets. From Aquarius on, the prompt said a Held line never names the set-aside item.
  3. Pisces *Dissolution*: the Buddhism Held line described the held pointer ("meditative self-loss", "contemplative community"). It was cut to the category only.
  4. Domain lands notes in Cancer, Sagittarius and Pisces said that "no scope file" exists. They were reworded to say the lands are not yet settled, without naming a scope file. The brief bars pointing the reader to the scope file.
- **Process slip (no effect on content):** the Aries sub-agent reworded four compare bullets and one Held line (in Identity, Courage, Anger and Competition) after marking those sheets done. From Taurus on, the prompt said the done mark is the very last write. Later sub-agents that reopened a sheet re-marked it done afterwards (Leo *Self-expression*, Sagittarius *Belief*).
- **South Asian rule:** the run agent's own name scan covered scholars, writers, works, communities, religions, place names and "Indo-". It was clean in all 130 sheets outside the Held lines. The South Asian category is held on 7 sheets: Leo *Self-expression* and *Honor*, Libra *Partnership* and *Reciprocity*, Sagittarius *Domain*, Capricorn *Ambition* and Pisces *Spirituality*. All of these are category only. **False-positive notes:** "Park Extension" / "Parc-Extension" appears 3 times: as a renters' district in Taurus *Ownership*, and as the historic Greek neighborhood in Leo *Play* (backgammon cafés) and Leo *Honor* (Greek *filotimo*). None of these names a South Asian community, so they were kept. The Gemini sub-agent's spelling check caught "Centre" only in French proper names (Centre québécois de la déficience auditive, Radio Centre-Ville, Centre d'études sur les médias, Centre-du-Québec), which were kept as published.
- **Buddhism (open question for the author):** it is held as a category, with nothing named, on 9 sheets: Scorpio *Death* and *Rebirth*; Sagittarius *Domain*, *Faith* and *Belief*; Capricorn *Discipline*; Aquarius *Detachment*; Pisces *Dissolution* and *Spirituality*. Scorpio *Death*'s Held line says that the funeral rites in question are those of "Vietnamese and other" communities. Pisces *Spirituality* keeps a pointer to Vietnamese household ancestor altars in Montreal, worded "apart from any temple". **For the author:** check whether the ancestor-altar pointer is acceptable under the Buddhism ruling, since the two practices are often entwined.
- **"Indian", universals, Hermes, zodiac words:** none in any sheet. Native peoples are named by their own names first.
- **Law:** Libra keeps the letter of the law (statutes in LégisQuébec, the referendum statute, courts and tribunals as written). Capricorn keeps the spirit. Other signs point law to Libra or Capricorn, and Pisces *Crime* is kept to wrongdoing as a moral and social category. The contested items (the language laws, the referendums, the 1990 Kanehsatà:ke resistance, residential schools, the James Bay agreements) are flagged as rival accounts where they appear.

## Repeat check across the nation
- **Exact repeats:** 0 lines, table rows, compare bullets, Flags lines or first queries repeated between any two of the 130 sheets. The template's fixed lines are excluded.
- **Near matches** (0.85 similarity, sections 3 to 5): only 1. It is the two Libra Held lines after the run agent's own category-only edits, which share the category wording by design.
- **Held lines:** none is a bare "none."; each names the kinds of pointer weighed for its concept. Many follow one frame ("the X, Y and Z pointers weighed for [concept] ... nothing set aside"). They are not copied, but they read as formulaic.

## Thin, repetitive or generic sheets
- **No sheet reads as thin.** The shortest is Aries *Competition* (1,095 words, 15 pointers).
- **Weakest on the pre-modern pointer:** Virgo *Work* (its earliest pointer is from 1897, although New France labor records such as notarial engagement contracts were an obvious route) and Sagittarius *Meaning* (earliest pointer from 1937). Five more sheets reach back only to the 19th century (folk tales and legends of 1834-1880): Aries *Competition*, Taurus *Stubbornness*, Cancer *Nurture*, Pisces *Escapism* and Pisces *Fear*. The rest have a New France, Jesuit, seigneurial, wampum or other pre-1800 pointer.
- **Recurring sources** (counted in section 2): Statistics Canada appears in 50 sheets, BAnQ in 42 and Radio-Canada in 31. All the others are in 10 or fewer, for example Kativik in 10, the *Jesuit Relations* in 9, the NFB in 9, Avataq in 8, the ISQ in 7 and Barbeau in 5. The three national sources are expected anchors, not padding, but a later pass could vary them.
- **Possible over-inclusion:** Haitian Montreal appears in 127 of 130 sheets and Nunavik and the Inuit in 122. This reads partly as a routine slot in the compare section rather than a concept-driven choice. Check that the later research does not treat these as default comparisons.

## Depth: do the sheets exploit the nation's depth?
Mostly yes. Sheets naming each region or people (of 130, by name search): Montreal 130; Quebec City and the Capitale-Nationale 92; the Gaspé 77; the Saguenay–Lac-Saint-Jean 67; the Côte-Nord 65; Abitibi 53; the Beauce and Chaudière-Appalaches 53; the Bas-Saint-Laurent 48; the Mauricie 40; the West Island 40; Eeyou Istchee (by that name) 32; the Eastern Townships 31; the Magdalen Islands 31; the Laurentides 20; **the Outaouais 17** (the thinnest region). Peoples: Nunavik Inuit 122; Innu 99; Kanien'kehá:ka 88; Eeyou 82; Atikamekw 76; Naskapi 53; Wendat 45; W8banaki 37; Anishinaabeg 36; Mi'gmaq 29; Wolastoqiyik 27; Acadians 17. Communities: Haitian 127; Anglophone Quebecers 108; Jewish communities 104; Maghrebi 51; Italian 47; Vietnamese 45; Latin American 41; Portuguese 30; Lebanese 28; Greek 22. Search terms use Quebec French and *joual*, the Acadian French of the Magdalen Islands, Innu-aimun, East Cree, Kanien'kéha, Atikamekw, Inuktitut of Nunavik (in syllabics where the agent was sure), Wendat, Mi'gmaq, W8banaki, Haitian Creole and Yiddish, with each uncertain form marked *check*. The Outaouais, the Laurentides and the Acadians of the Magdalen Islands are the least used of the named regions and peoples.

## Judgment calls for the author
1. **Lands:** the tracker settles no lands and there is no scope file. The sheets write for Quebec as the province stands. Labrador, the Maritimes and Franco-Ontario appear only as comparison, and the note to that effect is in each Domain sheet only. Please settle whether Quebec's post-war lands reach beyond the province (Labrador, the Maritimes, Franco-Ontario).
2. **Ancestor altars (Pisces *Spirituality*):** keep this pointer, or hold it with Buddhism as a category?
3. **Park Extension:** keep the neighborhood name? It appears as a renters' district and as the historic Greek neighborhood, with no South Asian community named.
4. **The three category-only cuts** (Libra *Partnership* and *Reciprocity*, Capricorn *Ambition*) follow Monday's rulings on scholars of South Asian heritage abroad and their datasets. They stand until the author rules.
5. **Pre-modern gap** in Virgo *Work* and Sagittarius *Meaning*: patch these in the research stage, or relaunch them as single-concept jobs?
