# Ukraine: springboard scouting report (2026-11-25)

Run agent, deeper brief, one sub-agent per sign (12 sub-agents). **130/130 sheets done**, all first lines `STATUS: done 2026-11-25, not verified`. Sheets: `Targets/Europe/Ukraine/Springboards/`.

- **Wall clock:** run agent start 05:06, first sub-agent 05:07, last sub-agent end 08:59, nation-wide checks done 09:03 (about 4 hours).
- **Sub-agent tokens:** 3,032,043 in total (12 agents, 816 tool calls), about 233,000 per sign. The run agent's own tokens are not counted here.
- **Relaunches:** 0. Every fix was a run-agent smallest edit (6 edits, listed below).
- **QA (`springboard_qa.py Ukraine`):** 130 sheets scanned, 0 problems. There were no false positives, and no "Indian" or "sikh" hits.

## Per-sign table

| # | Sign | Sheets | Avg words | Longest | Shortest | Pointers | Sub-agent tokens (tools) | Time | Fixes |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11/11 | 1,196 | 1,268 Identity | 1,129 Independence | 14-16 | 179,964 (43) | 05:07-05:23 | none |
| 2 | Taurus | 11/11 | 1,199 | 1,271 Possession | 1,142 Stubbornness | 14-15 | 219,081 (50) | 05:24-05:40 | none |
| 3 | Gemini | 10/10 | 1,208 | 1,268 Domain | 1,165 Information | 14-15 | 211,455 (42) | 05:41-05:54 | Learning: search-term row echoed Taurus/Values (0.91), so it was rewritten; Held line trimmed (see below) |
| 4 | Cancer | 10/10 | 1,196 | 1,274 Domain | 1,109 Nurture | 14-16 | 215,125 (41) | 05:55-06:07 | none |
| 5 | Leo | 13/13 | 1,207 | 1,285 Domain | 1,076 Joy | 14-16 | 251,201 (59) | 06:08-06:25 | none |
| 6 | Virgo | 10/10 | 1,190 | 1,296 Domain | 1,104 Perfectionism | 13-15 | 223,381 (44) | 06:26-06:40 | Domain: Lands line echoed Leo's (0.93), so it was reworded |
| 7 | Libra | 11/11 | 1,192 | 1,258 Projection | 1,134 Balance | 13-14 | 249,021 (91) | 06:41-07:00 | none |
| 8 | Scorpio | 11/11 | 1,226 | 1,266 Domain | 1,140 Crisis | 14 | 281,808 (86) | 07:01-07:21 | Domain: church-bodies compare-bullet label echoed Libra's Domain (0.86), so it was relabeled |
| 9 | Sagittarius | 11/11 | 1,173 | 1,249 Domain | 1,065 Conviction | 13-14 | 277,963 (89) | 07:22-07:46 | Education and Fundamentalism: Held lines trimmed so the set-aside item cannot be identified |
| 10 | Capricorn | 10/10 | 1,190 | 1,298 Domain | 1,104 Discipline | 14 | 267,928 (72) | 07:48-08:04 | none |
| 11 | Aquarius | 10/10 | 1,207 | 1,264 Domain, Community | 1,137 Nonconformity | 12-14 | 325,967 (89) | 08:05-08:30 | none |
| 12 | Pisces | 12/12 | 1,207 | 1,287 Domain | 1,109 Intuition | 13-14 | 329,149 (100) | 08:31-08:59 | none |

Across the nation the average is 1,200 words by `wc -w` (longest: Capricorn Domain at 1,298; shortest: Sagittarius Conviction at 1,065). No sheet is over 1,300.

## Pointers
There are 1,835 pointers across the 130 sheets (12 to 16 per sheet, average 14.1), with 1,832 distinct pointer labels. Only three pointers appear twice: the Chirikli Roma women's foundation (Taurus Self-worth, Pisces Empathy), the Ferenc Rákóczi II Transcarpathian Hungarian College (Gemini Learning, Pisces Domain) and the *Сказання про Бориса і Гліба* (Gemini Duality, Libra Peace at any price). Each comes back with a different reason.

## Repeat check (own; lines, table rows, "Who to compare" bullets, Flags lines, first queries)
- **Exact repeats:** 0, within Ukraine and against Belarus, Romania, Hungary, Bulgaria and Poland (Poland had no sheets yet when checked).
- **Near matches at 0.85 or above** (within Ukraine; against Belarus and Romania): three were fixed (above). Two are kept: the Trust and Power rows for Transcarpathian Hungarian (*bizalom* and *hatalom*) and the Aquarius Hope and Pisces Compassion rows for Crimean Tatar (*umut* and *merhamet*). In both pairs the term is different and only the table frame matches. There are no near matches against Belarus or Romania.
- **Lands note:** once per sign, in each Domain sheet's Flags, worded differently each time. No sheet mentions a scope file, and no unit list was added.

