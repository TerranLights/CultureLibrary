# Norway: springboard scouting report (2026-11-25)

**Result: 130 of 130 sheets done** (`springboard_status.py Norway`). Whole-nation QA (`springboard_qa.py Norway`) found **0 problems**. The run used 12 sign sub-agents and **0 relaunches**. The Cancer sub-agent stalled on a background step of its own with one sheet in progress, and one message brought it back. Brief: the deeper brief (Priority block), one sub-agent per sign. Run agent: Norway run agent (wave 2).

- **Wall clock:** 10:27 (start) to 17:24 (checks done). One break: the harness asked for an early hand-back at 12:08, the main session resumed the run at 12:09, and it went on without a gap.
- **Sub-agent tokens:** **2,915,162** in all, with 836 tool uses. Run-agent tokens are not counted here.
- **Sheets:** 1,227 words on average by `wc -w` (1,066 to 1,299). Pointers: 1,801 in all, 12 to 16 per sheet (average 13.9).

## Per sign

| # | Sign | Sheets | Sub-agent tokens | Tools | Time | Avg / min / max words | Pointers | QA | Run-agent edits |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 177,255 | 48 | 10:27-10:42 | 1,211 / 1,115 / 1,290 | 165 (14-16) | 0 | 1 |
| 2 | Taurus | 11/11 | 221,616 | 57 | 10:47-11:20 | 1,225 / 1,071 / 1,297 | 153 (12-15) | 0 | 1 |
| 3 | Gemini | 10/10 | 220,241 | 53 | 11:20-11:35 | 1,224 / 1,167 / 1,263 | 140 (13-16) | 0 | 2 |
| 4 | Cancer | 10/10 | 232,306 | 92 | 11:36-12:09 | 1,246 / 1,197 / 1,299 | 138 (13-14) | 0 | 0 (resumed once) |
| 5 | Leo | 13/13 | 255,903 | 63 | 12:11-13:10 | 1,198 / 1,152 / 1,284 | 185 (13-16) | 0 | 2 |
| 6 | Virgo | 10/10 | 250,224 | 51 | 13:13-14:03 | 1,222 / 1,172 / 1,278 | 142 (14-15) | 0 | 0 |
| 7 | Libra | 11/11 | 266,741 | 77 | 14:07-14:35 | 1,184 / 1,066 / 1,278 | 152 (12-15) | 0 | 0 |
| 8 | Scorpio | 11/11 | 267,845 | 87 | 14:38-15:13 | 1,250 / 1,216 / 1,291 | 146 (13-14) | 0 | 0 |
| 9 | Sagittarius | 11/11 | 239,852 | 78 | 15:17-15:50 | 1,243 / 1,150 / 1,285 | 142 (12-14) | 0 | 0 |
| 10 | Capricorn | 10/10 | 260,797 | 77 | 15:52-16:38 | 1,279 / 1,252 / 1,298 | 131 (12-14) | 0 | 1 |
| 11 | Aquarius | 10/10 | 265,373 | 78 | 16:40-16:59 | 1,268 / 1,198 / 1,299 | 139 (13-15) | 0 | 1 (+1 at the end) |
| 12 | Pisces | 12/12 | 257,009 | 75 | 17:00-17:20 | 1,197 / 1,108 / 1,252 | 168 (13-15) | 0 | 0 (+1 at the end) |

## Rule breaks and fixes (10 smallest edits by the run agent, no relaunches)

**Near repeats of Sámi search-term rows against Finland (3 edits).** Three rows for common words matched Finland's same-named sheets at 0.85 to 0.95: Aries Anger (*suhttat*), Gemini Duality (*guovttegielat*) and Gemini Mediation (*soabadeapmi*). I gave each row a Notes cell specific to Norway and the concept. From Cancer on, the sub-agent prompt asked for such a cell on every Sámi and Kven row, and no near repeat came back after that.

**Held lines that described a held item or the author's question (4 edits).**
- Taurus Values referred to "any religion the author has left open". I reworded it for the concept.
- Leo Joy's Buddhism line described the held pointer. I cut it to the category.
- Capricorn Merit tied the South Asian category to "the mobility measures". I cut it to the category.
- Aquarius Detachment's Buddhism line described the tradition "beside the monasteries". I cut it to the category, then reworded it once more when my own edit came out as a near match (0.86) of Joy's line.

**A compare bullet that linked communities to a social problem (1 edit).** Leo Honor linked Muslim, Kurdish, Somali, Eritrean and Iraqi Norwegians to "honor-violence policy". I reworded it to each community's own words for honor and its part in the debate. From Virgo on, the prompt forbade tying a named community to a social problem.

**Missing pre-modern pointer (1 edit).** Pisces Empathy was the only sheet with nothing older than a 2008 film. I added Petter Dass's *Nordlands Trompet* (c. 1700) with a reason specific to the concept. Every other sheet has one, though on a few the oldest is 19th century (see "Depth" below).

**Final check.** The whole-nation repeat check found 0 exact repeats of a line, table row, compare bullet, Flags line or first query within Norway or against Sweden's (130 sheets, in progress or done) and Finland's sheets, at any length. It also found 0 near matches at 0.85 after the edits above.

**Known false positives and kept words:**
- **"Afghanistan"** on Leo Honor names Norway's military mission, in the veterans' day row. It is not a community, so I kept it.
- **"temple"** on Pisces Spirituality is the gloss of Old Norse *hof*, so I kept it.

**Scans with no hits:**
- No universals, no Hermes, no "Indian", no URLs.
- No South Asian name anywhere outside the Held line.
- No zodiac words.
- The missing-scope note appears once, in Aries Domain.

## Held lines

