STATUS: done 2026-11-23. Run agent's report; the sheets are unverified.

# France: springboard run report (deeper brief)

**Result:** all 130 sheets are done, and every first line reads `STATUS: done 2026-11-23, not verified`. The run used 12 sign agents and needed **no relaunch**. The whole-nation QA (`springboard_qa.py "France"`) found **0 problems** in 130 sheets. The run agent made 6 small hand edits, listed below.

**Tokens and wall-clock:**
- **Sub-agent tokens:** **3,059,841** for the 12 sign agents, as reported by the harness, with 779 tool uses. The run agent's own tokens are not included; the main session adds them.
- **Wall-clock:** the run agent started at **05:04 MST**. The Aries agent launched at 05:05 and the Pisces agent finished at 08:32. The checks and this report were done by **about 08:34 MST**, about **3 h 30 min** in all.
- **No stops:** the run hit no usage limit.
- **Cost trend:** the sign agents grew from 166k tokens (Aries) to 290k to 317k (Capricorn to Pisces). The later agents read the earlier signs' sheets to avoid repeats, as the prompt told them to.

## Per-sign table
| # | Sign | Sheets | Agents | Relaunches | QA | Hand edits | Avg words | Longest | Pointers (avg, range) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 0 | 1,228 | 1,275 (Self-assertion) | 14.7 (14-15) | 165,981 | 05:05-05:19 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 2 | 1,274 | 1,295 (Security) | 15.0 (13-16) | 213,337 | 05:20-05:34 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 3 | 1,255 | 1,297 (Communication) | 15.4 (15-16) | 222,130 | 05:35-05:48 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 0 | 1,213 | 1,297 (Domain) | 14.7 (14-15) | 227,462 | 05:49-06:01 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 0 | 1,247 | 1,285 (Domain) | 14.9 (13-16) | 245,469 | 06:02-06:17 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 0 | 1,256 | 1,294 (Work) | 15.3 (14-16) | 267,458 | 06:18-06:34 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 0 | 1,217 | 1,296 (Domain) | 14.0 (13-15) | 268,264 | 06:35-06:50 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 0 | 1,236 | 1,297 (Domain) | 13.7 (13-15) | 281,573 | 06:51-07:11 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 0 | 1,264 | 1,295 (Faith) | 13.7 (13-15) | 272,059 | 07:12-07:32 |
| 10 | Capricorn | 10/10 | 1 | 0 | 0 | 1 | 1,225 | 1,277 (Duty) | 13.8 (13-14) | 290,857 | 07:33-07:54 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 0 | 1,233 | 1,296 (Domain) | 13.4 (13-14) | 317,254 | 07:54-08:11 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 0 | 1,271 | 1,290 (Spirituality) | 14.2 (13-15) | 287,997 | 08:12-08:32 |
| | **Total** | **130** | **12** | **0** | **0** | **6** | **1,244** | **1,297** | **14.4 (13-16)** | **3,059,841** | **05:05-08:32** |

- **Word counts:** by `wc -w`, markup included, after the hand edits.
  - The shortest sheet is Libra/Peace at any price, at 1,136 words.
  - The longest are Gemini/Communication, Cancer/Domain and Scorpio/Domain, at 1,297 each.
  - 107 of the 130 sheets run over 1,200 words, and none is over the 1,300 flag.
- **Pointers:** these are the rows of section 2.
  - 14 sheets have 16, 47 have 15, 47 have 14 and 22 have 13.
  - "Who to compare" has 8 to 14 bullets per sheet (average 11.4).

## Rule breaks and fixes
**QA:** the scan flagged nothing in any sign or in the whole-nation pass. Through the hand edits it stayed at 0, after one fix: my first Taurus/Security edit pushed that sheet to 1,305 words, so I shortened my own wording and it came back to 1,295.

**Hand edits (smallest edit each; no relaunch was needed):**
1. **Taurus/Sensuality:** a Vietnamese-French and Chinese of Paris compare bullet (Lunar New Year and the 13th arrondissement) nearly copied Aries/Beginning. I reworded it to the concept: festival dishes and home cooking across generations.
2. **Taurus/Security:** a Chinese of Paris and Vietnamese-French bullet on rotating credit nearly copied Aries/Independence. I reworded it to who a tontine or family loan covers when banks refuse.
3. **Gemini/Information:** the "Sensitive or restricted" line opened with the same clause as Aries/Identity's (on French statistics and ethnic categories). I reworded the clause.
4. **Gemini/Learning:** the "Sensitive or restricted" line opened with the same clause as Aries/Competition's (on school results by origin). I reworded the clause.
5. **Gemini/Domain:** the lands note opened like Aries/Domain's. I reworded its opening.
6. **Capricorn/Discipline:** a Jewish-communities bullet on Paris and Strasbourg yeshivas nearly copied Virgo/Analysis. I reworded it to teaching Shabbat and kashrut to children as self-rule.

From Gemini on, each prompt named the repeat patterns already found, and the later sign agents cleared repeats themselves. Several reopened sheets to do so, and in each case they rewrote the STATUS line last.

**Repeat check (my own, whole nation):** I checked lines of 40 characters or more, table rows, compare bullets and Flags lines.
- Nothing is copied exactly.
- Two kinds of near-match remain, both accepted:
  - **Held lines:** most Held lines open with the brief's category phrase ("South Asian-heritage communities in the nation's lands"). Each then gives its own concept-specific reason.
  - **Languages lines:** two Taurus "Languages needed" lines (Values, Security) share their first clause, "French; German and Luxembourgish for Luxembourg's …". The rest of each line differs.
