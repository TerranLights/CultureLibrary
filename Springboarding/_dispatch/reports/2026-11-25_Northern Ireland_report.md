# Northern Ireland: springboard run report (2026-11-25)

Run agent for Northern Ireland, Wednesday wave 1. **Wall clock:** 05:05 to 10:26 MST. **Result:** 130/130 sheets done (`springboard_status.py`), whole-nation QA (`springboard_qa.py`) 0 problems. One sub-agent per sign (12 in all), **0 relaunches**, 20 run-agent smallest edits (listed below).

**Total sub-agent tokens:** 3,138,977 (12 sign agents; the run agent's own use is not included).

## Per sign

| # | Sign | Sheets | Words avg / max / min (`wc -w`) | Pointers | Sub-agent tokens | Minutes | Run-agent edits |
|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,202 / 1,284 / 1,123 | 14-15 | 205,223 | 17.7 | 1 |
| 2 | Taurus | 11 | 1,237 / 1,293 / 1,149 | 13-15 | 224,680 | 15.3 | 0 |
| 3 | Gemini | 10 | 1,204 / 1,244 / 1,135 | 13-15 | 210,184 | 18.0 | 1 |
| 4 | Cancer | 10 | 1,243 / 1,284 / 1,194 | 13-14 | 231,408 | 15.0 | 0 |
| 5 | Leo | 13 | 1,254 / 1,299 / 1,186 | 13-14 | 266,597 | 21.3 | 13 |
| 6 | Virgo | 10 | 1,191 / 1,296 / 1,110 | 12-14 | 256,653 | 22.4 | 2 |
| 7 | Libra | 11 | 1,240 / 1,283 / 1,181 | 12-15 | 295,009 | 28.7 | 0 |
| 8 | Scorpio | 11 | 1,248 / 1,297 / 1,189 | 12-14 | 324,629 | 26.7 | 0 |
| 9 | Sagittarius | 11 | 1,236 / 1,292 / 1,156 | 13-14 | 278,862 | 21.6 | 3 |
| 10 | Capricorn | 10 | 1,240 / 1,296 / 1,180 | 12-13 | 314,711 | 28.6 | 0 |
| 11 | Aquarius | 10 | 1,240 / 1,287 / 1,202 | 12-13 | 264,355 | 35.4 | 0 |
| 12 | Pisces | 12 | 1,251 / 1,288 / 1,177 | 13-15 | 266,666 | 56.6* | 0 |
| | **Nation** | **130** | **1,233 / 1,299 / 1,110** | **12-15** | **3,138,977** | | **20** |

\*Pisces' wall clock includes the sub-agent's own end checks after its last sheet. Pointer counts are table rows in section 2: 17 sheets at 12, 44 at 13, 51 at 14, 18 at 15. None is over 1,300 words; the longest are Leo Domain (1,299, after the run agent's edit), Scorpio Death (1,297), Virgo and Capricorn Domain (1,296).

## Rule breaks and fixes (all by smallest edit; no relaunch was needed)

- **Leo, all 13 sheets:** every sheet carried the same lumped "Who to compare" label naming all ten newer communities in one bullet. Each label was cut to the communities apt to that sheet's own check (Creativity's check also gained three craft terms). From Virgo on, the prompts carried a line against the lumped bullet, and it did not recur.
- **Sagittarius Travel and Honesty:** two newer-community bullets near-copied each other and labeled communities by job ("nurses", "meat-plant workers") with no concept check. Both were rewritten as what to check. From Capricorn on, the prompts carried a line against job labels.
- **Held lines that described the held item:** Gemini Mediation (described the set-aside go-between's role) and Sagittarius Meaning ("South Asian-related material") were cut to the category wording.
- **Near copies:** Aries Domain's Held line (against Initiative's), Virgo Criticism's clergy bullet (against Discernment's) and Virgo Domain's Lands line (against Leo's) were reworded.
- **Other:** Taurus to Pisces held their law content to pointers to Libra or Capricorn outside those signs; Libra kept to the letter and Capricorn to the spirit. There was no 'universals' framing, no Hermes, and none of the scan's banned words for almanacs.

## Repeat check across the nation (run agent's own)

