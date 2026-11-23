# Thailand: springboard run report (2026-11-22)

**Result:** 130 of 130 sheets done (12 signs, Aries to Pisces), one sub-agent per sign, 0 relaunches. The whole-nation QA scan (`springboard_qa.py Thailand`) found 0 problems in 130 sheets. The run agent's own nation-wide repeat check found no copied line, table row, Flags line or "Who to compare" bullet between sheets (details below).

- **Wall clock:** 08:36 (start) to 12:28 (end), about 3 h 52 min. No usage-limit stop.
- **Sub-agent tokens:** 2,771,294 in total (12 agents, 625 tool uses). That is above the 2.2 to 2.5M of earlier nations because the later signs re-read the earlier sheets to check for repeats (the Sagittarius agent alone used 284k).
- **Lands:** the tracker header lists no settled lands, and there is no `00 - Scope.md`. The missing-scope note appears once per sign, in the Domain sheet only, and no unit list was added.
- **Patani** (Pattani, Yala, Narathiwat) appears only as comparison in every sheet. The Southern Thai outside Patani (Satun, Songkhla, Nakhon Si Thammarat, Phuket, Krabi) are kept inside Thailand.

## Per-sign table
| # | Sign | Sheets | Relaunches | QA | Avg words | Longest | Pointers (range, avg) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 0 | 0 | 1,153 | 1,282 (Domain) | 15-16, 15.5 | 174,722 | 08:37-08:51 |
| 2 | Taurus | 11/11 | 0 | 0 | 1,193 | 1,284 | 15, 15.0 | 205,608 | 08:52-09:06 |
| 3 | Gemini | 10/10 | 0 | 0 | 1,213 | 1,268 (Domain) | 14-15, 14.7 | 191,590 | 09:06-09:19 |
| 4 | Cancer | 10/10 | 0 | 0 | 1,242 | 1,278 (Abandonment) | 14-15, 14.7 | 236,201 | 09:19-09:35 |
| 5 | Leo | 13/13 | 0 | 0 | 1,204 | 1,279 | 13-15, 14.5 | 271,236 | 09:35-09:56 |
| 6 | Virgo | 10/10 | 0 | 0 | 1,226 | 1,290 | 13-15, 14.3 | 219,636 | 09:57-10:16 |
| 7 | Libra | 11/11 | 0 | 0 | 1,201 | 1,257 | 14-16, 15.2 | 239,341 | 10:17-10:35 |
| 8 | Scorpio | 11/11 | 0 | 0 | 1,239 | 1,292 | 15-16, 15.1 | 265,699 | 10:36-10:59 |
| 9 | Sagittarius | 11/11 | 0 | 0 | 1,187 | 1,281 (Domain) | 14-15, 14.3 | 284,461 | 11:00-11:30 |
| 10 | Capricorn | 10/10 | 0 | 0 | 1,226 | 1,265 | 14, 14.0 | 233,497 | 11:30-11:48 |
| 11 | Aquarius | 10/10 | 0 | 0 | 1,226 | 1,271 | 14-15, 14.3 | 230,624 | 11:48-12:08 |
| 12 | Pisces | 12/12 | 0 | 0 | 1,224 | 1,281 | 14, 14.0 | 218,679 | 12:08-12:24 |
| | **Total** | **130/130** | **0** | **0** | **1,210** | **1,292** | **13-16, 14.6** | **2,771,294** | **08:36-12:28** |

- **Word counts** are by `wc -w`. 73 sheets run over 1,200 words and none over 1,300. The shortest is Aries Competition at 1,056.
- **Pointers** are the rows in "Where to look first". Two sheets have 13 (Leo Honor, Virgo Criticism), and all the rest have 14 to 16.

## Rule breaks and fixes
- **Aries, six bare Patani and diaspora bullets.** In Domain, Self-assertion, Identity, Initiative, Beginning and Recklessness, the "Who to compare" bullet said only "Patani (comparison only; separate culture-nation)", with no reason tied to the concept. I gave each a concept-specific reason by small hand edits and kept the status lines. From Taurus on, the prompt required a reason in these bullets, and every later sheet has one.
- **Sagittarius, a correction in mid-run.** My own prompt had placed Thai court Brahmin ritual on the held line, which was too cautious. I corrected the sub-agent while it was running: Thai court Brahmin ritual is the nation's own material, as Indonesia's Balinese Hinduism was kept for Indonesia. That covers the Devasathan, the Royal Ploughing Ceremony and the *phram* of Nakhon Si Thammarat and Phatthalung. The Sagittarius Domain sheet now names it as a pointer, and the prompt carried the clarification from Capricorn on.
- **South Asian rule.** 81 sheets have a category-only held line. These lines set aside classical-language scripture behind Thai sermons and monastic exams, the monastic code in its original language, and Islamic missionary and reformist movements founded in South Asia. They also set aside pilgrimage circuits to the Buddha's sites outside Southeast Asia, and the houses of worship and scholarship of South Asian-heritage communities. No language, scholar, community or work is named. Thailand's own Theravada and court heritage in Thai and regional languages was kept as the nation's material: *Traiphum Phra Ruang*, *Ramakien*, Mahachat and jataka-derived Thai literature, Lanna palm-leaf manuscripts, the Three Seals Law (Libra only) and the *Thotsaphit Ratchatham*.
- **No lesson-9 false positives.** No Pali- or Sanskrit-derived Thai word tripped the scan.
- **Law.** No law pointers appear outside Libra and Capricorn: other signs send law to Libra in passing. Libra keeps to the letter of the law (the Three Seals Law, statutes, court procedure). Capricorn keeps to the spirit of law.
- **Other checks.** No zodiac terms, URLs, "Indian", Human Universals or other universals lists, Hermes_research, or findings phrases appear anywhere.