- Only one pointer name repeats across the nation: Corbin, Courtine and Vigarello as editors. They are two different works, *Histoire des émotions* (Aries/Domain) and *Histoire du corps* (Aries/Anger).

**South Asian rule:**
- My own scan after each sign was clean. It looked for South Asian place, people, religion and scholar names, the former French trading posts, and the South Asian-origin communities of Réunion.
- No sheet names a South Asian work, scholar, community, language, religion or place outside the Held line, and every Held line is category-only.
- There were no false positives from the scan's patterns.

**Law:**
- **Libra:** kept to the letter of the law. I checked Justice by hand: the *Olim*, letters of remission, the penal codes of the three lands, and the Outreau, Dutroux and Bommeleeër cases.
- **Capricorn:** kept to the spirit. I checked Law by hand: Carbonnier's *non-droit*, Garapon, *Crainquebille*, the traffic-fine amnesties and trust-in-justice barometers. It names no codes or statutes.
- **Other signs:** the word "statute" appears only for statutes of confraternities, a chivalric order and a medieval university, and in notes that point the law on to Libra and Capricorn.
- **Pisces/Crime:** kept to wrongdoing as a moral and social category.

**Lands:**
- The tracker lists no settled lands and there is no `00 - Scope.md`.
- The lands note appears once in each sign's Domain sheet (12 of 12), each worded differently, and in no other sheet.
- No sheet tells the reader to check a scope file, and no unit list was added.
- The core is metropolitan France with Corsica, Wallonia, Brussels and Luxembourg.

**Other rules:** no zodiac, divination-label or horoscope words, no "Indian" and no "Indo-" compounds. No sheet mentions Human Universals or any universals list, and none uses Hermes_research.

## Thin, repetitive or generic sheets
- **None reads as generic.** Sample reads were Aries/Courage, Cancer (all pointer lists), Libra/Justice and Capricorn/Law. They show concept-specific, often regional pointers, for example:
  - the *Combat des Trente*;
  - Courrières and Marcinelle;
  - the Bommeleeër trial;
  - Corsican *voceri*;
  - Patrick Williams on the Manouches;
  - the Zinneke Parade.
- **Fewest pointers (13):** 22 sheets.
  - Taurus: Possessiveness.
  - Leo: Honor.
  - Libra: Reciprocity, Indecision, Peace at any price.
  - Scorpio: Domain, Betrayal, Revenge, Power.
  - Sagittarius: Freedom, Belief, Conviction, Honesty.
  - Capricorn: Responsibility, Merit.
  - Aquarius: Group, Equality, Friendship, Nonconformity, Detachment, Hope.
  - Pisces: Self-sacrifice.
  - Aquarius is the leanest sign (average 13.4 pointers).
- **Pre-modern pointer:** present in all sheets but one. Libra/Peace at any price starts at the Dreyfus Affair (1898) and has nothing earlier.

## Does the run use the nation's depth?
Mostly yes. Counts are the number of sheets (of 130) that mention each item.
- **Regions:**
  - Paris 125, Brittany 120, Corsica 112, Occitan 112.
  - Alsace 84, the Nord and Picardy 80, Provence and the Midi 77, the Lyon area and the Alps 60, the Massif Central 50, Lorraine 43.
  - Wallonia and Luxembourg are named in every sheet (at least in its Target line), and Brussels is in 124.
- **Peoples:**
  - Maghrebi-French 124, West African-French 71, the overseas departments 71, Manouche and other Travelers 80, Jewish communities 64.
  - Vietnamese-French 50, Portuguese-French 46, the Chinese of Paris 39, Pieds-Noirs 34, Harkis 34, Armenian-French 19, Protestants 19.
- **Pre-modern sources:** well used throughout, for example:
  - *Girart de Roussillon*, the *Olim*, Froissart, Dhuoda;
  - the *Évangiles des quenouilles*;
  - the Lyon martyrs of 177;
  - Montaigne, Vovelle and the Annales school.
- **Weak spots:**
  - **Regions:** Normandy (25 sheets), Burgundy (28) and Aquitaine/Bordeaux (29) are thinner than their size warrants.
  - **Communities:** Italian-heritage (11), Polish-heritage (3, mostly the Nord mining basin), Turkish and Kurdish (2) and Comorian (0, for example Marseille) are barely reached.
  - **Belgium and Luxembourg:** the German-speaking Community of Belgium does not appear as a group. Luxembourg's Portuguese and Cape Verdean residents appear only lightly.

## Judgment calls for the author
1. **Flemish Belgium.** It is pointed to only as comparison (the lands notes, Belgian-level surveys, the Fourons/Voeren dispute). French Flanders (the Nord) is treated as part of France. Does Flanders belong in this nation, or with the Netherlands?
2. **French Basque Country and Northern Catalonia/Roussillon.** They are named only in the lands notes, as comparison. No sheet treats them as core. Confirm they go to the Basque and Catalan culture-nations.
3. **Overseas departments.** They are pointed to in 71 sheets where a concept needed them (Antillean and Réunion material). Confirm whether they are in the nation's lands or comparison only.
4. **Buddhism.** The Pisces sub-agent treated Buddhism and Zen as South Asian-origin religions and kept them only as a category on Spirituality's Held line. Three earlier sheets name Vietnamese and Chinese Buddhist pagodas and Vietnamese-French Buddhists as East and Southeast Asian communities: Taurus/Values, Scorpio/Rebirth and Sagittarius/Domain. I left both as written. Which reading should hold?
5. **Lands wording.** Every Domain sheet reads the core as metropolitan France with Corsica, Wallonia, Brussels and Luxembourg, pending Stage 0.