- **0 exact repeats** of any line, table row, "Who to compare" bullet or Flags line across all 130 sheets (the template's fixed lines aside).
- **0 exact repeats against the United Kingdom's sheets.**
- **17 near matches remain, all among the 7 category-only South Asian Held lines** (Aries Domain and Identity, Gemini Mediation, Cancer Care, Leo Domain and Joy, Libra Reciprocity). The prescribed category wording makes these near matches unavoidable. Sagittarius Domain, Meaning and Education and Pisces Spirituality hold the same category in longer lines that differ enough not to match.

## South Asian rule, Buddhism, false positives

- **South Asian category held on 11 sheets,** category only: Aries Domain, Identity and Initiative; Gemini Mediation; Cancer Care; Leo Domain and Joy; Libra Reciprocity; Sagittarius Domain, Meaning and Education; Pisces Spirituality. No South Asian scholar, work, community, language or religion is named anywhere (the run agent's name scan over all 130 sheets).
- **Buddhism held as a category on 4 sheets,** naming no community, temple or text: Sagittarius Domain, Capricorn Discipline, Pisces Dissolution and Spirituality. Dissolution's and Discipline's lines say "meditation groups" and "meditation" as the kind of pointer. The author may want those cut to the bare category.
- **False positives:** "East Asian" (Libra Projection, on COVID-era incidents against Chinese residents) matched the run agent's own wider name pattern, not the QA scan. It is kept.

## Thin, repetitive or generic sheets

- **Generic before the fix:** Leo's lumped newer-community bullet (fixed). Cancer's empty Held lines followed one formula ("X sources were weighed against the standing rules; nothing set aside"), worded differently on each sheet. They were left as written but are the most formulaic Flags lines of the run. From Leo on, the Held lines name what was actually weighed (privacy, no Northern Ireland breakdown, outsider framing, and so on).
- **Lower pointer counts, still in range:** 17 sheets have 12 pointers, mostly late (Scorpio Purging, Trust, Revenge, Secrecy, Power and Crisis; Capricorn Ambition, Hierarchy, Merit, Law and Order; Aquarius Domain, Idealism, Nonconformity and Hope; Virgo Discernment; Libra Projection).
- **Narrowest spread of groups and regions:** Aries Recklessness (5 groups, 5 regions), Scorpio Crisis (6, 4), Aries Courage, Scorpio Revenge, Aquarius Reform (6, 5). None is thin on sources.

## Depth: do the sheets use the nation's depth?

Mostly yes.
- **Pre-modern pointers on all 130 sheets.** Examples: the *Annals of Ulster*, the *Táin*, the Brehon texts and Kelly's *Early Irish Farming*, *Ceart Uí Néill*, the Ó Caiside physicians of Fermanagh, the Plantation records, the 1641 Depositions, kirk-session minutes, Bunting and the United Irishmen.
- **Languages on every sheet:** Ulster Scots and Irish terms.
- **Groups, by number of sheets naming them:** Polish and Lithuanian 130; Travellers (Mincéirí) 121; Hong Kong Chinese 126; Syrian and Muslim communities 123; Portuguese and East Timorese 115; Filipino 81; Roma 65; Belfast's Jewish community 43; people who are neither (the 'others') only about 17. That last is the clearest gap for the research stage.
- **Regions, by number of sheets naming them:** Belfast 130; Derry / Londonderry 122; Tyrone and the Sperrins 116; Fermanagh 116; south Armagh 110; the Glens, the Causeway Coast and Rathlin, the Ards and Strangford, the Mournes and south Down, and the Lough Neagh shore 73 to 86 each.
- **Averages:** about 8 groups and 8 regions per sheet.
- **Contested names:** given in both forms (Derry / Londonderry, the Good Friday (Belfast) Agreement) and framed as accounts.
- **Sample read** (Aquarius Community): early Irish *comar*, session minute books, Harris's *Prejudice and Tolerance in Ulster*, *December Bride*, Corrymeela, the Housing Executive's shared-neighbourhood schemes, the 2017 North West floods, Rathlin's community plans, a Traveller education group and STEP Dungannon. That is varied, specific and spread across the six counties.

## Judgment calls for the author

1. **Lands:** no `00 - Scope.md`. Each Domain sheet notes once that the lands are still to be settled. Every sheet writes for the six counties, and the Republic (Donegal, Cavan and Monaghan included) is comparison only. No unit list was added.
2. **The two Buddhism Held lines that name the kind of practice ("meditation"):** keep them, or cut them to the bare category?
3. **The prescribed South Asian category wording** leaves near-identical Held lines on 7 sheets. Accept this as the rule's own form, or vary it further?
4. **The 'others'** (people who are neither unionist nor nationalist, Protestant nor Catholic) appear on few sheets. You may want them raised as a candidate unit at Stage 0.
5. **Diaspora** (Ulster Scots and Irish in Appalachia, North America and Australia) is kept to comparison only, as are the United Kingdom and the Republic of Ireland.