## Repeat check (nation-wide)
- **Exact matches.** No non-template line of 25 or more characters appears in two sheets. That covers table rows, "Who to compare" bullets, Flags lines including "Languages needed", and first queries.
- **Near matches.** Of the 20 near-match pairs (similarity of 0.85 or more), 17 are short formulaic Held lines in Leo ("none; the epic named is Tai", "none; the texts named are Thai"). Each Held line is worded for its own sheet, so none is copied. The other three are short "Who to compare" bullets of similar shape:
  - Moken and Urak Lawoi, in Aries Autonomy and Taurus Security, and again in Cancer Care and Motherhood;
  - Khmer-speaking Thais and Kuy, in Leo Play and Joy.
  Each still gives a different reason, so I left them.
- **Recurring sources.** A handful of standard works recur in new rows with new reasons, for example Reynolds, Akin Rabibhadana, Skinner, Pasuk and Baker, Ivanoff on the Moken, and the Digital Library of Northern Thai Manuscripts. No row is copied.

## Thin, repetitive or generic sheets
- **Thinnest by pointer count:** Leo 11 Honor and Virgo 07 Criticism (13 each). Both are still full sheets.
- **Shortest:** Aries 09 Competition (1,056), Sagittarius 08 Honesty (1,074) and Aries 08 Anger (1,089). None reads as generic.
- **Formulaic Held lines:** Leo's "Held for review: none; the X named is Thai" pattern repeats in shape across 8 sheets.
- **Sagittarius:** Khmer-speaking Thais were missing at first and were added late, in only 5 of the 11 sheets.
- **No sheet reads like research or carries invented-looking names** in the three full-sheet spot-checks (Gemini Siblings, Libra Justice, parts of others). Named items are well-known real works and institutions, for example:
  - Sharp and Hanks's *Bang Chan*, Potter's *Family Life in a Northern Thai Village*, and Akin's *Organization of Thai Society*;
  - McCargo's *Fighting for Virtue* and Haberkorn's *In Plain Sight*;
  - Thai Lawyers for Human Rights and iLaw, and ThaiLIS and ThaiJO queries in Thai script.
  All are marked *check*.

## Does it exploit the nation's depth?
Largely yes.

- **Thai script and regions.** Every sheet has Thai-script terms, and every sheet has Lanna or Kham Mueang and Isan pointers. 127 of 130 name the Southern Thai.
- **Minorities.** Counts are sheets naming the group:

  | Group | Sheets |
  |---|---|
  | Thai Chinese | 124 |
  | Hmong | 122 |
  | Karen | 114 |
  | Moken | 84 |
  | Khmer-speaking Thais | 82 |
  | Satun and Thai Malay (non-Patani) | 78 |
  | Akha | 77 |
  | Mon | 76 |
  | Lahu | 63 |
  | Kuy | 57 |
  | Urak Lawoi | 54 |
  | Tai Yai (Shan) | 51 |
  | Mien | 49 |
  | Thai Vietnamese | 37 |
  | Lua/Lawa | 36 |
  | Maniq and Mlabri | 35 |
  | Phuket Baba-Peranakan | 35 |
  | Phu Tai | 32 |
  | Lisu | 25 |
  | Tai Lue | 20 |
  | Moklen | 11 |

  The rarer groups were nudged from Libra on, after the Phu Tai were absent and the Tai Lue, Tai Yai, Lua, Maniq, Mlabri and Peranakan were rare in the first six signs.
- **Pre-modern pointers.** Every sheet has at least one, judged by reading the 25 sheets a keyword scan missed. They include Sukhothai and Lanna inscriptions, Ayutthaya court texts, Rama II's dance-drama verse, chronicles, manuscripts, Isan *phaya* and Sri Thanonchai tales, and Ban Chiang. The weakest cases are Sagittarius Fundamentalism and Taurus Possession, which reach the pre-modern only through modern studies of the holy-man revolts and the Ban Chiang site.
- **Still thin:**
  - **Groups and languages:** the Moklen, the Tai Lue of Nan and Phayao, the Lisu and the So/Thavung; minority-language terms beyond Hmong, Karen and Isan (Akha, Lahu and Mon terms are fewer).
  - **Regions:** the west (Kanchanaburi, Tak, Mae Hong Son) is weaker than the north and northeast. The Eastern Seaboard (Chanthaburi, Trat) is rarely named.

## For the author
- **Lands.** Thailand's lands are still to be settled (Stage 0). The sheets assume the core Thai lands minus Patani.
- **Court Brahmin ritual.** Treating Thai court Brahmin ritual as Thai material (Sagittarius) is a judgment call to confirm.