## Rule breaks and fixes
- **South Asian rule:** no South Asian name, work, community or language appears outside a Held line. The category is held on four sheets, each as a real set-aside: Gemini Learning, Sagittarius Education, Sagittarius Fundamentalism, and Pisces Spirituality (South Asian-derived meditation and body practices). Three of these Held lines said enough about the set-aside pointer to identify it (second-language learning studies; foreign students at the medical universities; a movement targeted by anti-sect writing). I trimmed them to "one pointer was set aside" plus the category.
- **Buddhism:** held as a category only on Aquarius Detachment and Pisces Spirituality. Nothing is named.
- **Universals, Hermes, banned words:** clean. The only "Brown" is Kate Brown's *Manual for Survival*, a Chornobyl history.
- **Law:** letter of the law in Libra only and spirit in Capricorn only. Other signs route law to them (for example the mobilization rules in Scorpio, the Pale of Settlement in Pisces, property law in Taurus).
- **Process slips reported by sub-agents:** the Capricorn sub-agent ran `springboard_qa.py` itself (outside the brief's inputs; harmless). It also wrote one temp file directly in `/tmp/claude-1000/`, which it deleted; I confirmed it is gone. The Aquarius sub-agent edited three sheets (Domain, Group, Reform) after marking them done; they are still complete and clean.

## Thin, repetitive or generic sheets
- **None are thin by count.** The lowest pointer counts are Aquarius Detachment (12) and the 13-pointer sheets in Virgo (Perfectionism), Libra (Balance to Projection), Sagittarius (Domain, Conviction, Honesty, Fundamentalism), Aquarius and Pisces (Surrender, Crime, Fear). The shortest are Sagittarius Conviction (1,065) and Honesty (1,068).
- **Somewhat repetitive in form:** the Cancer Held lines all share one sentence shape ("X was weighed and left out; no standing rule"), though each names a different item. Prompts from Leo on asked for varied shapes, and the later signs vary.
- **Reuse across signs:** Aquarius brings back a few earlier sources with a new focus: the Kyiv Caves Patericon, *Барвінок*, items from the ESS and the WVS, and Green Week. This is flagged by the sub-agent, not hidden.
- **Generic sheets:** none spotted. Every sheet names regional and minority pointers.

## Depth
Yes, the sheets use the nation's depth, and from Aries on. Pre-modern pointers appear in every sign, for example:
- St Sophia's graffito on Boyan's land, the Izbornyk of 1076 and the Rus'-Byzantine treaties;
- the Kyiv Caves Patericon, the Galician-Volhynian Chronicle, the Lithuanian Metrica and the Third Statute, the 1557 *voloka* reform and castle-court books;
- the Samovydets, Velychko and Hrabianka chronicles, Orlyk's Constitution, the 1743 *Prava*, and Skovoroda;
- the *dumy*, Crimean Khanate *kadı* registers and *yarlıq* charters, and the Hasidic texts of Mezhyrich, Polonne, Berdychiv, Korets and Breslov.

Minorities and regions recur across signs:
- the Crimean Tatars, Karaim and Krymchaks;
- the Azov Greeks (Rumeic and Urum);
- Rusyns, Hutsuls, Boykos and Lemkos;
- the Hungarians of Berehove and Uzhhorod, and the Romanians of Bukovina and the Budjak;
- the Bulgarians and Gagauz of the Budjak (Bolhrad);
- Lipovans, Mennonites and German colonists, Doukhobors and Molokans;
- Roma groups, Poles, the Jewish communities, Baptists and Pentecostals, and the two Orthodox jurisdictions and the Greek Catholics.

Search terms come in Ukrainian dialect forms, *surzhyk*, Russian, Crimean Tatar, Yiddish, Hebrew, Hungarian, Romanian, Church Slavonic, Rumeic and Urum. The thinnest groups (Krymchaks, Urum speakers, Gagauz) are flagged as thin, with where to look; nothing is padded.

## Judgment calls for the author
1. **Lands (Stage 0):** the census's successor table lists "Ukraine → Russia (core state)", while Ukraine is also a target. Whether Ukraine's lands are split between the two rows, and where, is open. The sheets are written for Ukraine as the sources treat it, with Crimea and the east as lands with their own peoples, and no border settled.
2. **Lev Sylenko's *Мага Віра* and RUNVira** (Sagittarius Faith) are kept as a Ukrainian native-faith pointer. Please confirm that this does not fall under the South Asian rule.
3. **Buddhism** is held as a category on Aquarius Detachment and Pisces Spirituality.
4. **The no-stereotype rule** is used once as a reason to hold: in Virgo Discernment, tabloid "romance-scam" exposés that profile one city's women are held as evidence of the stereotype only.
5. **Indigenous peoples:** Aries Identity gives *корінні народи* as the official term for the Crimean Tatars, Karaim and Krymchaks (the legal side is routed to Libra). Please confirm that this usage suits the survey's own "Native or Indigenous" wording.
6. **Restricted or private material** was kept out by choice in four places: Soviet dissidents' psychiatric files (Aquarius Nonconformity), closed veterans' chats (Leo Honor), videos of the abuse of captives (Leo Humiliation), and Hutsul *molfary* knowledge, a lead only where its keepers choose to speak (Scorpio Secrecy).
7. **Diaspora** pointers stay comparison only. One was deliberately kept back on Capricorn Duty (men's duties in the diaspora).
