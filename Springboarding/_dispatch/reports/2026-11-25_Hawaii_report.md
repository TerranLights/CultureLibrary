# Hawaii springboard scouting: run report (2026-11-25)

**Result:** 130/130 sheets done (`springboard_status.py Hawaii`), whole-nation `springboard_qa.py Hawaii`: 130 sheets scanned, 0 problems. Run agent with one sub-agent per sign (12), plus 1 single-concept relaunch. Lands: no settled lands and no `00 - Scope.md`; pre-war lands USA; written for the Hawaiian Islands (the main islands with Papahānaumokuākea) as the core; the lands note appears once per sign, in each Domain sheet's Flags only. No unit list was added. `Hermes_research` was not opened.

**Wall clock:** first launch 05:07, last sub-agent back 10:05, checks and report done about 10:15 MST (about 5 h 10 min).
**Sub-agent tokens:** 3,379,059 in all (12 sign agents 3,293,548; the relaunch 85,511), 903 tool uses.

## Per sign

| # | Sign | Sheets | Agents | Relaunches | QA | Run-agent edits | Avg words | Longest | Shortest | Pointers | Tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 0 | 1,215 | 1,260 Beginning | 1,178 Competition | 12-14 | 209,206 | 05:07-05:27 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 0 | 1,218 | 1,272 Domain | 1,159 Stubbornness | 13-15 | 218,431 | 05:28-05:43 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 0 | 1,226 | 1,266 Domain | 1,174 Mediation | 13-15 | 233,107 | 05:44-06:01 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 0 | 1,208 | 1,249 Home | 1,165 Care | 13-14 | 267,368 | 06:02-06:22 |
| 5 | Leo | 13 | 1 | 0 | 0 | 0 | 1,152 | 1,207 Creativity | 1,064 Play | 14-15 | 257,249 | 06:23-06:41 |
| 6 | Virgo | 10 | 1 | 1 (Improvement) | 0 | 1 (relaunched sheet's Held line) | 1,197 | 1,268 Domain | 1,119 Usefulness | 13-14 | 281,771 + 85,511 | 06:42-07:05; 09:10-09:13 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1 | 1,260 | 1,277 Peace at any price | 1,249 Reciprocity | 13-14 | 286,282 | 07:06-07:28 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 2 (nation pass) | 1,171 | 1,271 Domain | 1,107 Crisis | 12-14 | 307,857 | 07:28-07:59 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 4 | 1,113 | 1,276 Domain | 1,015 Honesty | 12-14 | 296,358 | 08:00-08:28 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1 | 1,238 | 1,294 Domain | 1,182 Merit | 13-14 | 322,653 | 08:29-09:09 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1 (nation pass) | 1,203 | 1,298 Domain | 1,099 Detachment | 12-14 | 288,456 | 09:10-09:36 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 2 | 1,259 | 1,299 Domain | 1,184 Fear | 12-14 | 324,810 | 09:37-10:05 |

Whole nation: average 1,204 words by `wc -w` (1,015 to 1,299; none over 1,300). Pointers per sheet: 12 on 11 sheets, 13 on 45, 14 on 70, 15 on 4.

## Rule breaks and fixes
- **South Asian rule.**
  - Virgo Improvement used, as a table pointer and as a first query, a US intergenerational-mobility dataset known by a South Asian-heritage economist's name. It was relaunched as a single-concept job. The dataset is now replaced by census-tract tables and a Kamehameha Schools report (both marked *check*), and the Held line gives the category only.
  - Capricorn Ambition's Held line named the same dataset. It is now cut to the category.
  - Sagittarius Truth's and Meaning's Held lines described the held item ("a historiography pointer"; "the purpose-seeking rows"). Both are now cut to the category.
  - The Cancer Domain sub-agent removed a co-author with a likely South Asian surname before marking the sheet done.
  - A name scan over all 130 sheets (an extended surname and term list) is otherwise clean.
- **Findings.** Three pointers stated a belief or claim and were reworded to say what to check:
  - Libra Partnership: the Lāʻie temple row stated members' belief about marriage.
  - Sagittarius Belief: the Pali pork-rule row said the rule was "still repeated".
  - Pisces Crime: one bullet said how Niʻihau's community handles wrongs.
- **Trait statements in "Who to compare".** Four bullets stated something about a group. Each now says what to check:
  - Pisces Crime: shame talk presumed among Japanese and Okinawan families.
  - Scorpio Rebirth: "their speech was never broken".
  - Scorpio Secrecy: "their privacy is long-standing".
  - Aquarius Idealism: "paradise seekers ... who never sought the islands".
- **Near repeats.** Two Held lines that I had cut to the category came out close to other Held lines (Virgo Improvement and Sagittarius Education; Sagittarius Truth and Capricorn Ambition). Both were reworded.
- **Indo- pattern.** The Scorpio sub-agent renamed the US military's Pacific command to avoid the pattern. "Indian" appears in no sheet. Neither universals nor Hermes appears in any sheet.
- **Final repeat check across the nation:** 0 exact repeats (lines over 40 characters, table rows, compare bullets, Flags lines, first queries) and 0 near matches at 0.85 (sections 3 to 5).
- **Kept false positives from my own name scan:**
  - "Brown": Ryan P. Brown's honor-states study on Leo Honor, and Brown University's segregation project on Pisces Boundary.
  - "Pali": the Nuʻuanu Pali.
  - "Roy": Roy Sakuma's ʻukulele festival.
  - "temple": heiau rites, as in Malo, Kamakau, Valeri and Puʻukoholā, and the Latter-day Saint temple at Lāʻie.
- **Log errata.** My Libra and Scorpio Run log lines misnamed one Buddhism-hold sheet each:
  - Libra: the actual sheets are Domain, Justice, Reciprocity and Peace at any price.
  - Scorpio: the actual sheets are Domain, Death, Rebirth, Purging and Secrecy.

## Holds
- **South Asian category:** 8 sheets (Sagittarius Domain, Meaning, Truth, Education and Fundamentalism; Libra Projection; Capricorn Ambition; Virgo Improvement), category only. Five sit in Sagittarius. The two from the dataset are real. I cannot verify that the Sagittarius ones hide a real pointer rather than a routine line; Education's and Fundamentalism's look the most formulaic.
- **Buddhism as a category:** 46 sheets, with no community, temple or text named. This is far more than on the mainland nations. Japanese Buddhist temples and missions are a major island institution, so the open Buddhism question weighs heavily on Hawaii. Taurus held it on 7 of 11 sheets, so from Gemini on the prompt asked for a hold only where a concept-specific pointer was really set aside. After that the count ran at 2 to 6 per sign.

## Thin, repetitive or generic sheets
- **Shortest and thinnest:** Sagittarius Honesty (1,015 words, 12 pointers), Conviction (1,036, 12) and Fundamentalism (1,053, 12), and Leo Play (1,064). Twelve-pointer sheets also include Scorpio Trust, Revenge and Crisis; Aquarius Reform, Nonconformity and Detachment; Pisces Crime.
- **Formulaic Held lines:** the "nothing set aside; the X, Y and Z pointers weighed ... raised no item under the standing rules" pattern recurs on many sheets. Each is worded differently, but the form is generic.
- **Niʻihau bullets:** many sheets carry a "go only through the community" bullet for Niʻihau. These are right as access notes, but repetitive in kind. Kalaupapa, Kahoʻolawe (6 sheets) and the Windward side (13) are thinner.
- **Reused source:** Aquarius Domain reuses the church relief-drive source from Scorpio Crisis (2009 Samoa tsunami, 2022 Hunga Tonga), with different wording and a different reason. Kept.

## Depth
The sheets do use the nation's depth. Counts across the 130 sheets:

| What | Sheets |
|---|---|
| Kalihi | 55 |
| Waiʻanae | 64 |
| Hilo | 74 |
| Molokaʻi | 72 |
| Kauaʻi | 68 |
| Hāna | 47 |
| Kaʻū | 39 |
| Lānaʻi | 42 |
| Lahaina | 29 |
| Papahānaumokuākea | 16 |
| Puerto Rican | 78 |
| Visayan | 108 |
| Marshallese | 114 |
| Chuukese | 111 |
| paniolo | 31 |
| military families | 59 |
| Latter-day Saint | 48 |
| Hawaiian-language newspapers (nūpepa) | 58 |
| Kamakau | 37 |
| Malo | 18 |
| ʻĪʻī | 10 |
| Bishop Museum | 20 |
| Hawaiʻi State Archives | 35 |

Some high counts include the "Languages needed" lines. Pre-modern pointers appear in every sign, with the fewest in Cancer. Some core works are lightly used, which is acceptable at this stage: the *Kumulipo* (2 sheets), the Māhele (4) and the Kūʻē petitions (2).

## Judgment calls for the author
1. **Buddhism on 46 sheets.** Japanese Buddhist temples and missions are among Hawaii's main community institutions, so a ruling on the Buddhism question will change many of these sheets.
2. **The mobility dataset (Virgo Improvement, Capricorn Ambition).** I treated it as "a project known by a South Asian-heritage scholar's name" and held it. Please confirm.
3. **Shinto shrines are named as pointers on 9 sheets** (for example a Daijingu and the Izumo Taishakyo Mission). No standing rule covers Shinto. Confirm that they stay.
4. **Contested ground and restricted knowledge** (the overthrow, sovereignty, Mauna Kea, Red Hill, Kalaupapa, the Lahaina fire, heiau sacrifice on Pisces Self-sacrifice, *ʻanāʻanā*, *iwi kūpuna*, Niʻihau) is flagged sheet by sheet as accounts or as restricted. Please spot-read Scorpio Revenge, Pisces Self-sacrifice and Pisces Crime.
5. **Lands are still unsettled.** Each Domain sheet carries the note once, and nothing beyond the islands is treated as the target.
