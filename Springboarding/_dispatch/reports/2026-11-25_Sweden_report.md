# Sweden: springboard scouting report (2026-11-25)

Run agent: Sweden, all twelve signs, deeper brief, one sub-agent per sign. Scouting only; nothing is verified.

## Result
- **130/130 sheets done**, 12 sign agents, **0 relaunches**.
- **Whole-nation QA (`springboard_qa.py Sweden`): 130 sheets, 0 problems.**
- **Repeat check (own scripts):**
  - Within Sweden: 0 exact repeats (lines, table rows, compare bullets, Flags lines, first queries), and 0 near matches at 0.85 across 2,414 compare, Flags and first-query items.
  - Against Norway (87 sheets present at the end), Finland (130) and Estonia (130): 0 exact repeats after one fix (below), and 0 near matches at 0.85 against 5,936 items.
  - Denmark and Iceland have no sheets yet.
- **Sub-agent tokens:** 2,910,979 in total (684 tool calls).
- **Wall clock:** 10:10 to 15:20.
  - The harness forced one interim hand-back at 13:49. The coordinator resumed the run at 13:50, and no duplicate agent was launched.
  - No usage-limit stop.
- **Length:** average 1,253 words by `wc -w` (1,112 to 1,299). 112 sheets are over 1,200 and none is over 1,300.
- **Pointers:** 12 to 16 per sheet, average 14.2 (12: 1 sheet; 13: 21; 14: 60; 15: 42; 16: 6).

## Per sign
| # | Sign | Sheets | Relaunches | QA | Avg words | Longest | Shortest | Pointers | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 0 | 0 | 1,195 | 1,262 Domain | 1,112 Recklessness | 13-16 | 178,063 | 10:11-10:27 |
| 2 | Taurus | 11 | 0 | 0 | 1,221 | 1,282 Ownership | 1,181 Security | 13-14 | 218,566 | 10:28-10:47 |
| 3 | Gemini | 10 | 0 | 0 | 1,258 | 1,287 Domain | 1,227 Curiosity | 13-14 | 217,755 | 10:48-11:09 |
| 4 | Cancer | 10 | 0 | 0 | 1,295 | 1,299 (three) | 1,286 Motherhood | 12-15 | 250,187 | 11:10-11:33 |
| 5 | Leo | 13 | 0 | 0 | 1,279 | 1,299 Honor | 1,230 Leadership | 13-15 | 267,140 | 11:34-12:01 |
| 6 | Virgo | 10 | 0 | 0 | 1,234 | 1,290 Domain | 1,181 Health | 13-14 | 248,027 | 12:03-12:29 |
| 7 | Libra | 11 | 0 | 0 | 1,257 | 1,292 Domain | 1,197 Indecision | 13-15 | 273,341 | 12:30-12:53 |
| 8 | Scorpio | 11 | 0 | 0 | 1,235 | 1,280 Control | 1,172 Secrecy | 14-15 | 234,792 | 12:54-13:17 |
| 9 | Sagittarius | 11 | 0 | 0 | 1,277 | 1,295 Faith | 1,227 Honesty | 15 | 261,001 | 13:18-13:48 |
| 10 | Capricorn | 10 | 0 | 0 | 1,267 | 1,299 Domain, Duty | 1,222 Ambition | 14-15 | 231,981 | 13:50-14:08 |
| 11 | Aquarius | 10 | 0 | 0 | 1,235 | 1,276 Group | 1,206 Hope | 15-16 | 225,195 | 14:09-14:23 |
| 12 | Pisces | 12 | 0 | 0 | 1,280 | 1,299 Boundary | 1,248 Intuition | 13-15 | 304,931 | 14:24-15:12 |

## Rule breaks and fixes (3 hand edits, no relaunches)
1. **Aries, Competition:** a North Sámi search-term row (*gilvu*) matched a row in Finland's Competition sheet word for word.
   - Fix: I rewrote the Notes cell for Sweden.
   - From Taurus on, the prompt told the sub-agents to make shared Sámi, Finnish and Meänkieli rows specific to Sweden. No cross-nation row repeated after that.
2. **Sagittarius, Travel:** the Held line described the set-aside eighteenth-century voyage account closely enough to narrow it down (lesson 14).
   - Fix: I cut it back to the category only.
3. **Pisces, Self-sacrifice:** the Held line described the set-aside recent protest case closely enough to identify it.
   - Fix: I cut it back to the category only.

**False positives** (all kept as written):
- My own name scan, which is broader than the QA scan, caught "citizen" and "frozen" (Gemini) and "sikh" inside *Musikhjälpen* (Leo).
- The Sagittarius sub-agent worried that *blanka röster* (Libra, Indecision) contains "lanka". The QA scan does not catch it.
- None of these is a South Asian item.

