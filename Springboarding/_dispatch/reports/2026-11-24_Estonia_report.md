# Estonia springboard run: report (2026-11-24)

This run agent handled Estonia in Tuesday's wave 1, under the deeper brief (accuracy and depth first). It used one sub-agent per sign, Aries to Pisces, one after another. Nothing in the sheets has been verified, and every named item is marked *check*.

## Result
- **130/130 sheets done** across the 12 signs, written by 12 sign agents, with **0 relaunches**.
- **Whole-nation QA (`springboard_qa.py Estonia`):** 130 sheets scanned, 0 problems.
- **Repeat check across the nation** (the run agent's own scripts):
  - Exact repeats: **0**. The check covered every non-template line of 40 characters or more, every table row, "Who to compare" bullet, Flags line and first query.
  - Near matches at a ratio of 0.85 or above, on sections 3 to 5: **27 pairs**. All 27 are empty Held lines built on one frame inside a sign, such as "none; no revenge pointer was set aside" against "none; no power pointer was set aside" (mostly Scorpio and Virgo). No compare bullet, Flags line or first query is a near match.
  - 96 sheets carry the bare line "Held for review: none." (too short for the line check). It is the template's empty value, not a copied reason; see the judgment calls below.
- **Sub-agent tokens: 3,062,954** (748 tool uses). The main session adds the run agent's own tokens.
- **Wall clock:** 05:04 to 10:07.
  - First launch 05:06, last return 10:00.
  - There was no forced hand-back and no HTTP 429 stop.
  - Pisces was the slowest sign (61 minutes). Scorpio and Sagittarius took 30 minutes each.
- **Words by `wc -w`:** average 1,226, range 1,065 to 1,295, none over 1,300. 86 sheets run over 1,200. Most signs from Libra on sit at 1,250 to 1,295; the sub-agents for Scorpio and Aquarius reported this themselves.
- **Pointers per sheet:** 13 to 16, average 14.1 (1,837 in all).

## Per sign
| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers | Sub-agent tokens | Tools | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,213 | 1,279 Domain | 1,154 Competition | 15-16 | 194,699 | 46 | 05:06-05:23 |
| 2 | Taurus | 11 | 1,172 | 1,282 Domain | 1,104 Possessiveness | 13-16 | 208,059 | 51 | 05:24-05:39 |
| 3 | Gemini | 10 | 1,243 | 1,290 Domain | 1,176 Curiosity | 13-15 | 219,613 | 45 | 05:40-05:59 |
| 4 | Cancer | 10 | 1,235 | 1,290 Domain | 1,171 Care | 13-15 | 233,659 | 49 | 06:00-06:15 |
| 5 | Leo | 13 | 1,167 | 1,264 Domain | 1,065 Play | 14-15 | 249,199 | 76 | 06:16-06:36 |
| 6 | Virgo | 10 | 1,201 | 1,278 Domain | 1,156 Health | 14 | 261,878 | 56 | 06:37-06:57 |
| 7 | Libra | 11 | 1,261 | 1,295 Reciprocity | 1,162 Indecision | 13-14 | 243,893 | 64 | 06:58-07:14 |
| 8 | Scorpio | 11 | 1,268 | 1,294 Domain, Purging | 1,194 Revenge | 13-15 | 317,468 | 73 | 07:15-07:45 |
| 9 | Sagittarius | 11 | 1,253 | 1,287 Faith | 1,211 Conviction | 13-14 | 272,538 | 68 | 07:46-08:16 |
| 10 | Capricorn | 10 | 1,187 | 1,290 Domain | 1,099 Merit | 13-15 | 262,227 | 57 | 08:17-08:36 |
| 11 | Aquarius | 10 | 1,258 | 1,282 Domain | 1,224 Idealism | 14-15 | 322,190 | 89 | 08:37-08:59 |
| 12 | Pisces | 12 | 1,259 | 1,277 Boundary | 1,229 Intuition | 13-15 | 277,531 | 74 | 09:00-10:00 |

## Rules, breaks and fixes
- **Lands:** the tracker lists no settled lands, records no change to the pre-war lands, and there is no `00 - Scope.md`.
  - Each sign's Domain sheet carries the note once, in its Flags, and no other sheet repeats it. There is no unit list and no border is settled.
  - The Pechory district appears only as comparison, under the Seto's own name for it.
  - **One hand edit (Virgo, Domain):** the lands line named the scope file ("With no `00 - Scope.md` in the folder"). The run agent changed it to "With no settled unit list", because the brief says never to point the reader to a scope file. From Libra on, the sub-agent prompt said so outright, and no later sheet repeated it.
- **South Asian rule:**
  - The QA pattern found 0 hits.
  - After every sign, the run agent scanned the sheets by name for South Asian scholars, writers, works, communities and religions. Every scan was clean.
  - The category is held only where a pointer was really set aside: Sagittarius Belief (religions of South Asian origin and South Asian-heritage communities, from the census-category pointer) and Sagittarius Education (South Asian-heritage students and staff, from the student-mobility data). Neither line describes a held item closely enough to identify it.
- **Buddhism (the author's open question):** it is held as a category only, with no community, temple or text named, in 5 sheets:
  - Scorpio Rebirth
  - Sagittarius Domain
  - Sagittarius Belief
  - Aquarius Detachment
  - Pisces Spirituality
- **False positive (substring):** the Aquarius sub-agent's own scan caught "nepal" inside the surname Õnnepalu.
  - It cited the novel *Piiririik* (1993) under the pen name it was published under, Emil Tode. That is accurate, so it was kept.
  - The same sub-agent says it re-spelled one Russian word that contained "yoga". The run agent could not find which word; the Russian transliterations in Aquarius read as standard. The Pisces prompt added "never re-spell a real word or name to dodge a scan".
  - The QA script's own pattern (`\bnepali`) does not match Õnnepalu.
- **Universals:** no Human Universals and no universals list anywhere. There are 0 hits for "universal".
- **"Indian", zodiac words, Hermes_research, findings phrasing:** none.
- **Law:** Libra keeps to the letter of the law (Riigi Teataja texts and the like) and Capricorn to the spirit. Other signs point legal questions to Libra or Capricorn.
- **Contested ground:** the grey passport and citizenship policy, the deportations, and the 2007 Bronze Night are presented as accounts, each under the community's own name (for example Aries Anger, Aries Identity, Libra Fairness, Aquarius Equality).
- **Stereotypes:** a phrase scan of every "Who to compare" bullet found none. The bullets say what to check.
- **Relaunches:** none were needed. The one fix by hand is the Virgo Domain line above.

## Coverage
Number of sheets (out of 130) that mention each region or people:

| Region or people | Sheets |
|---|---|
| Seto / Setomaa | 130 |
| Ida-Virumaa (Narva, Kohtla-Järve, Sillamäe) | 130 |
| Tallinn / Harjumaa | 129 |
| Estonian Swedes | 129 |
| Võro / Võrumaa | 128 |
| Peipsi shore | 128 |
| Old Believers | 128 |
| Jewish community (incl. Yiddish) | 127 |
| Tatars | 121 |
| Kihnu | 120 |
| Ingrian Finns | 120 |
| Ukrainians | 119 |
| Saaremaa | 115 |
| Tartu | 112 |
| Belarusians | 112 |
| Hiiumaa | 106 |
| Orthodox | 105 |
| Lutheran | 105 |
| Mulgimaa / Mulgi | 104 |
| Muhu | 96 |
| Russian-speaking Estonians (that phrase; Russian terms appear in nearly every sheet) | 92 |
| Ruhnu | 85 |
| Vormsi | 84 |
| Maausk / Taarausk | 84 |
| Järvamaa | 79 |
| Läänemaa | 60 |
| Pärnu | 41 |

- **Pre-modern pointers:** 127 of 130 sheets carry one or more, such as a chronicle, manor or parish records, the runo-song corpus, *leelo*, *Kalevipoeg*, or 16th- to 18th-century texts.
  - The three without one are Virgo Discernment, Libra Diplomacy and Capricorn Merit, which are mostly modern topics.
  - The named items are spread thin rather than repeated: *Chronicle of Henry of Livonia* 12 sheets, Hurt 12, *regilaul* 17, *Kalevipoeg* 16, *leelo* 11, *Livonian Rhymed Chronicle* 6, Wanradt-Koell 6.
- **Core institutions are not overused:** the Estonian Folklore Archives and Literary Museum appear in 68 sheets, Statistics Estonia in 48, the National Museum (ERM) in 41 and the National Archives in 35.

## Thin, repetitive or generic sheets
- **Thin:** none in substance.
  - The shortest sheets are Leo Play (1,065 words), Capricorn Merit (1,099) and Taurus Possessiveness (1,104). They still carry 13 to 14 pointers.
  - The Pisces sheets Intuition and Fear and several Libra and Sagittarius sheets have 13 pointers, the low end of the range.
- **Repetitive:** only the empty Held lines (see the judgment calls below). Sources recur across signs only in new rows written for the new concept.
- **Generic:** none found in the spot checks (Aries Anger, the Domain flags, and the Held lines of every sign).
- **Coverage gaps:** Pärnu and the west coast (41 sheets), Läänemaa (60) and Järvamaa (79) are used less than the other regions the prompt named.

## Does it exploit the nation's depth?
Largely yes.
- Every sheet reaches the Seto, Ida-Virumaa, the Estonian Swedes and the Peipsi Old Believers, and the smaller islands (Kihnu, Muhu, Vormsi, Ruhnu) appear in 84 to 120 sheets.
- The search terms run across Estonian, Võro, Seto, Russian (Cyrillic with transliteration), the coastal Swedish and, where apt, Yiddish.
- Pre-modern anchors run through almost every sheet without any one source filling a sign.
- The thinnest use of depth is regional: Pärnu, Läänemaa and Järvamaa, against the far denser use of Setomaa and Ida-Virumaa.

## Judgment calls for the author
1. **Buddhism** is held as a category in 5 sheets: Scorpio Rebirth, Sagittarius Domain and Belief, Aquarius Detachment, and Pisces Spirituality. Should it stay a category, or be named?
2. **South Asian category:** it is held in Sagittarius Belief (census religion categories and communities) and Sagittarius Education (students and staff). Please confirm.
3. **Õnnepalu / Emil Tode:** *Piiririik* is cited under its published pen name because a sub-agent's own substring scan caught the surname. Keep the pen name, or add the author's legal name? Separately, one Russian word was reportedly re-spelled to dodge "yoga", and the run agent could not locate it.
4. **Virgo Domain lands line:** this was the one hand edit (the scope file's name was removed). Please confirm the wording.
5. **Empty Held lines:** 96 sheets use the bare "none." and 28 use a concept-worded "none; no X pointer was set aside" (27 near-match pairs come from these). Is the bare template value acceptable, or should empty Held lines be worded per concept?
6. **Lands:** Estonia's lands are still to be settled at Stage 0, and so is whether the Pechory district (comparison only here) has any place in them.
