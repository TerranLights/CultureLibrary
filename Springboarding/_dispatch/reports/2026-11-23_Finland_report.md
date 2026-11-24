# Finland springboard run: report (2026-11-23)

This run agent handled Finland in Monday's wave 1, under the deeper brief (accuracy and depth first). It used one sub-agent per sign, Aries to Pisces, one after another. Nothing in the sheets has been verified, and every named item is marked *check*.

## Result
- **130/130 sheets done** across the 12 signs, written by 12 sign agents, with **0 relaunches**.
- **Whole-nation QA (`springboard_qa.py Finland`):** 130 sheets scanned, 0 problems.
- **Repeat check across the nation** (the run agent's own scripts):
  - Exact repeats: **0**. The check covered every non-template line, table row, "Who to compare" bullet, Flags line and first query.
  - Near matches: **0** at a ratio of 0.85 or above, on sections 3 to 5.
  - At 0.80 there were 3 pairs. Each pair shared only a frame such as "Finland-Swedes and Ålanders: check Swedish-language ...", and the content differed by concept. They were left as they are.
  - The sub-agents also checked their sheets against all earlier signs and reworded near-copies before finishing.
- **Sub-agent tokens: 3,019,533** (758 tool uses). The main session adds the run agent's own tokens.
- **Wall clock:** about 05:04 to 09:53.
  - First launch 05:05, last return 09:46.
  - At 07:27 a forced hand-back interrupted the run while the Libra sub-agent was still writing. It was not a usage limit. The main session resumed the run at once. No duplicate agent was launched, and Libra finished on its own at 07:29.
  - There was no HTTP 429 stop.
- **Words by `wc -w`:** average 1,196, range 1,038 to 1,295, none over 1,300. 64 sheets run over 1,200 (mostly Domain sheets and the later signs).
- **Pointers per sheet:** 13 to 16, average 14.4 (1,871 in all).

## Per sign
| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers (avg) | Sub-agent tokens | Tools | Time |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1,123 | 1,251 Domain | 1,038 Recklessness | 14-16 (15.5) | 163,167 | 31 | 05:05-05:18 |
| 2 | Taurus | 11 | 1,202 | 1,277 Ownership | 1,132 Possessiveness | 13-14 (13.7) | 240,642 | 62 | 05:19-05:40 |
| 3 | Gemini | 10 | 1,245 | 1,282 Learning | 1,197 Gossip | 14-16 (14.9) | 227,356 | 53 | 05:41-06:01 |
| 4 | Cancer | 10 | 1,207 | 1,280 Domain | 1,157 Belonging | 14-15 (14.1) | 246,678 | 56 | 06:02-06:27 |
| 5 | Leo | 13 | 1,161 | 1,266 Domain | 1,085 Generosity | 13-15 (13.9) | 273,924 | 68 | 06:28-06:51 |
| 6 | Virgo | 10 | 1,204 | 1,246 Usefulness | 1,146 Criticism | 13-16 (14.2) | 250,684 | 66 | 06:52-07:09 |
| 7 | Libra | 11 | 1,182 | 1,294 Domain | 1,116 Reciprocity | 14-16 (14.7) | 223,543 | 53 | 07:10-07:29 |
| 8 | Scorpio | 11 | 1,205 | 1,267 Death | 1,149 Trust | 13-15 (13.6) | 250,054 | 54 | 07:30-07:50 |
| 9 | Sagittarius | 11 | 1,235 | 1,291 Domain | 1,186 Conviction | 14-16 (15.1) | 250,681 | 65 | 07:51-08:09 |
| 10 | Capricorn | 10 | 1,158 | 1,295 Domain | 1,100 Ambition | 14-15 (14.2) | 281,016 | 55 | 08:10-08:32 |
| 11 | Aquarius | 10 | 1,215 | 1,276 Reform | 1,162 Detachment | 14-16 (14.8) | 253,851 | 79 | 08:33-08:57 |
| 12 | Pisces | 12 | 1,227 | 1,264 Compassion | 1,138 Intuition | 13-15 (14.0) | 357,937 | 116 | 08:59-09:46 |

## Rules, breaks and fixes
- **Lands:** the tracker lists no settled lands, and there is no `00 - Scope.md`.
  - Each sign's Domain sheet states this once, and no other sheet repeats it. There is no unit list.
  - The pre-war lands carried in Russia (Finnic and Karelian people and lands such as Karelia) are pointed to as part of the nation's people where a concept needs them. No borders are settled.
- **South Asian rule:**
  - The QA pattern found 0 hits outside the Held lines.
  - The run agent also scanned every sheet by name for South Asian scholars, writers, works, communities and religions. The scan was clean.
  - The category appears in 15 Held lines; see the judgment calls below.
- **Universals:** no Human Universals and no universals list anywhere. The one hit for "universal" is Aquarius, Idealism, which names the ESS human-values module's dimensions "universalism, benevolence" (Schwartz's value types). That is a survey's own term, not a universals list, and it is kept as written; see the judgment calls.
- **"Indian", zodiac words, URLs, findings phrasing:** none.
- **Hermes_research:** not opened, not cited.
- **Law:** Libra keeps to the letter of the law (the 1734 Code, Finlex texts, the Åland and Sámi Parliament acts as texts), and Capricorn to the spirit. Other signs send legal texts to Libra or Capricorn, often in their Held line.
- **Stereotypes:** a phrase scan of every "Who to compare" bullet found none. Ideas such as *sisu*, the "silent Finn", work ethic, high trust and egalitarianism appear only as claims to examine.
- **No relaunches and no hand edits were needed.**

