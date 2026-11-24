# Belarus springboard run: report (2026-11-23)

**Run agent:** one per nation, deeper brief (accuracy and depth first), one sub-agent per sign, Aries to Pisces in order. Monday wave 2.
**Result:** 130/130 sheets `STATUS: done 2026-11-23, not verified` by `springboard_status.py`; whole-nation `springboard_qa.py Belarus`: **130 sheets scanned, 0 problems**. No relaunches, no hand edits by the run agent, no usage-limit stop.
**Wall clock:** start 09:55 (first launch 09:56), last sub-agent back 15:28, report 15:30.
**Sub-agent tokens:** **3,276,893** (12 sign agents, 0 relaunches; 873 tool uses).

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA | Avg words | Longest | Pointers | Tokens | Minutes |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,145 | 1,280 (Domain) | 14-16 | 179,538 | 15.8 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,188 | 1,282 (Domain, Ownership) | 13-14 | 198,387 | 13.6 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 1,191 | 1,246 (Duality) | 13-14 | 199,673 | 13.0 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,169 | 1,281 (Domain) | 12-14 | 248,810 | 19.1 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,209 | 1,272 (Being seen) | 13-15 | 272,603 | 32.3 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,196 | 1,289 (Domain) | 12-15 | 252,066 | 20.3 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,263 | 1,290 (Reciprocity) | 12-14 | 270,729 | 22.5 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,260 | 1,291 (Rebirth) | 13-15 | 300,548 | 32.2 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 1,248 | 1,278 (Travel) | 13-14 | 303,352 | 24.0 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1,250 | 1,290 (Domain) | 12-14 | 326,922 | 39.1 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1,253 | 1,287 (Reform) | 13-14 | 382,854 | 30.7 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,257 | 1,296 (Boundary) | 12-13 | 341,411 | 62.3 |
| | **Total** | **130** | **12** | **0** | **0** | **1,219** | 1,296 | 12-16 (avg about 13.6) | **3,276,893** | |

Word counts by `wc -w`: 1,063 (Aries Competition) to 1,296 (Pisces Boundary); none over 1,300. Pointers per sheet: 12 in 14 sheets, 13 in 46, 14 in 58, 15 in 11, 16 in 1.

## Rule breaks and fixes
- **None found by the QA scan or by the run agent's checks**, so no relaunch or hand edit was needed.
- **South Asian rule:** the run agent's own name scan (scholars, writers, works, religions, place names) was clean in all 130 sheets. The category is held on two Held lines, each for a real pointer set aside: Sagittarius *Fundamentalism* (a new religious movement of South Asian origin) and Pisces *Spirituality* (Minsk studios teaching a meditation and body practice of that origin). Every other Held line says none, in its own words.
- **Buddhism:** not named anywhere; no sheet needed it beyond the two holds above.
- **Law:** letter of the law only in Libra (the Statutes of the Grand Duchy are spread over ten of its eleven sheets, each with a different reason); spirit of the law in Capricorn. Elsewhere law is pointed to Libra or Capricorn (Taurus Ownership, Security, Stubbornness; Cancer Family, Protection, Motherhood; Capricorn Duty; Aquarius Reform). "Statute" outside Libra refers only to guild and brotherhood charters (Capricorn Merit, Pisces Compassion).
- **Universals:** no "universal" anywhere in the nation's sheets. Kate Brown's Chernobyl history (*Manual for Survival*) in Aries Autonomy is a different author, not Donald E. Brown; kept.
- **Process notes (no rule broken):** in three signs the sub-agent reworded a sheet after first marking it done (Gemini Learning: one word, "values" to "lessons", without resetting the status line; Capricorn Duty, and Aquarius Group and Equality: reopened to swap a reused source, with the done line rewritten last). All files are complete.
- No Hermes material; no unit list; lands: the missing-scope note appears in each sign's Domain sheet only (12 times, never in a concept sheet).

