# Vietnam springboards: run report (2026-11-21, wave 2)

**Result:** all 130 sheets are marked `STATUS: done 2026-11-21, not verified`. The run used 12 sign agents and 1 targeted relaunch (Capricorn). The whole-nation QA (`springboard_qa.py Vietnam`) scanned 130 sheets and found 0 problems. No pointer has been checked; the sheets are unverified.

**Inputs:** the deeper brief (accuracy and depth first), with the operational lessons added to every sub-agent prompt:
- no zodiac, astrolog* or horoscope words;
- the lands note once, in the Domain sheet;
- the no-reuse rule also covers the compare bullets (from Aquarius on, also: the overseas-Vietnamese bullet never a bare "comparison only", and a compare bullet makes no historical claim);
- the concept stated neutrally;
- Hermes_research never opened;
- diaspora pointers for comparison only;
- temporary files only in the nation's own scratchpad `tmp/`.

Two nation-specific notes were added, neither changes the brief:
- **Native script:** Quốc ngữ with full diacritics, chữ Hán / chữ Nôm where sure, and minority-language terms and scripts where sure.
- **South Asian rule:** the Cham and Khmer Krom peoples and their own-language materials are in scope, but no Sanskrit- or Pali-language text or South Asian scripture is named as a pointer. Such a pointer goes on the held line as a category, without naming the language.

From Taurus on, the prompt also said the done line is the very last write.

**Lands:** the tracker header lists no settled lands ("Territory: to be settled by the author in Stage 0"; no `00 - Scope.md`). The sheets follow the brief's missing-scope rule: they are written for Vietnam's core lands, and no unit list was added. The note that the lands are still to be settled appears in all 12 Domain sheets and in no concept sheet. Nothing came from Hermes_research. The Taurus agent noted that it used province names from before the 2025 province mergers. That is worth keeping in mind when the author settles the lands.

## Per sign
| # | Sign | Sheets | Agents | Relaunches | QA problems | Avg words | Longest | Pointers per sheet | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1 | 0 | 0 | 1,201 | 1,260 (Identity) | 14-15 | 171,542 | 08:03-08:17 |
| 2 | Taurus | 11/11 | 1 | 0 | 0 | 1,222 | 1,279 (Possession) | 13-16 | 218,790 | 08:18-08:35 |
| 3 | Gemini | 10/10 | 1 | 0 | 0 | 1,143 | 1,180 (Domain) | 14-16 | 192,221 | 08:35-08:48 |
| 4 | Cancer | 10/10 | 1 | 0 | 0 | 1,235 | 1,285 (Home) | 14-16 | 200,148 | 08:48-09:02 |
| 5 | Leo | 13/13 | 1 | 0 | 0 | 1,176 | 1,240 (Recognition) | 14-15 | 239,828 | 09:02-09:24 |
| 6 | Virgo | 10/10 | 1 | 0 | 0 | 1,177 | 1,286 (Domain) | 14-16 | 199,900 | 09:24-09:38 |
| 7 | Libra | 11/11 | 1 | 0 | 0 | 1,270 | 1,293 (Partnership) | 14-15 | 239,628 | 09:38-09:57 |
| 8 | Scorpio | 11/11 | 1 | 0 | 0 | 1,242 | 1,299 (Death) | 14-16 | 212,784 | 09:57-10:13 |
| 9 | Sagittarius | 11/11 | 1 | 0 | 0 | 1,215 | 1,241 (Faith) | 15-16 | about 210,300 (estimated) | 10:13-10:29 |
| 10 | Capricorn | 10/10 | 1 | 1 (targeted) | 0 | 1,210 | 1,288 (Domain) | 14-16 | 201,205 (incl. fix turn) | 11:43-11:59 |
| 11 | Aquarius | 10/10 | 1 | 0 | 0 | 1,228 | 1,286 (Equality) | 14-16 | 217,424 | 11:58-12:13 |
| 12 | Pisces | 12/12 | 1 | 0 | 0 | 1,239 | 1,279 (Compassion) | 15-16 | 226,513 | 12:13-12:31 |

Word counts are before the final hand edits. Those edits added 13 to 16 words to four sheets; Virgo's Domain is now 1,299.

