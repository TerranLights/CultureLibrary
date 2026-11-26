# Argentina springboards: run report (2026-11-25)

Run agent for Argentina (target "Argentina (without Patagonia)"), deeper brief, one sub-agent per sign, all twelve signs in order. Launched into Chile's slot in wave 2.

**Result:** 130/130 sheets `STATUS: done 2026-11-25, not verified` (by `springboard_status.py`). Whole-nation QA: 2 flags, both false positives (published titles containing "Indian", kept in quotation marks). 12 sign agents, 0 relaunches, 18 run-agent smallest edits. Own repeat check across the nation, against Chile's 130 sheets and against the 128 Araucanía-Patagonia sheets on disk at the end: 0 exact repeats and 0 near matches at 0.85 after the edits.

**Tokens and time:** sub-agents 3,010,957 tokens, 816 tool calls. Wall clock 09:39 (first launch) to 13:24 (last sheet checked); report 13:27.

## Per sign

| # | Sign | Sheets | Relaunches | QA flags | Run-agent edits | Avg words | Longest | Shortest | Pointers | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 0 | 1 (false positive) | 1 | 1,193 | 1,273 Identity | 1,112 Independence | 14-16 (161) | 179,381 | 09:39-09:54 |
| 2 | Taurus | 11 | 0 | 1 (false positive) | 5 | 1,222 | 1,265 Ownership | 1,172 Stubbornness | 14-16 (165) | 214,691 | 09:57-10:10 |
| 3 | Gemini | 10 | 0 | 0 | 2 | 1,191 | 1,292 Domain | 1,114 Gossip | 14-15 (142) | 198,225 | 10:13-10:26 |
| 4 | Cancer | 10 | 0 | 0 | 2 | 1,223 | 1,262 Domain | 1,144 Nurture | 14-15 (145) | 234,283 | 10:28-10:43 |
| 5 | Leo | 13 | 0 | 0 | 0 | 1,273 | 1,299 Honor | 1,193 Domain | 14-16 (191) | 244,552 | 10:45-11:00 |
| 6 | Virgo | 10 | 0 | 0 | 0 | 1,180 | 1,230 Service | 1,112 Perfectionism | 14-15 (143) | 239,773 | 11:02-11:16 |
| 7 | Libra | 11 | 0 | 0 | 2 | 1,239 | 1,261 Projection | 1,193 Domain | 13-14 (147) | 285,213 | 11:18-11:37 |
| 8 | Scorpio | 11 | 0 | 0 | 0 | 1,230 | 1,272 Purging | 1,191 Power | 14-16 (164) | 262,690 | 11:40-11:58 |
| 9 | Sagittarius | 11 | 0 | 0 | 2 | 1,242 | 1,276 Domain | 1,171 Honesty | 12-14 (147) | 250,748 | 12:00-12:18 |
| 10 | Capricorn | 10 | 0 | 0 | 0 | 1,236 | 1,255 Duty | 1,191 Ambition | 13-14 (131) | 272,137 | 12:21-12:39 |
| 11 | Aquarius | 10 | 0 | 0 | 1 | 1,244 | 1,279 Reform | 1,171 Detachment | 13-15 (137) | 316,814 | 12:41-13:00 |
| 12 | Pisces | 12 | 0 | 0 | 3 | 1,229 | 1,252 Surrender | 1,201 Spirituality | 12-14 (160) | 312,450 | 13:03-13:24 |
| | **Nation** | **130** | **0** | **2** | **18** | **1,227** | 1,299 | 1,112 | 12-16 (1,833) | **3,010,957** | 09:39-13:24 |

Pointers per sheet: 12 on 3 sheets (Sagittarius Conviction and Honesty, Pisces Intuition), 13 on 29, 14 on 56, 15 on 36, 16 on 6. Average 14.1. Pointer counts drift down in the later signs (Capricorn to Pisces), as they did for Chile, while length stays about the same.

## Rule breaks and fixes (all smallest edits by the run agent)
- **Near-copied search-term rows (10):** common words whose note matched another sheet: Taurus Values (*no tiene precio*, vs Araucanía-Patagonia), Security (*mutuo soccorso*, vs Aries Independence), Stability (*llaqta*, vs Chile Cancer Home), Possessiveness (*celos/celotipia*, vs Chile); Gemini Curiosity (*tapuy*, vs Learning), Gossip (*el qué dirán*, vs Chile); Cancer Belonging and Shelter (vs Chile); Libra Projection (*el burro hablando de orejas*, vs Chile); Sagittarius Meaning (*todo pasa por algo*, vs Chile); Pisces Intuition (*me da mala espina*, vs Chile). Each note made concept-specific. From Gemini on, the prompt asked for concept-specific notes on common words.
- **Copied "Who to compare" bullet (1):** Aquarius Domain's Corrientes-Misiones-Entre Ríos bullet (vs Capricorn Domain), reworded.
- **Lands note repeated and scope file named (1):** Taurus Domain; cut. The note stays once, in Aries Domain. Later prompts said so, and no later sheet repeats it.
- **Held lines describing a held item (5):** Aries Autonomy (the kind of practice), Libra Projection (no category given), Sagittarius Belief (the kind of group and its hill region), Pisces Dissolution (a Buddhist teaching described), Pisces Domain (a 'transcendence' pointer). All cut to the bare category. One Libra edit of mine was itself a near match with Aries Autonomy and was reworded again.
- **QA false positives (2, kept):** Wilbert and Simoneau's titles "Folk Literature of the Toba Indians" and "... of the Mataco Indians" (Aries Beginning), and Jules and Zunia Henry's "Doll Play of Pilagá Indian Children" (1944) (Taurus Possessiveness). Spanish published titles with *indios* are also kept as published: Mansilla's *Una excursión a los indios ranqueles* (Gemini Communication, Scorpio Betrayal), the *Confessionario para los curas de indios* (1585) (Sagittarius Honesty), and the colonial *pueblos de indios* of Córdoba (Pisces Dissolution).
- **Process:** the Leo sub-agent set all 13 STATUS lines in one pass at the end, not per sheet, and trimmed rows from drafts over 1,300 words (every sheet kept 14 to 16 pointers). Later prompts repeated the mark-each-sheet rule, and every later sign complied. The Scorpio sub-agent reported auto-mode safety-check timeouts during Rebirth that cleared on retry, with nothing lost.

