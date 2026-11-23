# Patani springboard run: report (2026-11-22)

Run agent for Patani (wave 3), deeper brief (accuracy and depth first). One sub-agent per sign, Aries to Pisces, one after another. Nothing in the sheets has been verified; every named item is marked *check*.

## Result
- **130/130 sheets done** (12 signs), 12 sign agents, **0 relaunches**.
- **Whole-nation QA (`springboard_qa.py Patani`): 130 sheets scanned, 0 problems.**
- **Repeat check across the nation** (run agent's own script: every non-template line, table row, "Who to compare" bullet, Flags line and first query; plus a near-match test on sections 3 and 4): **0 exact repeats; 1 near-match**, between two Held lines (Aries Initiative and Taurus Domain). These were different in content, but the Aries line was reworded to fit its concept, by one small hand edit. After the edit, 0 repeats.
- **Sub-agent tokens: 3,118,078** (717 tool uses). Wall clock **12:30 to about 17:05** (first launch 12:32, last return 16:57; no usage-limit stop). The run went past the 15:00 window because the nation was already in flight.
- Words by `wc -w`: average 1,216, range 1,091 to 1,297, none over 1,300 (80 sheets over 1,200). Pointers per sheet: 12 to 15, average 13.5 (1,760 in all).

## Per sign
| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers (avg) | Sub-agent tokens | Tools | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,172 | 1,253 Beginning | 1,113 Initiative | 13-15 (14.1) | 177,480 | 40 | 12:32-12:47 |
| 2 | Taurus | 11 | 1,200 | 1,272 Domain | 1,142 Stubbornness | 13-15 (13.6) | 217,878 | 46 | 12:48-13:02 |
| 3 | Gemini | 10 | 1,178 | 1,270 Domain | 1,091 Gossip | 13-15 (13.9) | 219,608 | 45 | 13:03-13:16 |
| 4 | Cancer | 10 | 1,198 | 1,272 Domain | 1,118 Motherhood | 13-14 (13.6) | 272,981 | 45 | 13:17-13:34 |
| 5 | Leo | 13 | 1,235 | 1,280 Domain | 1,165 Joy | 12-15 (13.6) | 274,043 | 64 | 13:35-13:56 |
| 6 | Virgo | 10 | 1,191 | 1,289 Domain | 1,110 Perfectionism | 13-15 (14.0) | 235,025 | 58 | 13:57-14:13 |
| 7 | Libra | 11 | 1,196 | 1,263 Justice | 1,152 Partnership | 14 (14.0) | 227,678 | 53 | 14:14-14:30 |
| 8 | Scorpio | 11 | 1,218 | 1,261 Purging | 1,180 Revenge | 12-14 (13.5) | 293,859 | 64 | 14:31-14:53 |
| 9 | Sagittarius | 11 | 1,223 | 1,288 Domain | 1,181 Freedom | 12-13 (12.3) | 308,306 | 80 | 14:54-15:25 |
| 10 | Capricorn | 10 | 1,214 | 1,293 Domain | 1,108 Merit | 12-14 (12.9) | 320,845 | 72 | 15:26-15:57 |
| 11 | Aquarius | 10 | 1,278 | 1,297 Equality, Hope | 1,239 Friendship | 13-15 (14.1) | 268,559 | 65 | 15:58-16:26 |
| 12 | Pisces | 12 | 1,268 | 1,292 Self-sacrifice | 1,235 Spirituality | 12-14 (13.2) | 301,816 | 85 | 16:27-16:57 |

## Rules, breaks and fixes
- **Lands:** the tracker lists no settled lands and there is no `00 - Scope.md`. Each sign's Domain sheet states this once and writes for the core (Pattani, Yala, Narathiwat and the Malay-speaking districts of Songkhla and Satun). No other sheet repeats the hedge, and there is no unit list. Nothing was taken from `Hermes_research`.
- **South Asian rule:** after every sign, the run agent scanned for South Asian names, scripture languages, religions and the South Asian-founded movements active in the region. Nothing was found outside the Held lines. All 46 Held lines that name something give a category only, such as South Asian-heritage Muslim families of the towns, a South Asian-founded preaching movement, or the source epic behind part of the shadow-play repertoire. The region's own pre-Islamic past (Langkasuka, Yarang) is named only by local names. One false hit was kept: "dance-drama", caught by the "rama" pattern.
- **Law:** Libra keeps to the letter (statutes, the 1946 Islamic family and inheritance law, courts as written). Capricorn keeps to the spirit (the Law sheet was checked by hand: *maqasid*, forum choice, trust in justice, compliance). Pisces Crime treats wrongdoing as a moral and social category and refers law to Libra and Capricorn (checked by hand).
- **Stereotypes and the conflict:** "Who to compare" bullets were spot-checked in Anger, Gossip, Fundamentalism and Crime. They name what to check, with no group traits. The Flags lines in conflict-related sheets tell the researcher not to characterize any community or movement, and to treat partisan labels as objects of study.
- **Held lines:** in Aries and Taurus, each sub-agent wrote a category into every Held line, which read as a formula. From Gemini on, the prompt asked for a held item only where one was actually set aside. Most sheets now say "nothing held" in words specific to the concept, and none of those lines is copied.
- **Source variety:** in sheets 00 to 04, the Scorpio sub-agent swapped out sources it had reused from earlier signs. Its replacements were checked and are specific to the concept. From Sagittarius on, the prompt said a core source may recur with a new row and reason, but must not be dropped just to avoid a repeat. The sources that recur most are each used no more than three times (the labor force survey and the Asian Barometer) or twice (Teeuw and Wyatt's *Hikayat Patani*, Bradley, Kobkua, Fraser, Ibrahim Syukri, Jory, McCargo, Tej Bunnag, Crisis Group, Golomb, Reid).
- **Other edits:** the single Held-line rewording in Aries Initiative described above. The Virgo sub-agent reworded its own Service Held line after writing the done line. Three Pisces sheets were reworded by their sub-agent to clear near-repeats and length.

## Thin, repetitive or generic sheets
- **Fewest pointers (12):** Leo Honor; Scorpio Revenge, Secrecy and Crisis; Sagittarius Meaning, Freedom, Truth, Belief, Conviction, Honesty, Education and Fundamentalism; Capricorn Merit, Law and Order; Pisces Surrender and Crime. Sagittarius (average 12.3) is the thinnest sign. Pointer counts drifted toward the floor in the later signs, while word counts rose.
- **No clear pre-modern pointer** by keyword scan (worth a look in the research stage): Taurus Security and Possessiveness; Cancer Belonging, Protection and Abandonment; Leo Play; Scorpio Death and Crisis; Capricorn Order. Aquarius Nonconformity has one only through the Mak Yong repertoire.
- **Repetitive:** the Aries and Taurus Held lines (formula, see above). No copied lines remain anywhere.

## Depth: do the sheets exploit the nation?
Mostly yes, given how small and thinly documented the nation is.
- **Scripts:** all 130 sheets give Jawi and Thai-script terms; 98 also give Chinese script.
- **Pre-modern pointers:** the *pondok* appears in 93 sheets, and the Patani *ulama* (Daud al-Fatani, Ahmad al-Fatani and others) in 51. The *Hikayat Patani* is named in 15, the sultanate's queens in 13, and Langkasuka or Yarang in 10. The sultanate and the queens are underused for a culture with that history.
- **Communities:** Buddhist Thai residents appear in 125 sheets, Chinese of the towns in 130, Maniq or Kensiw in 121 (Virgo 7 of 10, the lowest), Urak Lawoi in 107, and Thai-speaking Muslims in 54. Sam-Sam appear in 51 sheets but thin out late (1 sheet each in Sagittarius and Pisces). Christians appear in 2 sheets only.
- **Regions:** Yala 127, Narathiwat 112, Betong 102, Satun 94 (thinner in Virgo, Aquarius and Pisces), Songkhla's Malay districts 77, and Sungai Kolok 47.
- **Comparisons:** Kelantan appears in 121 sheets, always as comparison or as a shared cross-border tradition (Mak Yong, *main teri*, cross-border *nikah*), never as Patani's core. Diaspora (Mecca, Malaysia) stays as comparison.
- **Data flags** often say "thin": many concepts reach the culture only through Thai theses and a few ethnographies. The sheets say so and give queries; no padding with generic Malay or Thai material was found in the spot checks.
- **Not done:** the run agent did not read every sheet in full. Accuracy of the named works is unverified by design.
