# México springboard run: report (2026-11-23)

**Result:** 130/130 sheets `STATUS: done 2026-11-23, not verified` (by `springboard_status.py "México"`). Whole-nation QA (`springboard_qa.py "México"`): **130 sheets scanned, 0 problems.** 12 sign agents (one per sign, in the background, one at a time), **0 relaunches**, 7 hand edits by the run agent (smallest edits, listed below). No usage-limit stop.

**Wall-clock:** run agent started 09:55; first sub-agent launched 09:58; last sub-agent finished about 13:19; checks and report done about 13:21 (about 3 h 26 min).
**Sub-agent tokens:** **2,775,497** (657 tool uses). The run agent's own tokens are not in this figure.

## Per-sign table
| # | Sign | Sheets | Relaunches | QA | Hand edits | Avg words | Longest | Shortest | Pointers (avg, range) | Sub-agent tokens | Tools | Minutes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 0 | 0 | 0 | 1,222 | 1,267 Self-assertion | 1,176 Anger | 15.0 (14-16) | 199,155 | 48 | 17.6 |
| 2 | Taurus | 11 | 0 | 0 | 1 | 1,214 | 1,298 Domain | 1,158 Stubbornness | 15.2 (14-16) | 196,957 | 43 | 12.1 |
| 3 | Gemini | 10 | 0 | 0 | 0 | 1,256 | 1,275 Learning | 1,219 Gossip | 14.4 (13-16) | 208,923 | 43 | 12.8 |
| 4 | Cancer | 10 | 0 | 0 | 0 | 1,265 | 1,290 Domain | 1,228 Nurture | 14.9 (14-15) | 237,305 | 46 | 15.3 |
| 5 | Leo | 13 | 0 | 0 | 0 | 1,254 | 1,293 Creativity | 1,203 Honor | 13.8 (13-14) | 296,146 | 79 | 21.6 |
| 6 | Virgo | 10 | 0 | 0 | 0 | 1,254 | 1,294 Service | 1,202 Perfectionism | 13.9 (13-14) | 214,252 | 44 | 15.3 |
| 7 | Libra | 11 | 0 | 0 | 0 | 1,265 | 1,286 Justice | 1,230 Balance | 14.6 (14-15) | 257,655 | 53 | 19.2 |
| 8 | Scorpio | 11 | 0 | 0 | 0 | 1,177 | 1,274 Death | 1,113 Secrecy | 14.5 (13-16) | 213,490 | 46 | 13.5 |
| 9 | Sagittarius | 11 | 0 | 0 | 0 | 1,249 | 1,275 Truth | 1,153 Education | 14.0 (13-15) | 213,709 | 53 | 14.0 |
| 10 | Capricorn | 10 | 0 | 0 | 0 | 1,175 | 1,295 Domain | 1,110 Merit | 13.3 (13-14) | 254,563 | 71 | 18.0 |
| 11 | Aquarius | 10 | 0 | 0 | 0 | 1,251 | 1,300 Nonconformity | 1,191 Detachment | 14.4 (13-15) | 220,793 | 51 | 14.2 |
| 12 | Pisces | 12 | 0 | 0 | 6 | 1,270 | 1,300 Boundary | 1,245 Surrender | 14.0 (13-15) | 262,549 | 80 | 19.7 |
| | **Total** | **130** | **0** | **0** | **7** | **1,238** | 1,300 | 1,110 | **14.3 (13-16)** | **2,775,497** | **657** | |

Words by `wc -w`: 102 sheets over 1,200, none over 1,300 (two at exactly 1,300: Aquarius Nonconformity, Pisces Boundary). Every sheet has 13 to 16 pointers.