## Tokens and wall-clock
- **Sub-agent tokens: about 2,530,300 in all.** That is the sum of 12 sign agents, with Capricorn's fix turn included in its 201,205. Eleven figures come from the harness. Sagittarius's agent was stopped by the 5-hour usage limit after its last sheet was already marked done, so the harness reported no figure. Its 210,287 is my estimate from that agent's transcript, read the way the reported figures are counted (it reproduces Aries's 171,542 to within 0.3%). The 11 reported figures alone come to 2,319,983. That is about 19,500 tokens per sheet, a little above Qin (2.32M) and Jin (2.26M). The run agent's own tokens are not counted here; the main session adds them.
- **Wall-clock:** started 08:02 MST and ended about 12:35 (report written). **Interruption: about 10:35 to 11:43**, when the 5-hour usage limit stopped the run. No sheet was lost or redone: Sagittarius was complete at 10:29, and the run resumed with Capricorn. Active time was about 3 h 25 min. Signs took 13 to 21 minutes each.
- **Words:** 157,781 in all by `wc -w`, markup included. The average is 1,214, and sheets run from 1,061 (Gemini Duality) to 1,299 (Scorpio Death, Virgo Domain). 81 sheets are over the brief's "up to about 1,200"; none is over the scan's 1,300. All 11 Libra sheets sit between 1,245 and 1,293, which suggests that agent wrote up to the line. Per lesson 4, no length instruction was added.