## Standing rules
- **South Asian:** category held on 6 sheets (Aries Autonomy, Libra Projection, Sagittarius Domain and Belief, Pisces Domain and Spirituality), nothing named. My name scan found no South Asian scholar, writer, work, community or religion. Victoria and Silvina Ocampo appear (Gemini Siblings, Virgo Discernment, Pisces Fear), and nothing beyond them. Capricorn Ambition uses Argentine mobility studies and names no mobility atlas or dataset from the concept block.
- **Buddhism:** held as a category on 9 sheets (Aries Domain and Beginning, Cancer Domain, Sagittarius Domain, Faith and Belief, Aquarius Detachment, Pisces Dissolution and Spirituality), nothing named.
- **Law:** Libra kept to the letter (statutes, rulings, courts as written), and Capricorn to the spirit (custom, discretion, compliance, legal culture). Elsewhere law is pointed to Libra or Capricorn.
- No universals, no Hermes, no zodiac words, no URLs, no 'Indian' outside published titles.
- **Contested ground:** the dictatorship and the trials, CORREPI's count, Montoneros texts, Nisman, Peronism, the Malvinas, AMIA, Napalpí and Rincón Bomba, and the Afro-Argentine 'disappearance' account are framed as accounts throughout.

## Thin, repetitive or generic sheets
- **Formulaic Held lines:** Virgo's ten Held lines share one formula with a different list each time ("nothing set aside; the X, Y and Z pointers weighed for ... raised no standing-rule issue"). There is no near match at 0.85 (0.81-0.82 between some pairs), so I kept them. Gemini's and Leo's are close to the same formula. From Libra on, each Held line names its own closest call.
- **Common note phrases on search-term rows:** in the 0.80-0.85 band, there are Quechua rows with the same note ("Kolla and Bolivian communities *check*") on different words (Gemini, Leo, Sagittarius Domain), and Yiddish rows noted "community press" (Aries). These are different terms, not copies, but a little generic.
- **Thinnest by pointer count:** Sagittarius Conviction and Honesty and Pisces Intuition, with 12 each. Capricorn is the lowest sign (13 on nine sheets). None reads as padded or generic on spot-checks (Aries Anger and Courage, Leo Humiliation and Pride, Libra Justice, Capricorn Law).

## Does the run use the nation's depth?
Largely yes. The pre-modern pointers recur in varied form: Schmidl, Lozano, Dobrizhoffer, the Jesuit Chaco and Misiones records, the 1583 relation, the Third Council of Lima confessionary, the colonial *pueblos de indios* of Córdoba, petitions of the 1820s, and Tau Anzoátegui on colonial legal custom. Interior regions appear on every sheet: Santiago del Estero's Quichua, Salta and Jujuy, Cuyo, the Litoral, Misiones, Chaco and Formosa, and La Pampa. The Qom, Wichí, Moqoit, Pilagá, Mbyá, Kolla, Diaguita and Huarpe appear by their own names, with Napalpí and Rincón Bomba as contested ground. So do Afro-Argentine and Cape Verdean, Jewish (Once and the Entre Ríos colonies), Syrian-Lebanese, Armenian, Ukrainian, Polish, Volga German, Mennonite, Okinawan, Korean, Chinese, Bolivian, Paraguayan and Peruvian pointers. The weakest coverage is of the smaller groups' own-language sources (Wichí, Pilagá and Moqoit terms, and Plautdietsch). Sheets mark these as thin rather than padding them.

## Judgment calls for the author
1. **Lands:** no scope file and no settled lands. The sheets are written for Argentina north of Patagonia, with Patagonia and the Mapuche lands as comparison only (Araucanía-Patagonia's row). Where the line runs (La Pampa, southern Buenos Aires province, southern Mendoza) is for you. La Pampa (Ranquel pointers, the Mennonites) is treated as core here. The Falklands / Malvinas are comparison only.
2. **Buddhism** is held on 9 sheets, and the South Asian category on 6: rulings pending.
3. **Living or recent named people in sensitive rows:** a convicted dictatorship officer (Scorpio Betrayal, through court and relatives' records only), Nisman polls (Sagittarius Truth), and Meinvielle (Sagittarius Fundamentalism, studies about him rather than his writings). Please confirm the handling.
4. **Sensitive "Who to compare" items to confirm:** Leo Humiliation's Jewish-community bullet on the trafficking era, as recorded by the community; Pisces Escapism's fernet-in-Córdoba row, kept only as a claim to test; Pisces Crime's rustling row, where old press linked rustling to Native peoples.
5. **Published titles containing "Indian" / *indios*:** kept in quotation marks or italics as published (listed above). The style question is open.