## Rule breaks and fixes
- **QA flags:** none in any sign.
- **Run agent's own South Asian-name scan (after each sign and for the whole nation):** clean. Every hit was a false positive: the colonial *casta* paintings and labels and the Caste War of Yucatán ("caste"), Spanish *madrastra* ("madras"), "citizen" ("zen"), "sodalities" ("dalit"), Penelope Brown (my "brown's" pattern), and the published title of Las Casas's *Brevísima relación de la destrucción de las Indias* (kept as published). My scan was tightened after each.
- **No named South Asian scholar, writer, work, community or religion anywhere.** South Asian items appear only as categories, on 9 Held lines, each where a real pointer was set aside: Aries Domain, Virgo Service and Aquarius Equality (the South Asian-born figure behind the *china poblana* story, each from a different angle: costume lore, colonial service, colonial rank); Virgo Health, Sagittarius Meaning, Pisces Dissolution and Spirituality (South Asian-origin body and meditation disciplines at retreats and centers); Sagittarius Conviction (a South Asian leader's nonviolence writings cited by Mexican movements); Sagittarius Fundamentalism (high-control groups of South Asian origin). 
- **Buddhism (open question):** held as a category only, no community, temple or text named, on 6 sheets: Virgo Health, Sagittarius Domain, Aquarius Detachment, Pisces Compassion, Dissolution and Spirituality.
- **"Indian":** none outside a published title; the Cancer sub-agent named the Latorres' Kikapú ethnography by its authors and subject instead of its English title (which contains the word).
- **Law outside Libra and Capricorn:** none found by hand; every other sign points law to Libra and Capricorn (Scorpio's Held lines set aside five law items that way). Libra's Justice checked as the letter (Puga's *Cedulario*, the 2014 national criminal-procedure code, the *Semanario Judicial*, the Cherán ruling, Oaxaca's *sistemas normativos internos*); Capricorn's Law as the spirit ("obedezco pero no cumplo", *Ciudadanos imaginarios*, the 1916-17 debates, constitutional-culture surveys).
- **Universals, Hermes, banned divination words:** none.
- **Lands note:** once per Domain sheet, nowhere else; no unit list.
- **Hand edits (smallest):** (1) Taurus Domain: its comparison-only bullet was near-identical to Aries Domain's; given a possessions-specific reason. (2 to 7) Pisces: seven of its first queries, and one in Aquarius Domain, opened with the same formula ("Look up each table 1 term in Molina and a Mexicanism dictionary; ..."); those in Compassion, Dissolution, Boundary, Surrender, Intuition and Fear were rewritten to name each sheet's own terms; the two Domain sheets' versions (Aquarius, Pisces) were kept, as their second halves differ. STATUS lines untouched.
- **Process notes (no harm found):** the Aries, Leo and Aquarius sub-agents reworded comparison or Held lines after marking sheets done (Leo and Aquarius reset the STATUS to in progress first, as told from Taurus on); the Gemini sub-agent drafted all ten sheets before marking each done.

## Repeat check across the nation
- **Exact repeats:** 0 lines, table rows, compare bullets, Flags lines or first queries repeated between any two sheets.
- **Near repeats (same first 70 characters):** 16 pairs or triples, all openings with different reasons after them: group-label openings in compare bullets (for example "Afro-Mexican communities of the Costa Chica and Veracruz: check ..." in Aries Domain, Aries Identity and Gemini Duality; "Lebanese-Mexican, Jewish, Chinese-Mexican and Japanese-Mexican ..." in Aries, Taurus, Capricorn, Aquarius), and the comparison-only lines, which from Gemini on each carry their own concept reason.
- **Most-used pointer:** Frank Cancian, *Economics and Prestige in a Maya Community*, on 4 sheets (Aries Competition, Taurus Domain, Virgo Service, Pisces Self-sacrifice), each for a different question. No other named pointer is on more than 3 sheets.

## Thin, repetitive or generic sheets (by name)
- **Shortest and leanest:** Capricorn Merit (1,110 words), Scorpio Secrecy (1,113, 13 pointers), Scorpio Trust, Power and Crisis (1,136-1,137), Capricorn as a sign (13.3 pointers on average, the lowest).
- **Templated:** Pisces, the most formulaic sign: three "Smaller communities: check Jewish, Lebanese-Mexican and Chinese-Mexican ..." bullets (Self-sacrifice, Escapism, Intuition), three comparison-only lines with the same opening (Empathy, Self-sacrifice, Fear), two Guerrero bullets and two Oaxaca bullets with shared openings. The reasons differ, but the lists read as a pattern.
- **Terse compare bullets:** Aries (several bullets of a single short clause, for example the Afro-Mexican and internal-migrant bullets of the Domain and Identity sheets).
- None reads as research (no findings, no statistics); none is generic in its sources.

## Pointers and depth
- **Pointers per sheet:** 13 to 16, average 14.3.
- **Does it exploit the nation's depth? Largely yes.** Every sign has pre-modern pointers (Florentine Codex books, *Huehuetlahtolli*, *Relación de Michoacán*, *Codex Mendoza*, Mixtec codices and *lienzos*, *Cantares mexicanos*, Chimalpahin, Molina, the *Testaments of Culhuacan*, *Relaciones geográficas*, Inquisition files, Sor Juana, the *Lienzo de Tlaxcala*), Indigenous-language terms in their own names, and INEGI and other national survey series. Spread by number of sheets naming each: Tsotsil 98, Ñuu Savi 87, Rarámuri 80, Tseltal 76, Purépecha 71, Triqui 56, Ayuuk 53, Wixárika 47, Chinantec 40, Hñähñu 38, Me'phaa 31, Totonac 25, Mazatec 23; Afro-Mexican 104, Mennonite 102, Kikapú 89, Jewish 65, Lebanese 61, Central American migrants 50, Evangelical 46, Chinese- and Japanese-Mexican 35 each, Spanish Republican exiles 25; Costa Chica 94, Los Altos 57, Isthmus 46, Sinaloa 38, Huasteca 36, Sierra Norte 36.
- **Thinner coverage:** Zoque (2 sheets), Náayeri (Cora) 10, Mazahua 11, Tojolabal 11, Ch'ol 17, Ñomndaa (Amuzgo) 16, O'dam (Tepehuan) 16; Popoloca, Chocholtec and Yoreme/Guarijío none; Tamaulipas 13, Querétaro 15, Colima 2, Aguascalientes 3. The Kikapú appear often but mostly as "thin, start with ..." notes, which is honest.

## Judgment calls for the author
1. **Lands:** no settled lands; the sheets are written for the core of pre-war Mexico, with the lands note once per Domain sheet. Yucatán (the Peninsula, Petén, the Yucatec Maya), Sonora (Yoeme, Comcaac, O'odham), Cascadia's Bajas (Tijuana, Mexicali, Kumiai, Cucapá, Paipai, Kiliwa), the CSA's Tejanos and the US diaspora appear only on comparison-only lines; Campeche and Quintana Roo only there.
2. **Edges the sub-agents treated as core, to confirm:** **Tabasco** (14 sheets, as core México: Garrido Canabal's anticlericalism, Greene's novel); Chiapas's Maya peoples including the Lacandon (Hach Winik) (core, as the Peninsula is Yucatán's); Chihuahua and northern Sinaloa as core, while their Yoreme (Mayo) and Guarijío neighbors of the Sonoran side appear nowhere. Where México meets Sonora in Sinaloa and Chihuahua, and Yucatán in Tabasco and southern Campeche, is for you.
3. **The *china poblana* figure** (a South Asian-born woman in colonial Puebla) was held as a category on three sheets under the strict rule; the costume itself is named freely. Confirm that this is how you want her handled.
4. **Buddhism:** held as a category on 6 sheets (listed above), never named.
5. **South Asian-origin practices and movements in México** (meditation and body disciplines, high-control groups, a nonviolence leader's writings) held as categories on 6 sheets.
6. **Law items held in Scorpio** (advance directives, the *Ley Olimpia*, transparency and data-protection laws, trust in courts, no re-election) are pointed to Libra and Capricorn rather than given there; Capricorn's Law names the 2020 amnesty law as a statement of purpose (spirit), not its text.
7. **Mediation (Gemini)** keeps dispute-settlement ethnographies (Nader, Collier) and the federal labor-conciliation body as social pointers; statutes are pointed to Libra.

## Files
- Sheets: `Targets/Latin America/México/Springboards/01 - Aries/` to `12 - Pisces/`.
- Run log lines: `_dispatch/SPRINGBOARD_PROGRESS.md` (twelve sign lines, one timing correction, one completion line; appended only).