## Coverage
Number of sheets (out of 130) that mention each region or people:

| Region or people | Sheets |
|---|---|
| Sámi | 130 |
| Somali-Finns | 130 |
| Åland | 129 |
| Russian-speakers | 129 |
| Ostrobothnia | 128 |
| Kale Roma | 128 |
| Lapland | 127 |
| Tatars | 122 |
| Uusimaa | 119 |
| Kainuu | 116 |
| North Karelia | 115 |
| Karelians | 114 |
| Jews | 109 |
| Savo | 107 |
| Ingrian Finns | 98 |
| Tavastia | 95 |
| Turku | 89 |
| Old Believers | 87 |
| Meänkieli | 5 |
| Kven | 2 |

- Meänkieli and Kven appear rarely, which is apt because their speakers live mainly in Sweden and Norway.
- **Pre-modern pointers:**
  - *Kalevala* in 46 sheets and SKVR in 48; Agricola in 10.
  - Every sheet carries at least one older or folk-tradition pointer. Examples: treasure legends, Turku guild records, the 1771 *Tidningar Utgifne Af et Sällskap i Åbo*, Swedish-era tax and church records for Sámi families, peasants' border-peace pacts, the 1840s *hihhulit* revival, and Matti Kuusi's proverb studies.

## Do the sheets exploit the nation's depth?
Mostly yes.
- **Languages:** the sheets use Finnish and Finland-Swedish terms throughout, and North, Inari and Skolt Sámi, Karelian and Kale Romani terms where the sub-agents were confident. Uncertain terms are marked *check*.
- **Institutions:** they draw on Finland's strong institutional layer: SKS and SLS archives, Kotus, Statistics Finland, the Finnish Social Science Data Archive, THL, Yle, the National Library's digitized press, Siida and the Sámi Archives in Inari, ÅSUB and Åland's own institutions.
- **Movements:** they point to the revival movements, the popular movements and the Orthodox tradition.
- **Thinner spots:** these are honestly labeled thin rather than padded. Old Believers, Tatars, the Kale for some concepts, Skolt and Inari Sámi vocabulary, and Ingrian Finns are pointed to through their own organizations, with a note that sources are scarce.
- **Repeated sources:** a few sources recur across signs in new, differently worded rows. Examples: SKVR, Finna, the ESS Finnish rounds, the Youth Barometer, *Kunnian kenttä* and the Independence Day reception. This is acceptable, but a later researcher will meet them often.

## Thin, repetitive or generic sheets (by name)
- **Shortest sheets** are still full: Aries Recklessness (1,038), Aries Initiative (1,044), Leo Generosity (1,085), Capricorn Ambition (1,100).
- **Sagittarius Held lines:** all eleven carry the South Asian category, each reworded for its concept. Some read as filler, for example Honesty ("whose news and elders they trust") and Meaning ("self-help imports"). From Capricorn on, the sub-agents were told to use the category only where a real pointer was set aside. After that it appeared only in Capricorn Merit, Aquarius Equality and Pisces Spirituality.
- **Held lines used for other matters:** several early sheets use the Held line for other things, such as an accuracy hold on Karelian and Romani terms (Aries Domain) or a note routing a pointer to Libra or Capricorn. This is harmless but not the line's strict use.
- No sheet reads as generic.

## Judgment calls for the author
1. **Hiring field experiment:** Virgo Discernment and Capricorn Merit each hold one hiring-discrimination field experiment, unnamed, described as "by a South Asian-heritage scholar". It is set aside under the standing rule. Confirm the hold, and that this wording of the Held line is acceptable.
2. **Sagittarius Held lines:** all eleven carry the South Asian category. Keep them as they are, or trim them to the Domain sheet only?
3. **"universalism, benevolence"** in Aquarius Idealism: this is the ESS human-values module's own vocabulary, not a universals list. Keep it, or reword it to "the human-values module"?
4. **Russia's Finnic lands:** Karelians and Ingrian Finns in the pre-war lands are treated as part of the nation's people, with no borders drawn. The author settles the lands at Stage 0.
5. **Sámi across the border:** Sámi in Norway and Sweden are comparison only. Estonia, Sweden Finns and American Finns are comparison only.
6. **Aries Domain:** its Held line keeps the Karelian and Kale Romani name terms on hold until a dictionary confirms them. This is an accuracy hold, not a standing-rule hold.