**Other rules:**
- **Lands:** the note appears once, in each Domain sheet's Flags; no sheet names a scope file, and no unit list was added.
- **Hermes:** not opened.
- **Universals:** none mentioned.
- **"Indian":** none.
- **Law:** letter of the law only in Libra, spirit only in Capricorn; every other sign points law to those two.
- **Contested ground:** the race-biology institute, the sterilization laws, the Sámi land cases and the Truth Commission, the Travellers and Roma, wartime neutrality and the integration debates appear as accounts or as sources to read critically.

## Held lines
- **South Asian category, actually set aside (7 sheets):** Aries Competition; Sagittarius Domain, Belief, Education, Fundamentalism and Travel; Pisces Self-sacrifice.
- **Rule named with nothing set aside:** about 35 other Held lines, mostly in Aries to Gemini and Sagittarius, end with a clause saying no pointer came under the South Asian rule. Each is worded for its sheet, and none uses the category. The author may want such clauses dropped in later runs if they read as routine.
- **Buddhism, as a category only (12 sheets):** Taurus Sensuality; Scorpio Rebirth; Sagittarius Domain, Meaning and Belief; Capricorn Discipline; Aquarius Detachment; Pisces Domain, Dissolution, Escapism, Spirituality and Surrender. No community, temple or text is named.
- **Empty Held lines:** none is a bare "none."; each names what was weighed.

## Thin, repetitive or generic sheets
- **Repetition:** none found by the scripts, either within Sweden or across nations.
- **Fewest pointers:** Cancer Domain, with 12 (still within the brief).
- **Cancer runs tight on length:** all ten sheets are 1,286 to 1,299 words, close to the scan's 1,300 line. Nothing reads padded in the spot-checks.
- **Generic:** no sheet read generic in the spot-checks (Aries Domain in full; the Held lines and compare bullets of every sign).

## Depth (how many of the 130 sheets mention each item, by text search)
- **Regions:**
  - Sápmi 130, Norrbotten and the Torne Valley 127, Stockholm and the Mälardalen 123, Skåne 101, Gothenburg and Västra Götaland 86, Uppland 72, Småland 71, Gotland 66, Dalarna 63, Västerbotten 61, Jämtland and Härjedalen 48, Värmland 47, Bergslagen 40, Öland 38, Halland and Blekinge 35, Östergötland 28.
- **Peoples:**
  - Sámi 130, Meänkieli and Tornedalians 127, Somalis 115, Iranians 112, Sweden Finns 109, Kurds 103, Roma and the Travellers 101, Bosniaks 101, Eritreans 94, Jewish community 89, Assyrians and Syriacs 84, Iraqis and Syrians 84, Laestadians 83, Chilean exiles 80, free churches 66, Muslim communities 57, Catholics 31, Estonian Swedes 26, Swedish Sign Language 17.
- **Pre-modern pointers:** a rough scan finds them in at least 100 sheets (runestones 18, Birgitta and Vadstena 14, provincial laws and the Land Law 10, Linnaeus 10, Olaus Magnus 5, Schefferus 5, *husförhörslängder* 3, the 1734 Code 3). Everything else comes from the wider pre-modern record: sagas, early modern ordinances and parish sources.
- **Verdict:** the sheets use the nation's depth well, especially for the Sámi, the Torne Valley and the newer communities.
- **Lighter spots:** Östergötland, Catholics, Estonian Swedes and Swedish Sign Language are lighter. So are several of the named classical sources (Olaus Magnus, Schefferus, the household examination registers), which appear in only a handful of sheets each.

## Judgment calls for the author
1. **Afghanistan under the South Asian rule.** The Cancer sub-agent counted Afghanistan as South Asian. Before finishing, it replaced an Afghan-origin compare bullet in Nurture with Eritrean parents. Confirm whether Afghan communities count under the rule. If they do not, Nurture could get the bullet back.
2. **Swedish East India Company (Gothenburg, 1731-1813)** is a pointer on Taurus Wealth, under its own historical name. It is a Swedish company, it traded mainly with China, and the scan does not catch it. Confirm it may stay.
3. **Buddhism** is held as a category on 12 sheets, five of them in Pisces. These wait on the author's open question.
4. **Seven South Asian set-asides** are listed above, all as categories only. Two of the Held lines were cut back by hand so the held items cannot be identified.
5. **Shared Sámi vocabulary** with Norway and Finland. The search-term rows were made Sweden-specific. The terms themselves (the same North Sámi words) naturally recur across the three nations.