## Rule breaks and fixes
1. **QA: 0 problems in every sign and in the whole nation.** No zodiac words, no "Indian", no "sikh"-pattern hit, no URL and no finding phrasing.
2. **Capricorn, compare bullets (found by my own check, not the QA scan):** sheets 01 to 09 all carried the same bare bullet "Overseas Vietnamese: comparison only.", which breaks lesson 6. The agent also reported a Mekong Delta compare bullet in 01 Authority that stated a historical claim. I resumed the same agent with the problem. It rewrote only those ten bullets, setting each sheet to in progress, editing it, then marking it done as the last write. Recheck: clean.
3. **Cross-sign repeats (found by the whole-nation check), fixed by the smallest hand edits:**
   - The same bare overseas bullet appeared in the Leo, Virgo and Capricorn Domain sheets. Each now gives a domain-specific reason.
   - One search-term row (riêng tư; đời tư) was identical in Scorpio 08 Secrecy and Pisces 05 Boundary. The Boundary row's Notes cell was filled in.
   - After the fixes, no line over 25 characters (outside the template's fixed lines) repeats anywhere in the nation, and no compare bullet is copied.
4. **Checkpoint order (process note, final state clean):** the Aries agent went back to sheets 00 to 09 after marking them done, to rewrite a copied overseas bullet. So for those ten sheets the done line was not the very last write. The final files are correct. From Taurus on, the prompt said the done line comes last, and no other agent broke the order.
5. **Held for review:** 21 sheets carry a held line, all category-only. Examples are classical-language scriptures, liturgy and inscriptions of South Asian origin in Khmer Krom and Cham religious life, the scriptural story behind Vu Lan, and South Asian-heritage communities. The other 109 sheets read "none". No South Asian language, work or scholar is named anywhere.
6. **For the author's eye, not a break:** Pisces 10 Crime names some court and police material: the Năm Cam trial, a wrongful-conviction case and the anti-corruption trials. These are framed as crime coverage, not law research, but they sit near the Libra and Capricorn line.

## Thin, repetitive or generic sheets (by name)
- **Fewest pointers:** Taurus 09 Stubbornness has 13, the only sheet under 14. The nation averages 15.1 pointers (1,960 rows, of which 1,684 have distinct first cells).
- **Shortest:** Gemini 06 Duality (1,061), Leo 12 Joy (1,073), Leo 07 Humiliation (1,092) and Virgo 05 Discernment (1,106). All are still above the brief's 1,000 aim.
- **Pre-modern coverage:** a rough scan finds no dated pre-1900 or dynastic pointer in section 2 of 28 sheets. These include Aries Initiative, Gemini Connection and Siblings, Leo Joy, Scorpio Trust and Crisis, Aquarius Community, Friendship and Nonconformity, and Pisces Escapism, Spirituality, Surrender, Crime and Fear. The scan undercounts. A spot read found Gemini Gossip has *Tang thương ngẫu lục*, Aquarius Hope has *Truyền kỳ mạn lục* and the Trạng Trình prophecies, and Pisces Crime leans on folk verse and the Trạng Quỳnh tales. Several of these sheets are still modern-heavy and are the first candidates for added classical pointers.
- **Most reused works** (sheets naming them in a pointer's first cell):

| Work | Sheets |
|---|---|
| Phan Kế Bính, *Việt Nam phong tục* | 12 |
| Salemink, *The Ethnography of Vietnam's Central Highlanders* | 10 |
| Condominas, *Nous avons mangé la forêt* | 9 |
| Philip Taylor, *The Khmer Lands of Vietnam* | 8 |
| World Values Survey | 8 |
| Leshkowich, *Essential Trade* | 7 |
| Toan Ánh, *Nếp cũ* | 7 |

  The most-named outlets anywhere in a sheet are VnExpress (50 sheets) and Tuổi Trẻ (40). These are all standard and fitting, and none is a crutch on the scale of CNKI in the Sinian sheets.
- **Formulaic compare roster:** the wording and reasons differ in every bullet, but the roster is close to fixed. Counts out of 130 compare sections:

| Group | Sheets |
|---|---|
| Khmer Krom | 125 |
| Cham | 113 |
| Hmong | 112 |
| Hoa | 95 |
| Ê Đê | 92 |
| Jarai | 87 |
| overseas Vietnamese | 78 |
| Mekong Delta | 75 |
| Dao | 64 |
| Thái | 60 |
| Bahnar | 58 |
| Tày | 52 |
| Mường | 35 |
| Nùng | 34 |

  Of Vietnam's many smaller peoples, few appear: Mnông in 24 to 28 sheets, Xơ Đăng in 16, Raglai and Hà Nhì in 5 each, Bru-Vân Kiều and Cơ Tu in 3, Chu Ru and Lô Lô in 2, and Brâu, Rơ Măm, Ơ Đu and Pu Péo in 1 each. Protestant highland communities appear in only 7 sheets.

## Do the sheets exploit the nation's depth?
Mostly yes.
- **Classical and Hán-Nôm depth:** chữ Hán forms appear in 129 of 130 sheets; only Libra 10 Projection lacks them. The pre-modern pointers reach the classical canon, including:
  - *Đại Việt sử ký toàn thư*, *Lĩnh Nam chích quái* and *Truyền kỳ mạn lục*;
  - Nguyễn Trãi, Lê Quý Đôn and Hải Thượng Lãn Ông;
  - *Truyện Kiều*;
  - the Hán-Nôm Institute's holdings.
- **Colonial-era ethnography and the modern literary canon:** Phan Kế Bính, Toan Ánh, Nam Cao, Vũ Trọng Phụng and Bảo Ninh, set beside Western and Vietnamese scholarship. That scholarship includes Malarney, Kwon, Taylor, Endres, Salemink, Condominas, Hue-Tam Ho Tai and Ngô Đức Thịnh.
- **Datasets:** VHLSS, PAPI, the census, the World Values Survey and the Asian Barometer.
- **Weak spot, minority scripts:** Khmer script appears in 108 sheets. Cham (Akhar Thrah) and Tai Viet (Thái) script appear in **none**. Cham, Thái, Tày-Nùng and highland terms are given only in romanization. The agents followed the "only when sure" rule, so this is caution, not error, but it is the main gap in native-script depth.
- **Other gaps:** the northern uplands beyond the Hmong, Dao, Tày and Thái, and the smaller Central Highlands peoples, are thin. Regional Kinh variation (Red River, Nghệ-Tĩnh, Huế, Mekong) is covered steadily.

## Files
- Sheets: `Targets/Asia/Mainland Southeast Asia/Vietnam/Springboards/01 - Aries/` to `12 - Pisces/`.
- Run log lines were appended to `_dispatch/SPRINGBOARD_PROGRESS.md` only with `>>`: one per sign plus a completion line. The file's first line was not touched.
