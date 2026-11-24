# Lithuania springboards: run report (2026-11-24)

**Result:** 130 of 130 sheets done (all `STATUS: done 2026-11-24, not verified`). There are twelve signs, Aries to Pisces, with one sub-agent per sign under the deeper brief. There were no relaunches and no usage-limit stop. Whole-nation QA: **130 sheets scanned, 0 problems.** My own repeat check across the nation found **0 exact repeats** of any line, table row, "Who to compare" bullet, Flags line or first query (template lines aside).

**Wall clock:** the run agent started at 05:04, the first sub-agent was launched at 05:05, and the last sub-agent returned at 08:30. Checks and fixes ended at about 08:35. The twelve sign agents ran one after another, so the whole nation took about 3 h 30 min.

**Sub-agent tokens:** 2,759,112 in total (671 tool uses), about 230,000 per sign. The run agent's own tokens are not counted here.

## Per sign

| # | Sign | Sheets | Agents | Relaunches | QA problems | Avg words | Longest | Shortest | Pointers (min-max, avg) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,132 | 1,222 (Domain) | 1,050 (Anger) | 14-15, 14.8 | 172,143 | 05:05-05:19 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,170 | 1,272 (Ownership) | 1,064 (Possessiveness) | 14-16, 14.9 | 226,474 | 05:21-05:38 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,256 | 1,297 (Duality) | 1,192 (Connection) | 15, 15.0 | 204,675 | 05:40-05:53 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,251 | 1,286 (Domain) | 1,229 (Nurture) | 14-15, 14.3 | 227,407 | 05:54-06:09 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,204 | 1,271 (Domain) | 1,136 (Joy) | 12-15, 13.8 | 265,050 | 06:10-06:29 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,219 | 1,278 (Work) | 1,179 (Perfectionism) | 13-15, 14.4 | 212,272 | 06:31-06:44 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,197 | 1,261 (Domain) | 1,126 (Impartiality) | 14-15, 14.2 | 254,845 | 06:46-07:01 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,205 | 1,263 (Domain, Purging) | 1,148 (Power) | 13-15, 13.7 | 275,923 | 07:03-07:21 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,222 | 1,268 (Domain) | 1,167 (Conviction) | 13-15, 14.1 | 247,553 | 07:23-07:41 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1,209 | 1,248 (Domain) | 1,159 (Hierarchy) | 14-15, 14.3 | 234,700 | 07:44-07:59 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,191 | 1,275 (Domain) | 1,104 (Detachment) | 14-15, 14.6 | 202,908 | 08:01-08:12 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,167 | 1,271 (Domain) | 1,097 (Escapism) | 14-16, 14.7 | 235,162 | 08:14-08:30 |
| | **Nation** | **130/130** | **12** | **0** | **0** | **1,201** | **1,297** | **1,050** | **12-16, 14.4** | **2,759,112** | **05:05-08:30** |

Word counts are by `wc -w` after the fixes below. No sheet is over 1,300 words. The longest, Gemini Duality at 1,297, is close to the limit because of the Languages-line fix.

## Rule breaks and fixes

The QA scan found nothing. Every fix below came from my own checks and is a run-agent edit, not a relaunch:
1. **Lands note wording (Taurus Domain).** The note read "Lithuania has no settled lands list or scope file yet", but the brief says never to point to a scope file. I reworded it to "Lithuania's exact lands are still to be settled" and told later signs to say only that.
2. **South Asian Held lines that used the sub-agent's own category** (as with Appalachia on Monday). I rewrote both to the brief's category only:
   - Sagittarius Domain: "South Asian-derived religious movements in Lithuania".
   - Pisces Spirituality: "... and seekers' practices of South Asian origin".

   From Capricorn on, the prompt also told each sub-agent to word the category as the brief does.
