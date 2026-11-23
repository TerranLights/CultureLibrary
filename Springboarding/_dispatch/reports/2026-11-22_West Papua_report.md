# West Papua springboard run: report (2026-11-22)

**Run agent:** one per nation (deeper brief, one sub-agent per sign, all lessons added to the sub-agent prompts). **Folder:** `Targets/Asia/Maritime Southeast Asia/West Papua/Springboards/`. **Lands:** none settled (no `00 - Scope.md`); the missing-scope rule was followed, with the lands note once per Domain sheet and no unit list added.

## Totals
- **Sheets:** 130 of 130, every one `STATUS: done 2026-11-22, not verified`.
- **Agents:** 13 (12 sign agents and 1 single-concept relaunch).
- **Whole-nation QA (`springboard_qa.py "West Papua"`):** 130 sheets scanned, 0 problems (after the one relaunch and the hand edits below).
- **Sub-agent tokens:** 2,865,760 (sign agents 2,800,156 and the relaunch 65,604). Run-agent tokens are not included; the main session adds them.
- **Wall clock:** first launch 12:31, last check 16:00 MST (about 3 h 29 min, with no usage-limit stop).
- **Words (`wc -w`):** nation average 1,225; range 1,106 (Leo, Joy) to 1,296 (Pisces, Domain); 91 of 130 over 1,200, none over 1,300.
- **Pointers per sheet ("Where to look first" rows):** 13 to 15 (25 sheets with 13, 94 with 14 and 11 with 15; average 13.9).

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA problems | Avg words | Longest | Pointers | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,165 | 1,261 (Domain) | 14-15 | 164,044 | 12:31-12:44 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,199 | 1,271 (Domain) | 13-14 | 212,924 | 12:44-13:00 |
| 3 | Gemini | 10 | 1 | 0 | 0 | 1,209 | 1,298 (Domain) | 13-15 | 182,032 | 13:00-13:12 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,230 | 1,285 (Home) | 13-14 | 226,358 | 13:12-13:26 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,177 | 1,265 (Domain) | 13-15 | 258,581 | 13:26-13:46 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,261 | 1,290 (Usefulness) | 13-14 | 240,047 | 13:46-14:03 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,277 | 1,291 (Partnership) | 13-14 | 230,023 | 14:04-14:19 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,218 | 1,295 (Domain) | 13-15 | 280,632 | 14:20-14:40 |
| 9 | Sagittarius | 11 | 2 | 1 | 1 (Domain 1,301 words) | 1,229 | 1,275 (Domain, after fix) | 14-15 | 205,736 + 65,604 | 14:41-14:56 |
| 10 | Capricorn | 10 | 1 | 0 | 0 | 1,238 | 1,276 (Domain, Law) | 13-14 | 237,029 | 14:57-15:13 |
| 11 | Aquarius | 10 | 1 | 0 | 0 | 1,252 | 1,287 (Equality) | 13-14 | 254,025 | 15:13-15:32 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,255 | 1,296 (Domain, after edit) | 14-15 | 308,725 | 15:33-15:59 |

