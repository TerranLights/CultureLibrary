# CSA springboard run: report (2026-11-23)

**Run agent, deeper brief (accuracy and depth first).** Nation: CSA (the culture-nation of the American South), all twelve signs, one sub-agent per sign. Folder: `Targets/North America/CSA/Springboards/`.

**Result:** 130/130 sheets `STATUS: done 2026-11-23, not verified`. Whole-nation QA (`springboard_qa.py CSA`): **130 sheets scanned, 0 problems.** 12 sign agents, 3 single-concept relaunches, 1 smallest edit by the run agent.

**Wall clock:** start 05:04, first sign launched 05:05, last sheet 08:57, report 09:12 (no usage-limit stop).
**Tokens:** sign sub-agents 3,154,648; relaunches 187,214; **total sub-agent tokens 3,341,862** (the run agent's own tokens are not included).

## Per sign
| # | Sign | Sheets | Relaunches | QA | Avg words (wc -w) | Longest | Shortest | Pointers (min-max, avg) | Sub-agent tokens | Minutes |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 0 | 0 | 1,192 (1,190 after the edit) | 1,278 Domain | 1,095 Recklessness | 15-16, 15.1 | 199,421 | 17.8 |
| 2 | Taurus | 11 | 1 (Stability, own scan) | 0 | 1,268 | 1,291 Possession / Stability | 1,249 Wealth | 14-15, 14.9 | 214,862 + 63,971 | 14.4 |
| 3 | Gemini | 10 | 1 (Connection, own scan) | 0 | 1,247 | 1,286 Learning / Connection | 1,194 Curiosity | 14-15, 14.1 | 217,023 + 61,476 | 13.9 |
| 4 | Cancer | 10 | 0 | 0 | 1,244 | 1,272 Home | 1,187 Nurture | 14-15, 14.1 | 265,635 | 17.7 |
| 5 | Leo | 13 | 0 | 0 | 1,237 | 1,288 Domain | 1,190 Humiliation | 14-15, 14.3 | 276,857 | 19.5 |
| 6 | Virgo | 10 | 0 | 0 | 1,248 | 1,291 Domain | 1,193 Discernment | 13-15, 14.1 | 297,547 | 20.4 |
| 7 | Libra | 11 | 0 | 0 | 1,252 | 1,298 Domain | 1,170 Impartiality | 15-16, 15.1 | 257,343 | 16.4 |
| 8 | Scorpio | 11 | 0 | 0 | 1,224 | 1,277 Domain | 1,157 Purging | 14-16, 14.7 | 276,886 | 22.3 |
| 9 | Sagittarius | 11 | 0 | 0 | 1,203 | 1,289 Domain | 1,136 Conviction | 14-16, 14.5 | 271,225 | 17.0 |
| 10 | Capricorn | 10 | 1 (Ambition, Held line) | 0 | 1,206 | 1,289 Domain | 1,122 Merit | 13-16, 14.7 | 284,514 + 61,767 | 23.0 |
| 11 | Aquarius | 10 | 0 | 0 | 1,200 | 1,280 Group | 1,073 Detachment | 12-15, 13.6 | 317,624 | 23.8 |
| 12 | Pisces | 12 | 0 | 0 | 1,189 | 1,297 Domain | 1,137 Dissolution | 13-14, 13.6 | 275,711 | 20.0 |
| | **Nation** | **130** | **3** | **0** | **1,226** | 1,298 (Libra Domain) | 1,073 (Aquarius Detachment) | **12-16, 14.4** | **3,341,862** | about 3 h 52 min |

None is over 1,300 words; 89 of 130 are over 1,200.

## Rule breaks and fixes
- **A South Asian-heritage scholar was named in two sheets** (caught by the run agent's own name scan after Capricorn; the QA scan matches words, not names). The economist who leads Opportunity Insights was named in Taurus *Stability* (Opportunity Atlas) and Gemini *Connection* (Social Capital Atlas). Both were relaunched as single-concept jobs: the rows were replaced with the Panel Study of Income Dynamics (Stability) and Add Health (Connection), and the datasets are now held as a category only. Capricorn's own sub-agent had already held the same atlas, but by name in the Held line. *Ambition* was relaunched, and its Held line now names the category only. From Aquarius on, the prompts said outright that US-based scholars of South Asian heritage fall under the rule.
- **One near-repeat Flags line** (the run agent's fuzzy check): the Aries *Recklessness* "Languages needed" line was a subset of *Anger*'s. The run agent fixed it with the smallest edit, adding the reason for each language specific to the concept.
- **After the fixes:** no line, table row, "Who to compare" bullet or Flags line is repeated exactly anywhere in the nation, and no first-column pointer cell is repeated exactly. The fuzzy check (similarity over 0.85) leaves only the "Held for review" lines, which share the brief's required category phrase ("South Asian-heritage communities in the nation's lands") and differ in their concept-specific clause. It also leaves two Domain "Lands" notes, which are worded differently, one per sign.
- **No** zodiac words, universals, Hermes, URLs, or "Indian" outside a published title. Law appears outside Libra and Capricorn only as plain history or as a pointer to those signs (checked by hand for signs 1 to 5, Scorpio, Sagittarius and Pisces *Crime*). The lands note appears once per Domain sheet and in no concept sheet.

## Thin, repetitive or generic sheets
- **Thinnest:** Aquarius *Detachment* (1,073 words, 12 pointers). Its pointers are real but loosely tied: a mix of literature, film, a NASA memoir and generic census and CPS tables. Aquarius and Pisces have the lowest pointer averages (13.6). The 13-pointer sheets are Aquarius *Reform*, *Friendship* and *Nonconformity*; Pisces *Self-sacrifice*, *Boundary*, *Spirituality*, *Intuition* and *Crime*; Capricorn *Merit*; and Virgo *Domain* and *Discernment*.
- **Repetition:** some standard works recur across signs, each time with a reason specific to the concept. Examples are Wyatt-Brown's *Southern Honor*, Fischer's *Albion's Seed*, Du Bois's *Souls of Black Folk*, Porter on Black Seminoles, the FIU Cuba Poll and Hurston. No row is copied.
- **Generic:** none stood out in the samples read (Aries *Identity*, Libra *Justice*, Sagittarius *Fundamentalism*, Pisces *Crime*). Each has specific named sources with reasons.

## Depth (counts of the 130 sheets naming each)
These are keyword counts, so treat them as approximate. Tejano 130, Vietnamese 130, Cuban 125, Florida 124, Cajun/Acadiana 110, Seminole/Miccosukee 97, Choctaw 92, Muscogee/Creek 86, Creole 84, Gulf Coast 83, Delta 66, Gullah Geechee 59, Black Belt 59, Lumbee 53, Lowcountry/Sea Islands 51, Piedmont 45, German Texans 42, Jewish Southerners 35, Ozarks 33, Greek 32, Lebanese/Syrian 28, Mississippian sites 27, Houma 15, Chickasaw 14, Czech/Wendish 14, spirituals 14, Cherokee 13, WPA narratives 12, Isleños 5, Delta Chinese 4, Melungeons 4. 119 of 130 sheets carry a pointer marked "pre-modern" (colonial French and Spanish records, Mississippian sites, early ethnography, slave narratives, spirituals). **The sheets exploit the nation's depth well:** they reach well beyond the Black and white binary to Tejano, Cuban, Vietnamese, Cajun and Creole, Native, Lumbee and smaller immigrant peoples, from the first sign on. The weaker spots are the Chickasaw, the Houma, the Isleños and the Delta Chinese, which appear rarely. Melungeons appear rarely too, but they are largely Appalachian, a separate nation.

## Judgment calls for the author
1. **South Asian-heritage scholars working in the US** (here, the Opportunity Insights datasets) were treated as falling under the strict South Asian rule and held as a category. Confirm, or allow such datasets back.
2. **"Yoga" kept in Pisces *Spirituality*.** It appears only as an item in a federal health survey (the NHIS complementary-health supplement), not as a work, scholar, community or language. Keep it or remove it.
3. **"The Carolina Indian Voice"**, the Lumbee weekly's own published title, is kept in quotation marks (Virgo *Criticism*).
4. **Lands:** each Domain sheet sketches the "core South" in its own words (for example "Tidewater to Texas and Florida", "Ozarks included", "the old Confederate states"). These are working descriptions, not unit lists. Whether Virginia's Tidewater, the Ozarks, Oklahoma (the removed Muscogee, Choctaw, Chickasaw, Seminole and Cherokee nations, used here as comparisons) and Kentucky and Tennessee (with the Appalachian parts going to Appalachia) belong to the CSA is for Stage 0.
5. **Native nations removed to Oklahoma** appear in "Who to compare" beside the nations that remain in the South (Mississippi Choctaw, Poarch Creek, the Florida Seminole and Miccosukee). Confirm whether the Oklahoma nations are CSA units or comparison only.
6. **Contested memory** (Confederate symbols, the Lost Cause, Massive Resistance) is flagged throughout as contested and is never presented as the region's single voice.