- **South Asian category, 6 sheets**, category only, with nothing named or described: Aries Identity and Anger, Gemini Mediation, Capricorn Ambition and Merit, Aquarius Idealism. Ambition and Merit say "scholarship by South Asian-heritage scholars abroad". Capricorn's concept block suggests social-mobility atlases, and the sub-agent used Statistics Norway (SSB) register data instead.
- **Buddhism, 3 sheets**, category only: Leo Joy, Aquarius Detachment, Pisces Spirituality.
- **Empty Held lines.** Every other Held line names what was weighed for that concept and why it was left out.

## Thin, repetitive or generic sheets (by name)

**Thinner sheets:**
- **Taurus Possessiveness** (1,071 words, 12 pointers, 4 regions).
- **Libra Indecision** (1,066 words, 13 pointers) and **Libra Reciprocity** (12 pointers).
- **Sagittarius Belief, Conviction and Honesty** (12 pointers each).
- **Pisces Intuition** (1,108 words).

None is padded. Their concepts have less Norway-specific material.

**Narrower spread of peoples or regions:**
- **Taurus Stability** names 6 of the run's 19 peoples, and **Taurus Wealth** 7.
- **Gemini Mediation** covers 4 of the run's 10 regions.

All other sheets cover 5 to 10 regions and 8 to 19 peoples (averages 7.2 and 13.1).

**Formulaic Held lines:**
- **Aries, Taurus and Cancer** Held lines close on a near-identical clause, "no <concept> pointer fell under the South Asian rule". Each is worded for its concept, and the exact and near checks pass. The prompt dropped this pattern from Leo on.
- **Pisces:** ten Held lines share one theme (data sorted by origin, set aside for the communities' own sources), each worded for its concept.

**Sources that recur:**
- The broad national ones are expected: SSB on 61 pointer rows, the National Library (nb.no) on 52, NRK on 49.
- Asbjørnsen and Moe recur on 23 rows and Ibsen on 18.
- The Jante idea is on 8 sheets. Aquarius steered away from it and from *Draumkvedet* on purpose and said so on its Held lines.
- No single specialist source dominates. Gullestad appears on 3 sheets and Ungdata on 5.

## Depth: do the sheets exploit Norway's depth?

**Yes, broadly.**
- **Regions:** every sign covers Oslo and Østlandet, Vestlandet, Trøndelag, Northern Norway, Finnmark and Svalbard (Longyearbyen, often with Barentsburg). Sørlandet, Telemark and Setesdal, the inland valleys and Finnskogen recur in most signs.
- **Peoples:** North, Lule and South Sámi (often kept apart), Kvens and Forest Finns appear from the first sign, each with a note where sources are scarce. So do the *tatere* and the Rom (kept apart), the Jewish community, Laestadians, Haugean and *bedehus* communities, and the Polish, Lithuanian, Somali, Eritrean, Iraqi, Kurdish, Syrian and Vietnamese communities.
- **Search terms** come in Bokmål and Nynorsk, dialect forms, North and South Sámi, Kven, Romani and the newer communities' languages.
- **Pre-modern pointers** run through the whole nation: the Gulating and Frostating laws, the Land Law, *Konungs skuggsjá*, the Bryggen runes, the homily book, *Draumkvedet*, Landstad, Asbjørnsen and Moe, Aasen, the missionaries' Sámi records and Petter Dass. On a few sheets the oldest pointer is 19th century (Taurus Sensuality, Libra Indecision and Projection), a weaker form of the rule.

**Contested ground is given as accounts:** Norwegianization and the 2023 commission, Alta, Fosen, the treatment of the *tatere*, 1942, the occupation, the treason settlement and the war children.

**Law:** the letter stays in Libra and the spirit in Capricorn. Crime in Scorpio and Pisces stays moral and social.

## Judgment calls for the author to confirm

1. **Lands.** The sheets cover Norway as it stands, with Svalbard. Sámi beyond Norway, Sweden, Finland, Denmark, Iceland, Greenland and the Upper Midwest diaspora are comparison only. Several sheets compare Longyearbyen with **Barentsburg**, the Russian settlement on Svalbard. Should Barentsburg's residents count as part of Norway's people, or only as comparison?
2. **Buddhism** is held on 3 sheets. The Vietnamese Norwegians appear only through Catholic parishes, so the Buddhist side of that community is not pointed to anywhere, by design of the hold.
3. **The old laws outside Libra and Capricorn.** I told the sub-agents to treat the Gulating and Frostating laws, the Land Law and the Constitution as historical and social records, not as law research. Please confirm that reading.
4. **"Afghanistan"** (Norway's mission) on Leo Honor was kept as a place, not a South Asian community.
5. **Capricorn Duty's Held line** says the jury (*lagrette*) ended in 2018. It is marked *check* and needs verifying.
6. **The South Asian category wording** "scholarship by South Asian-heritage scholars abroad" on Ambition and Merit (as on earlier nations' Capricorn sheets).

## Operations notes

- **The stall.** The Cancer sub-agent stopped to wait on its own background command and left Motherhood "in progress". One message finished it. From Leo on, the prompt said to run every check in the foreground.
- **Slow checks.** As Sweden and Finland grew, the sub-agents' end-of-sign re-checks across all sheets ran past the two-minute tool limit (Virgo, Sagittarius, Capricorn). Each sheet had already been checked before it was marked done. My check script got a word-set prefilter to stay fast.
- **Prompt additions during the run** (none changes the brief):
  - the Sámi and Kven Notes cell;
  - no formula Held lines;
  - foreground checks only;
  - no community tied to a social problem;
  - Buddhism Held lines without description;
  - per-sign law, belief, crime and mobility-atlas notes for Libra, Scorpio, Sagittarius, Capricorn and Pisces.

  The prompt template and helper scripts are in the run agent's scratchpad, `Norway/_run/`.