(Word counts in the table are final, after the hand edits; the Run log lines give the counts at each sign's check.)

## Rule breaks and fixes
1. **Sagittarius, Domain: 1,301 words** (QA "long"). A single-concept relaunch tightened it to 1,273 words and kept all 14 pointers, every search term and the lands note. QA then showed 0 problems.
2. **Trait-stating "Who to compare" bullets (no-stereotype rule).** QA did not flag these; the run agent's own scan found them, and each was fixed by the smallest edit, rewording it as something to check:
   - Virgo, Usefulness: "settler-run trades … set many town skill standards" became "check whether settler-run trades … set town skill standards".
   - Aquarius, Group: "their *paguyuban* … form groups of their own" became "check their *paguyuban* and party branches as groups".
   - Aquarius, Nonconformity: "their own subcultures mix with Papuan ones" became "check where their youth scenes mix with Papuan ones".
   - Gemini, Siblings: "migrant settler families with their own customs" became "migrant settler families, recorded separately".
   - Pisces, Domain, Escapism, Spirituality and Intuition: "a present-day layer with its own healers / pastimes / shrines and prayer groups / dream books and seers" became "a present-day layer; check which …".
3. **Scope-file mentions.** Six Domain sheets (Taurus, Cancer, Leo, Virgo, Libra, Scorpio) said "there is no scope file for West Papua". The brief asks only that the unsettled lands be noted, so the clause was cut by the smallest edit and the lands sentence kept. The sub-agents for Capricorn to Pisces were told not to mention a scope file.
4. **False positives (kept as written):** "Dutch East India Company (VOC)" in Gemini, Information, is a published organization name, not a South Asian pointer. "Dumont d'Urville" in Cancer, Domain, matched only the run agent's own grep. The ship name *Astrolabe* in the same row does not match the QA's banned-word pattern.
5. **South Asian check by name (lesson 11):** clean in every sign. "Held for review" lines are "none" with a concept-specific reason, or category-only.
6. **Law outside Libra and Capricorn:** none found (statute grep on Scorpio, Sagittarius, Aquarius and Pisces, including Crime). Libra kept to the letter of the law; Capricorn's Law sheet was briefed for its spirit.
7. **Within-agent self-corrections (no problem left):** Leo's Domain sheet was briefly over 1,300 words and was trimmed by its own agent. Scorpio, Rebirth swapped a pointer repeated from an earlier sign. Pisces swapped one Domain pointer and one Surrender pointer for the same reason. In each case the STATUS line was rewritten last.

## Repeat check across the nation (the run agent's own)
- **Exact repeats** (lines of 30 or more characters, template lines excluded; table rows, "Who to compare" bullets and Flags lines included): **0** across all 130 sheets.
- **Near repeats** (the same first 12 words): two sources each appear in two rows with different reasons (Saltford's UN history in Aries, Independence and Sagittarius, Freedom; Zegwaard's Asmat headhunting article in Aries, Courage and Libra, Reciprocity). This is allowed.
- **Recurring sources:** no pointer is used more than twice in the whole nation (by the first 45 characters of the Pointer cell). Kluge's Papuan Malay grammar, Pospisil's Kapauku (Mee) works, Rutherford, Chao (Marind), Mansoben, Giay, Zöllner (Yali), Haenen (Moi), Held (Waropen), Forrest's 1770s voyage, Andaya's Maluku and Bromley's Dani grammar each recur, always with a new reason.
- **Formulaic, not copied:** all 12 Pisces "Who to compare" lists open their settler bullet with the same lead, "Migrant settler communities in the towns: a present-day layer; check …". Each bullet ends in a different, concept-specific check, but the lead is stock. Rewrite the leads if the author wants more variety.

## Thin, repetitive or generic sheets (by name)
- **Thinnest by pointer count (13 pointers, still within 12 to 16):** Taurus, Stubbornness; Gemini, Duality; Cancer, Abandonment; Leo, Dignity and Humiliation; Virgo, Service, Usefulness, Analysis, Discernment and Perfectionism; Libra, Balance, Diplomacy, Reciprocity, Indecision, Peace at any price and Projection; Scorpio, Trust, Secrecy and Crisis; Capricorn, Domain; Aquarius, Community, Idealism, Nonconformity, Detachment and Hope.
- **Thin by the culture's documentation:** the sub-agents say so rather than pad. In Scorpio, own-language terms for betrayal, owed deaths, cleansing after war and the hungry season are marked "not known to the scout". In Capricorn, the Hatam/Meyah forest-zone names (Order) and Biak *fararur* (Duty) are marked *check*. Abstract concepts (Libra, Indecision and Projection; Virgo, Perfectionism and Analysis; Aquarius, Detachment) lean on present-day Papuan Malay terms, theses and church material, because older ethnography does not name them.
- **Generic-material risk:** 13 sheets cite Melanesian comparative works (Worsley, Burridge, Godelier and Strathern, Narokobi, Harrison, Forsyth and Eves, Lini). Each is marked "comparison only"; none fills a core slot. Papua New Guinea appears only as comparison.
- **Lengths sit high in the range:** the brief aims for about 1,000 and allows up to about 1,200; 91 of 130 sheets run 1,200 to 1,296. Virgo, Libra, Aquarius and Pisces cluster at 1,250 to 1,296, close to the 1,300 flag.

## Does the run exploit the nation's depth?
Mostly yes, for a small and thinly documented culture-nation:
- **Internal regions, counted by sheets that name them (counts are sheets out of 130 that match the name, ignoring case, so they are approximate):** Raja Ampat about 128 sheets; Biak and Cenderawasih Bay about 128; Merauke 109; Asmat 111; Sentani and Jayapura 113; and the Bird's Head peoples (Maybrat 78, Moi 99, Arfak 40, Hatam 47, Sougb 25, Mbaham-Matta 40).
- **Peoples beyond the best-known few:** Muyu 55, Moni 57, Nduga 49, Korowai 28, Waropen 23, Kombai 13, Ma'ya 83, Kamoro 104, Amungme 42, Yali 88, Lani 116. Muslim Papuans of Fakfak, Kaimana and Raja Ampat are a recurring comparison.
- **Pre-modern pointers:** Koreri and Manarmakeri in 21 sheets, Tidore in 33, men's houses in 21, *honai* in 15, Seram in 9. Early voyage and mission records (Forrest, Duperrey and Dumont d'Urville plates, VOC and Dutch archives) are read critically.
- **Own-language terms:** Papuan Malay throughout, plus Dani, Lani, Mee, Biak, Sentani, Marind, Asmat and Bird's Head terms. Uncertain forms are marked *check* rather than guessed.
- **Gaps:** no own-script issue, since the languages are written in Latin script. The weakest coverage is the Mamberamo basin (6 sheets) and the Lakes Plains peoples (2), the Sarmi coast (3), the Kaimana interior (Mairasi, 3) and the southern Bird's Head (Bintuni 2, Irarutu 3, Sumuri 1). These appear rarely or only in lists. Customary council records are also thin as pointers: the Dewan Adat Papua appears in 6 sheets and the LMA in 3.

## For the author
- West Papua's lands are still to be settled at Stage 0. The sheets are written for western New Guinea with Biak, Yapen and Raja Ampat, noted once per Domain sheet.
- The settler-bullet edits and the scope-file edits were made by hand by the run agent (smallest edits). They are listed above, so they can be reverted if the author prefers.