## Repeat check (whole nation, run agent's own)
- **Exact repeats:** none for any line over 40 characters, table row, "Who to compare" bullet, Flags line or first query (the template's fixed lines aside).
- **Near matches (ratio over 0.85):** 0 among "Who to compare" bullets and first queries. 22 among Held lines that say "none" and differ only in the concept word (most in Gemini, 03 to 08, and Cancer Family and Motherhood: "none; no learning pointer was set aside", "none; no curiosity pointer was set aside", and so on). They are formulaic, not copied; kept.
- **Same source twice:** Ivan Nasovič's proverb collection (1874) is a pointer in Aries *Recklessness* and Aquarius *Domain*, with different reasons; kept.
- The Domain sheets of Taurus and Gemini word the scope note almost the same way (the note is meant to be the same fact once per Domain sheet).

## Thin, repetitive or generic sheets
- **Fewest pointers (12):** Cancer *Care*; Virgo *Improvement*; Libra *Domain*, *Reciprocity*, *Peace at any price*, *Projection*; Capricorn *Hierarchy*, *Merit*; Pisces *Empathy*, *Self-sacrifice*, *Spirituality*, *Surrender*, *Intuition*, *Crime*. None is thin in content; the sheets grew longer per pointer.
- **Trend to watch:** pointers per sheet fell from 14 to 16 in Aries to 12 to 13 in Pisces while length rose from about 1,145 to about 1,257 words, close to the 1,300 scan line. The late sheets give longer reasons per pointer rather than more pointers.
- **Formulaic Held lines:** Gemini 03 to 08 (see above).
- No sheet reads as generic or padded on the run agent's spot reads (Aries Identity, Taurus Ownership and Security, Cancer law lines, Sagittarius Fundamentalism, Pisces Spirituality).

## Does it exploit the nation's depth?
Largely yes. Sheets mentioning each item (of 130): Hrodna, Polesia, Lipka Tatars, Roma, the Jewish and Litvak record, *trasianka* and both Belarusian spellings: 130 each; Old Believers 123; Homiel 109; Viciebsk 104; *kitab* literature 99; Protestant communities 95; Mahilioŭ 81; Chernobyl 76; the Lithuanian border and Astraviec 74; Braslaŭ 72; Navahrudak 67; Greek Catholics (Uniates) 62; Ukrainians of the south 40. Pre-modern pointers recur across signs (Kiryla Turaŭski, Simiaon Polacki, Husoŭski, the Bychowiec chronicle, the voloka survey, the Uniate abolition files, brotherhood statutes, the calendar-song editions); Skaryna is named in 7 sheets and the chronicles (*letapisy*) in 16, so the later research could lean on them more. **Weaker spots:** Ukrainians of the south (40 sheets) and Greek Catholics (62) are thinner than the other groups.

## Judgment calls for the author
1. **Lands:** no `00 - Scope.md` and no settled territory; the sheets are written for Belarus as it stands, with the note once per Domain sheet. Confirm when Stage 0 is set.
2. **South Asian holds:** Sagittarius *Fundamentalism* (a new religious movement) and Pisces *Spirituality* (a meditation and body practice) hold the category only. Confirm that both belong under the rule.
3. **Capricorn *Law*** includes amnesty laws tied to Victory anniversaries (read as mercy and public ritual, the spirit of law) and *kitab* passages on lawful and forbidden (religious law held beside state law). Confirm they sit in Capricorn rather than Libra.
4. **Kate Brown** (Chernobyl historian) is kept in Aries *Autonomy*; she is not the author of *Human Universals*.
5. **Post-2020 sources:** several sheets point to online polls (for example the Chatham House Belarus surveys) and note that independent polling and archive access inside the country have narrowed since 2020. The emigration and the diaspora are kept as comparison only.
6. **Charged titles:** Andrew Wilson's *Belarus: The Last European Dictatorship* is cited under its published title in Taurus *Stability*.

## Files
- Sheets: `Targets/Europe/Belarus/Springboards/01 - Aries/` to `12 - Pisces/` (130 files).
- Run log: 13 lines appended to `_dispatch/SPRINGBOARD_PROGRESS.md` (one per sign and one completion line).