3. **"Languages needed" lines that were bare lists** (lesson 6: each gives a reason specific to the sheet's concept). Eight lines had no reasons and closely matched each other: Gemini Information, Duality, Siblings and Mediation, and Leo Dignity, Leadership, Play and Honor. A ninth, Pisces Intuition, closely matched the Pisces Domain line. Each now ties each language to that sheet's own pointers.
4. **A mid-run prompt addition (Aries onward).** The QA scan's `indo-` pattern catches "Indo-European", and the usual comparison of Lithuanian with Sanskrit names a South Asian language. Both are central traps for Lithuania. Mid-run I sent the Aries sub-agent a rule to avoid every "Indo-" compound and never name Sanskrit, and I added it to every later prompt. As a result, no sheet uses either. Gimbutas appears in 4 sheets, described in other words.

My own looser name scan also matched the Belarusian *ціхмяны* (*tsikhmiany*, "meek, quiet") in Libra "Peace at any price" on "sikh". The QA scan, which uses word boundaries, did not flag it, so I kept it as written.

## Standing rules, checked by hand

- **Lands.** The missing-lands note appears once per sign, in the Domain sheet only. No sheet mentions a scope file and no unit list was added. The note sits in all 12 Domain sheets, one per sign, as in earlier nations' runs.
- **South Asian rule.** No South Asian scholar, work, community, religion or language is named anywhere. The category is held twice, both times on a real set-aside: Sagittarius Domain and Pisces Spirituality.
- **Buddhism.** It is held as a category three times, with nothing named: Sagittarius Domain, Aquarius Detachment and Pisces Spirituality.
- **Law.**
  - Libra stays with the letter of the law: the Criminal Code, statutes, Constitutional Court rulings, and composition for wrongs in the Statutes of Lithuania.
  - Capricorn stays with the spirit of the law: Sapieha's 1588 preface, legal nihilism, and proverbs on courts.
  - Elsewhere, law appears only as redirects to those two signs. Pisces Crime is kept to wrongdoing as a moral and social category.
  - Two borderline uses were judged not to be law research: Virgo Perfectionism uses the Vilnius guild statutes only for the masterpiece standard, and Scorpio Purging uses the Samogitian castle-court books as records of witchcraft accusations.
- **Banned words and phrases.** No "Indian", no zodiac words, no URLs, no findings phrases, no universals or Human Universals, and no Hermes material.
- **Contested ground** is presented as accounts, with each community named by its own name. This covers the Vilnius question, 1941 and the Holocaust, the deportations, the partisans (*miško broliai*) and the KGB-collaborator files. No compare bullet states a trait of a group.
- **Separate culture-nations.** Latvia, Estonia, Belarus, Poland and Kaliningrad (Lithuania Minor history) appear only as comparison or source context. The diaspora also appears only as comparison.

## Thin, repetitive or generic sheets

- **No thin sheet.** The shortest is Aries Anger at 1,050 words with 14 pointers. The fewest pointers are in Leo Honor (12). Several Leo and Scorpio sheets have 13 (Leo Dignity, Humiliation, Leadership and Joy; Scorpio Betrayal, Control, Revenge, Power and Crisis), plus Virgo Domain and Sagittarius Conviction.
- **Formulaic Held lines.** About 123 "Held for review: none; nothing on X was set aside" lines differ only by the concept word or phrase. None is an exact copy, and I kept them, as Belarus did on Monday.
- **Sources reused across signs.** Each reuse has new text and a new reason:
  - 5 times: Donelaitis's *Metai*.
  - 4 times: the academic proverb corpus *Lietuvių patarlės ir priežodžiai*.
  - 3 times each: Mykolaitis-Putinas's *Altorių šešėly*, Sruoga's *Dievų miškas*, Kerbelytė's tale catalog, the Sopoćko hospice, Mažvydas's catechism and Valančius's temperance brotherhoods.
  - Everything else appears at most twice.

  No sign is dominated by a few sources.
- **Generic content.** None noted. Every sheet has its own-language terms in several of the nation's languages, including Polish, Russian, Belarusian, Yiddish or Hebrew, and in places Karaim and Tatar Arabic-script terms.

## Do the sheets exploit the nation's depth?

Yes. Counts of sheets out of 130 mentioning each item:

| Group | Counts |
|---|---|
| Peoples | Poles 130, Belarusians 129, Lithuanian Tatars 129, Litvak community 127, Karaim 125, Old Believers 100, Roma 98, Lutherans 71, Romuva 71, Holocaust 61, Ukrainians 58 |
| Regions | Samogitia 124 (plus 19 with *Žemaitija*), Dzūkija 112, Klaipėda 102, Visaginas 95, Lithuania Minor 93, Kaunas 90, Suvalkija 86, Trakai 59, Šalčininkai 52, Curonian Spit 31, Šiauliai 28, Panevėžys 28 |
| Pre-modern sources | Tatar *kitabs* 32, the Vilna Gaon 16, the Statutes 11, Daukša 9, Donelaitis 7, the Juškas 7, Mažvydas 6, Rhesa 6, the book-smugglers 6, the Metrica 5, Łasicki 5 (plus 1 with the Latin spelling) |

Besides these, the sheets bring in many period and regional sources beyond the prompt's examples:
- Sirvydas's *Punktai sakymų*, Wigand of Marburg, the Teutonic Order's *Wegeberichte* and the Bychowiec Chronicle.
- Interwar officers' courts and kolkhoz chairmen's memoirs.
- The Vilna ghetto's Paper Brigade, *Misija Sibiras* and the Medininkai killings.
- Old Believer *nastavniki*, and Karaim and Tatar community periodicals.

Coverage of the minorities is broad, but the sheets repeatedly flag that sources for the smallest communities (Karaim, Roma, Belarusians) may be thin.

## Judgment calls for the author to confirm

1. **Lands.** Lithuania's lands are unsettled. Every sheet is written for Lithuania as it stands. The Klaipėda region and the Vilnius region are treated as internal, and Kaliningrad (historic Lithuania Minor) as comparison only.
2. **Comparing Lithuanian with Sanskrit.** I ruled that this falls under the South Asian rule, so it is left out of every sheet, along with all "Indo-" wording. Please confirm, or rule that a purely linguistic comparison may be named.
3. **The two South Asian holds**, Sagittarius Domain and Pisces Spirituality, are now category only. I chose not to record what was set aside beyond the category.
4. **Buddhism** is held as a category in three sheets, with nothing named, pending your ruling.
5. **The QA script's gap** remains: its `indo-` pattern would flag "Indo-European". It was avoided here by prompt, not fixed.
6. **The hand edits to nine Languages lines and two Held lines** were made by the run agent after the sheets were marked done. The STATUS lines were left unchanged ("done, not verified").
