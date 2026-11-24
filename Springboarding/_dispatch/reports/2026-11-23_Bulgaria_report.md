# Bulgaria springboard run: report (2026-11-23)

**Result:** 130/130 sheets done (`springboard_status.py`), whole-nation QA **0 problems** (`springboard_qa.py Bulgaria`), own repeat check across the nation **0 exact repeats** (lines of 40+ characters, table rows, "Who to compare" bullets, Flags lines, first queries; the template's two fixed header lines excepted) and **0 near matches** at 0.85 among compare bullets and Flags lines.
**Wall clock:** 09:55 (start) to 13:05 MST. **Sub-agent tokens:** 2,767,259 in all (12 sign agents 2,398,199; 2 fix agents 200,294; 3 single-concept relaunches 168,766). No usage-limit stop and no forced hand-back.
**Folder:** `Targets/Europe/Bulgaria/Springboards/` (12 sign folders).

## Per sign

| # | Sign | Sheets | Agents | Fixes | QA | Avg words | Longest | Pointers | Tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 3 run-agent edits (Languages lines, made after Leo) | 0 | 1,240 | 1,291 Identity | 14-15 | 173,817 | 09:56-10:10 |
| 2 | Taurus | 11 | 1 | none | 0 | 1,184 | 1,277 Ownership | 13-15 | 202,285 | 10:12-10:26 |
| 3 | Gemini | 10 | 1 | 7 Held lines (by the Libra fix agent) | 0 | 1,156 | 1,254 Domain | 14-15 | 194,014 | 10:28-10:41 |
| 4 | Cancer | 10 | 1 | 1 run-agent edit (Nurture Held line) | 0 | 1,149 | 1,277 Domain | 14 | 175,578 | 10:43-10:52 |
| 5 | Leo | 13 | 1 + fix + 1 relaunch | 13 Languages lines (fix agent); Joy relaunched for a pre-modern pointer | 0 | 1,158 | 1,292 Domain | 14-15 | 207,657 + 90,477 + 55,687 | 10:55-11:11, 13:02 |
| 6 | Virgo | 10 | 1 | none | 0 | 1,203 | 1,282 Domain | 14-16 | 205,160 | 11:10-11:25 |
| 7 | Libra | 11 | 1 + fix | 11 Held lines (fix agent); 1 trim (Projection) | 0 | 1,244 | 1,300 Projection | 15-16 | 218,749 + 109,817 | 11:27-11:46 |
| 8 | Scorpio | 11 | 1 + 1 relaunch | Revenge relaunched for a pre-modern pointer | 0 | 1,185 | 1,269 Rebirth | 14-15 | 205,657 + 55,617 | 11:43-11:58, 13:02 |
| 9 | Sagittarius | 11 | 1 | none | 0 | 1,253 | 1,275 Truth, Conviction | 14-15 | 205,034 | 12:00-12:14 |
| 10 | Capricorn | 10 | 1 | none | 0 | 1,215 | 1,264 Domain | 14-15 | 196,522 | 12:16-12:29 |
| 11 | Aquarius | 10 | 1 | none | 0 | 1,183 | 1,253 Group | 14-15 | 200,626 | 12:31-12:42 |
| 12 | Pisces | 12 | 1 + 1 relaunch | 1 run-agent edit (Spirituality compare bullet); Escapism relaunched for a pre-modern pointer | 0 | 1,196 | 1,284 Domain | 13-15 | 213,100 + 57,462 | 12:44-12:59, 13:02 |

**Words (wc -w):** average 1,198, range 1,077 (Leo Play) to 1,300 (Libra Projection); 65 sheets over 1,200, none over 1,300. **Pointers per sheet:** 13 to 16, average 14.6 (3 sheets with 13, 54 with 14, 70 with 15, 3 with 16).

## Rule breaks and fixes
- **Pre-modern pointers:** a final check across the nation found 3 sheets with no written source from before about 1800: Leo Joy, Scorpio Revenge and Pisces Escapism. Their oldest pointers were folk customs, curse formulas, *gurbet* songs and Hitov's memoirs of the 1870s. I relaunched each as a single-concept job to add one row, and each passed on its first try:
  - Joy: the *damaskini* miscellanies, given as a query.
  - Revenge: the kadı *sicil* of Sofia, Vidin and Ruse, used for feuds and blood-money settlements as social practice, not law.
  - Escapism: the medieval Lives of St. Ivan of Rila, including Patriarch Evtimiy's version.

  Every sheet now has a pre-modern pointer. Scorpio Crisis already had one (manuscript marginal notes, *приписки*), which my pattern scan had missed.
- **QA flags:** QA never flagged a sheet. The other fixes came from the run agent's own checks (lesson 6):
  - **Leo:** all 13 "Languages needed" lines were bare language lists, three of them near-copies (0.90-0.91). A fix agent rewrote each one to tie every language to that sheet's own pointers. From Virgo on, the prompt said explicitly that a bare list is not enough.
  - **Aries:** Competition, Recklessness and Independence also had thin Languages lines. The run agent rewrote them with the smallest edit.
  - **Libra and Gemini:** 9 near matches (0.86-0.92) came from a formulaic Held line ("none; no X pointer was set aside"). A fix agent rewrote 18 Held lines (all 11 in Libra, 7 in Gemini), giving each a note specific to its sheet. From Scorpio on, the prompt named that formula as one to avoid. The longer line pushed Libra Projection to 1,304 words, and I trimmed it to 1,300.
  - **Cancer Nurture:** its Held line was a near-copy of Aries Beginning's (0.88). I rewrote it to name the sheet's own pointers.
  - **Pisces Spirituality:** a compare-bullet header called White Brotherhood followers "mostly urban", which states a trait. I removed it.
- **STATUS not the last write:** the Leo agent rewrote its 13 Held lines after flipping STATUS, and the Scorpio agent reworded one compare bullet in Death after the flip. All of those files are complete, so this has no effect on the status grid.
- **South Asian names, Buddhism, universals, Hermes, scope file:** I scanned every sheet by hand-built pattern after each sign and once across the nation, for names as well as words. No South Asian scholar, work, community or religion is named anywhere. The only matches were false positives: *homily*, *khan* and Turkish *kibir*. Nothing refers to Human Universals or Hermes_research. The note that the lands are unsettled appears in Domain sheets only, and no sheet tells the reader to read a scope file.
- **Law:** outside Libra and Capricorn, law is routed to those two signs; I checked Taurus Ownership and Possession and Pisces Crime by hand. Libra keeps to the letter of the law (statutes, ECtHR judgments). Capricorn Law keeps to its spirit (customary law, haiduk legitimacy, the Roma *kris*, data on how the rule of law is perceived).

## Thin, repetitive or generic sheets
- No sheet is generic. The ones that read a little thinner than the rest (fewest pointers or words) are: Leo Play (1,077 words), Pisces Intuition (1,082 words, 13 pointers), Scorpio Power (1,085 words), Pisces Surrender and Taurus Stubbornness (13 pointers each). Each still has its own sources.
- Repetition was limited to the Flags-line formulas above, and all of them are fixed. The Held lines that say plainly "nothing held" now each add a concrete note for their own sheet.

## Does the run use the nation's depth?
Yes, broadly. This is the number of the 130 sheets (and of the 12 signs) that mention each item:

- **Regions:**
  - Kardzhali: 124 sheets
  - Upper Thrace: 110
  - Rhodopes: 109
  - Ludogorie: 102
  - Northwest: 90
  - Black Sea coast: 87
  - Danubian Plain: 75
  - Shopluk: 70
  - Dobruja: 70
  - Pirin: 64
  - Stara Planina towns: 60
  - Strandzha: 51
  - Sredna Gora: 21 (the thinnest region; it appears in 10 signs)
- **Peoples:**
  - Roma: 128
  - Pomaks: 124
  - Armenians: 98
  - Turks (by that name): 92
  - Sephardic Jews: 87
  - Karakachans: 86
  - Gagauz: 69
  - Lipovans: 63
  - Catholics and Paulicians: 61
  - Alevi (Kızılbaş and Babai): 60
  - Aromanians: 56
  - Thracian and Macedonian refugee families: 46
  - Protestants: 44
- **Pre-modern sources:** every sheet has at least one (after the 3 relaunches). Across the nation:
  - Rila: 30 sheets
  - *defters* and *sicil*: 20
  - Bogomils: 18
  - *chitalishte*: 17
  - Paisius: 11
  - *damaskini*: 12
  - Also used: the *Zlatostruy*, the Omurtag inscriptions, the Synodikon of Boril, the Responsa of Nicholas I, the *Zakon sudnyi lyudem*, the Rila Charter and the Bachkovo typikon.
- **Weakest spots:** the Sredna Gora; Protestants beyond the Roma Pentecostal churches; the refugee families of the 1910s-20s. A future pass could push these.

## Judgment calls for the author
1. **Lands:** no `00 - Scope.md` exists and the tracker header settles nothing, so the sheets write for Bulgaria as it stands, add no unit list and settle no borders. The note that the lands are unsettled appears once per Domain sheet.
2. **Buddhism (open question):** held as a category, with nothing named, in Aquarius Detachment (meditation groups in Bulgarian cities) and Pisces Spirituality.
3. **South Asian category:** used on one sheet only, Pisces Spirituality ("South Asian-heritage and South Asian-derived practice communities in the nation's lands"), where a real pointer was set aside.
4. **Published names:** the English name of the "International Centre for Minority Studies and Intercultural Relations" (IMIR, Gemini Mediation) is kept as published, with British "Centre".
5. **Contested ground, presented as contested:**
   - the Pirin region's Bulgarian or Macedonian self-descriptions (Aries Identity)
   - how Pomaks are counted and what they are called (Cancer Belonging, Gemini Domain)
   - the memory of Batak in 1876 (Pisces Self-sacrifice)
   - 1943: rescue inside the old borders, deportation from the occupied lands (Aries Identity)
6. **Sources left out on purpose; please confirm:**
   - Pisces Surrender: a chronicle claimed for the Chepino conversions is left out pending a historian's assessment of its authenticity.
   - Sagittarius Fundamentalism: security-service sources on present-day radicalization are left out as too restricted.
   - Leo: images of Rhodope weddings and rituals are marked as waiting on community consent.
7. **Dates:**
   - The Law for the Protection of the Nation is dated 1940 in Libra Projection and 1941 in Capricorn Law. It passed in December 1940 and took effect in January 1941, so both dates are defensible; the later research should settle on one.
   - Leo Honor gives *pativ* as both the Romani and the Armenian word for honor. Both are real words, and the match is a coincidence worth a check.
8. **Comparison only:** Turkish, Greek and North Macedonian scholarship appears only where a Bulgarian topic needs it: Robert College, the joint history commission, and Campbell's Greek fieldwork on honor. The emigrants of 1989 and the Bessarabian and Banat Bulgarians are cited as comparison only.
9. **QA script note:** its `indo-` pattern would flag "Indo-European" (for example in Thracian topics). No sheet used the word, but a later run might.
