STATUS: done 2026-11-21. Run agent's report; the sheets are unverified.

# Germany: springboard run report (deeper brief)

**Result:** all 130 sheets are done. Every first line reads `STATUS: done 2026-11-21, not verified`. The run used 12 sign agents plus 1 relaunch (Capricorn, after a usage-limit cutoff). The whole-nation QA (`springboard_qa.py Germany`) found **0 problems** in 130 sheets, and no sheet needed a hand fix.

**Tokens and wall-clock:**
- **Sub-agent tokens:** **2,372,001** as reported by the harness (11 sign agents plus the Capricorn relaunch). The first Capricorn agent was cut off by the 5-hour usage limit, and the harness reported no usage for it. Its transcript's last turn counts about **168,095** tokens, an estimate on the same basis as the reported figures (the same count gave 177,254 for Aries against the reported 177,737). **Total with that estimate: about 2,540,096.** The run agent's own tokens are not included; the main session adds them.
- **Tool uses:** 486 across the reported agents (the cut-off agent's count is unknown).
- **Wall-clock:** the run agent started at **08:02:18 MST**. The Aries agent launched at 08:03 and the Pisces agent finished at 12:19. The report was written by **about 12:25 MST**, so the run took about 4 h 23 min in all.
- **Interruption:** from **about 10:35 to 11:43** the run was paused because the 5-hour usage limit was hit during Capricorn. Active time was about 3 h 15 min.
- **Time per sign:** 11.8 to 16.7 min. Signs ran one after another.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,185 | 1,254 (Self-assertion) | 15.9 (15-16) | 177,737 | 08:03-08:18 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,210 | 1,276 (Ownership) | 16.0 (16) | 205,151 | 08:18-08:33 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,192 | 1,259 (Domain) | 14.7 (13-15) | 189,700 | 08:34-08:46 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,185 | 1,272 (Domain) | 15.9 (15-16) | 202,625 | 08:47-09:01 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,191 | 1,275 (Domain) | 15.2 (14-16) | 215,694 | 09:01-09:18 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,244 | 1,269 (Improvement) | 15.4 (14-16) | 207,529 | 09:18-09:34 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,210 | 1,247 (Peace at any price) | 14.9 (14-15) | 206,303 | 09:34-09:48 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,189 | 1,258 (Domain) | 15.2 (14-16) | 207,347 | 09:49-10:03 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,178 | 1,246 (Domain) | 15.6 (15-16) | 199,346 | 10:03-10:17 |
| 10 | Capricorn | 10/10 | 2 | 1 (usage-limit cutoff) | 0 | 1,244 | 1,279 (Hierarchy) | 15.6 (15-16) | about 168,095 (estimate) + 153,691 | 10:18-10:35, 11:42-11:50 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,160 | 1,232 (Domain) | 15.5 (14-16) | 192,792 | 11:51-12:03 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,201 | 1,270 (Dissolution) | 16.0 (16) | 214,086 | 12:03-12:19 |
| | **Total** | **130** | **13** | **1** | **0** | **1,199** | **1,279** | **15.5 (13-16)** | **2,372,001 reported; about 2,540,096 with the estimate** | **08:03-12:19** |

- **Word counts:** by `wc -w`, markup included. The shortest sheet is Sagittarius/Honesty at 1,073 words, and the longest is Capricorn/Hierarchy at 1,279. No sheet is over the 1,300 flag. Seventy sheets are between 1,200 and 1,279 words, which is within the brief's "a little over is fine".
- **Pointers:** these are the rows of section 2. Every sheet has 13 to 16, and only the Gemini Domain sheet has 13.

## Rule breaks and fixes
- **QA:** nothing was flagged in any sign or in the whole-nation scan.
  - No zodiac, divination-label or horoscope words.
  - No "Indian".
  - No "Indo-" words. The sub-agents were told the scan flags them.
  - No URLs.
  - No "sikh"-pattern false positives.
  - Nothing from Hermes_research.
- **South Asian rule:** 13 sheets carry the brief's category-only line "Held for review: South Asian-heritage communities in the nation's lands". These are the Scorpio Domain, Death and Crisis sheets and all 11 Sagittarius sheets. The other 117 sheets read "none".
- **Lands note:** it appears once in each sign's Domain sheet (12 of 12) and in no other sheet. It says that Germany's lands are still to be settled by the author. No sheet tells the reader to read a scope file, and no unit list was added.
- **Austro-Bavaria:** Bavaria is handled as a separate target, named at most as a neighboring comparison. In **Taurus, every sheet carries a standing bullet** of the form "Neighbor comparison only: Bavaria ... Diaspora comparison only: ...". Each bullet gives its own reason, and nothing in it is a rule break, but the pattern is formulaic. From Gemini on, the sub-agent prompt said to name Bavaria or a diaspora only where it sharpens the concept. After that, Bavaria appears on 1 or 2 sheets per sign (mostly the Domain).
- **Law:** the law material is in Libra (the letter of the law) and Capricorn (the spirit). Capricorn's relaunch prompt restated the spirit-of-law rule.
- **Checkpoint slips (no action):**
  - In Taurus, the sub-agent edited sheets 01 to 09 after marking them done. It gave each Bavaria bullet its own reason and dropped one surplus pointer each from Security and Stability. The final files are complete and clean.
  - In Capricorn, Hierarchy was half-written (`in progress`) at the cutoff. The relaunch read it and completed it. The six done sheets were not touched.

## Repetition
- **Lines:** no line of more than 40 characters repeats anywhere in the 130 sheets, apart from:
  - the template's fixed lines;
  - the brief's category-only Held-for-review line.

  That includes the "Who to compare" bullets.
- **Most-reused sources** (counted as sheets that name them, out of 130):
  - Luther (the Bible translation, the catechisms, or the word itself): 35.
  - The Brothers Grimm (the tales or the *Deutsches Wörterbuch*): 33.
  - DWDS: 29.
  - Weber: 17.
  - SOEP: 15.
  - Allensbach: 15.
  - ALLBUS: 10.
  - Elias: 8.

  No single named pointer cell appears on more than 6 sheets. The most frequent cells are DOMiD (Cologne), the *Handwörterbuch des deutschen Aberglaubens*, *Struwwelpeter* and the Cologne carnival committee, at 6 each. The Luther and Grimm counts are mostly search-term or etymology use rather than repeated table rows. They are the nearest thing to default pointers.

## Thin, repetitive or generic sheets
- **No sheet is thin.** The four shortest are:
  - Sagittarius/Honesty: 1,073 words.
  - Aquarius/Detachment: 1,087.
  - Leo/Humiliation: 1,115.
  - Cancer/Nurture: 1,118.

  All four still have 15 or 16 pointers.
- **Most query-heavy** (pointers given partly as a source type plus a query):
  - Gemini/Siblings and Gemini/Mediation: 7 or 8 rows carry a query.
  - Gemini/Gossip and Gemini/Connection: 5 each.
  - Capricorn/Hierarchy: 4.

  In Siblings the query sits next to a named anchor (for example FReDA, Destatis, Hartmut Kasten), so these rows are hedged named sources, not empty ones. Gemini's social concepts are where the agents were least sure of titles.
- **Generic tendency:** Sagittarius/Honesty leans on national-level, West-German-centered data (the lost-wallet experiment, SCHUFA, VroniPlag, Stiftung Warentest, the diesel scandal), with fewer regional and minority pointers than most sheets. It is worth a look in the review. The Taurus standing Bavaria and diaspora bullets (above) are the main formulaic feature.

## Does it exploit the nation's depth?
- **Minority and regional languages:**
  - Sorbian (Upper and Lower; Serbski institut on 11 sheets): 101 sheets.
  - Danish (the South Schleswig minority): 110.
  - Low German / Plattdeutsch: 85.
  - North Frisian (Nordfriisk Instituut on 7 sheets): 44.
  - Saterland Frisian: 12.
  - Romani and Sinti: 50.
- **Migrant-heritage communities:**
  - Turkish: 130 sheets.
  - Arabic: 123.
  - Russian-German / Aussiedler: 72.
  - Polish: 78.
  - Kurdish: 63.
  - Yiddish: only 6 sheets. Jewish Germans are named on 42 sheets, more often by name than by language.
- **Pre-modern pointers:** about 120 of 130 sheets contain one. They include:
  - Old and Middle High German terms: Middle High German on 37 sheets and Old High German on 10.
  - Tacitus, the *Nibelungenlied*, Hildegard, Eckhart and the Sachsenspiegel.
  - Reformation and Hanseatic material.
  - Grimm.
  - Older scripts (Fraktur, Kurrent, Sütterlin) are noted on 22 sheets.
- **East and West:** GDR, *Wende* and post-1990 East German sources run throughout (for example Steffen Mau's *Lütten Klein* and the GDR-era archives), as do the Ruhr, Saar, Rhineland, Hanseatic North, Saxony and Lusatia. Counted by sheet: GDR 99, Rhineland 71, Saxony 56, Lusatia 55, Ruhr 46, Hanse 33.
- **Verdict:** yes. The sheets go well beyond the best-known two or three and use native-language search terms throughout. The weak spots are:
  - Yiddish is thin.
  - The Taurus standing bullets.
  - A few sheets (Honesty, some Gemini sheets) lean national.

## Notes for the author
- **Lands:** Germany's lands are not settled (no `00 - Scope.md`). The sheets are written for the core German lands, with Bavaria outside them as a separate target. If the settled lands differ (for example, if they draw the Franconian or Swabian parts of today's Bavaria into Germany), the regional "Who to compare" bullets will need a look.
- **Usage limit:** the 5-hour limit hit during Capricorn at about 10:35, and the run resumed at about 11:43. The cut-off agent's tokens are an estimate (see above).
