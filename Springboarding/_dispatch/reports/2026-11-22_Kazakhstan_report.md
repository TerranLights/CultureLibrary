# Kazakhstan springboard run: report (2026-11-22)

Run agent for Kazakhstan, wave 2 of Sunday 11-22. Deeper brief (accuracy and depth first), one sub-agent per sign, Aries to Pisces, with lessons 1 to 9 added to every sub-agent prompt. Lands: none settled (no `00 - Scope.md`); the missing-scope note sits once, in each sign's Domain sheet; no unit list was added. East Turkestan appears only as comparison; Uyghurs in Kazakhstan are written as a minority of Kazakhstan. Nothing was read from `Hermes_research`.

**Result: 130/130 sheets done; whole-nation QA scan 0 problems; no repeated line, table row, Flags line or "Who to compare" bullet anywhere in the nation (my own check, exact and normalized).**

## Per sign
Words by `wc -w` after all fixes; pointers = rows in section 2.

| # | Sign | Sheets | Agents | Relaunches | QA scan | Avg words | Longest | Shortest | Pointers (min-max, avg) | Sub-agent tokens | Time |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Aries | 11 | 1 | 0 | 0 | 1,143 | 1,264 | 1,082 | 14-16, 15.2 | 163,350 | 08:37-08:50 |
| 2 | Taurus | 11 | 1 | 0 | 0 | 1,200 | 1,293 | 1,152 | 14-16, 14.9 | 204,477 | 08:50-09:06 |
| 3 | Gemini | 10 | 1 | 1 (Domain) | 0 | 1,249 | 1,295 | 1,196 | 14-16, 15.2 | 200,284 | 09:07-09:22 |
| 4 | Cancer | 10 | 1 | 0 | 0 | 1,225 | 1,274 | 1,136 | 16-16, 16.0 | 213,213 | 09:23-09:37 |
| 5 | Leo | 13 | 1 | 0 | 0 | 1,170 | 1,260 | 1,112 | 14-16, 15.0 | 243,842 | 09:38-09:57 |
| 6 | Virgo | 10 | 1 | 0 | 0 | 1,224 | 1,267 | 1,149 | 14-15, 14.3 | 221,673 | 09:58-10:13 |
| 7 | Libra | 11 | 1 | 0 | 0 | 1,201 | 1,264 | 1,150 | 13-15, 14.1 | 222,655 | 10:14-10:30 |
| 8 | Scorpio | 11 | 1 | 0 | 0 | 1,167 | 1,254 | 1,128 | 13-14, 13.8 | 217,862 | 10:31-10:47 |
| 9 | Sagittarius | 11 | 1 | 0 | 0 | 1,187 | 1,284 | 1,110 | 15-16, 15.1 | 239,095 | 10:48-11:06 |
| 10 | Capricorn | 10 | 1 | 1 (Hierarchy) | 0 | 1,245 | 1,292 | 1,159 | 15-16, 15.1 | 255,418 | 11:07-11:26 |
| 11 | Aquarius | 10 | 1 | 2 (Equality, Idealism) | 0 | 1,194 | 1,283 | 1,115 | 15-15, 15.0 | 214,500 | 11:27-11:40 |
| 12 | Pisces | 12 | 1 | 0 | 0 | 1,226 | 1,276 | 1,140 | 15-15, 15.0 | 268,977 | 11:41-12:03 |
| | **Nation** | **130** | **12 + 4 fix jobs** | **4** | **0** | **1,201** | **1,295** | **1,082** | **13-16, 14.9** | **2,665,346 + 277,080 = 2,942,426** | **08:36-12:08** |

**Tokens:** 2,665,346 for the twelve sign agents, 277,080 for the four single-concept fix jobs (68,191; 63,482; 66,076; 79,331): **2,942,426 sub-agent tokens in all.** Run agent's own tokens not included (the main session adds them). **Wall-clock:** start 08:36, end about 12:08 (about 3 h 32 min); no usage-limit stop.

**Length:** none over 1,300; 55 sheets over 1,200 (the brief allows "a little over"), the highest 1,295 (Gemini Domain, after its fix).

## Rule breaks and fixes
1. **South Asian rule (not caught by the scan; found by my name check).** Three sheets named a scholar of South Asian heritage (Bhavna Dave, *Kazakhstan: Ethnicity, Language and Power*, 2007): Gemini `00 - Domain and folkways` (pointer and first query 3), Capricorn `06 - Hierarchy` (pointer and first query 3), Aquarius `03 - Equality` (pointer). Aquarius `05 - Idealism` named a South Asian-derived religious community three times (search-language line, a pointer on its Karasai farm, a "Who to compare" bullet) and in first query 4. **Fixed by single-concept relaunches** (one each, all passed the first time): each pointer replaced by a different real pointer not used elsewhere in the nation (Gemini Domain: Pavlenko, ed., *Multilingualism in Post-Soviet Countries*, 2008; Hierarchy: Sarsembayev, *Central Asian Survey*, 1999; Equality: Kolstø, ed., *Nation-Building and Ethnic Integration in Post-Soviet Societies*, 1999; Idealism: the Soviet model city of Shevchenko, now Aktau), and each Held for review line now gives only the category. All marked *check*.
2. **Stock Flags line repeated across sheets (lesson 6).** "Held for review: none." stood word for word in 20 Taurus and Gemini sheets (the Aries agent had already varied its own). **Fixed by hand, smallest edit:** each line now names its concept ("none; no land, pasture or privatization pointer was set aside", and so on). No other Flags line or compare bullet repeats.
3. **Held lines that hold something (Sagittarius):** Freedom and Fundamentalism each set one pointer aside, written as the category only, as the brief asks.

## Judgment calls for the author
- **Afghanistan items kept:** Soviet-Afghan war veterans (Aries Courage, Virgo Service) and UNHCR's work with Afghan refugees (Cancer Shelter). These are Kazakhstani veterans and a refugee population, not South Asian works or scholars, and Afghanistan is not part of the subcontinent; say if the rule should cover them.
- **Law outside Libra and Capricorn, as events only:** Aries Anger names the 2024 Nukenova trial and the domestic-violence law passed after it, as a pointer to public anger, not as law research. Scorpio's trials and anti-corruption items are also events. Left as written.
- **Ahmad Yasawi, Sufi Allayar and the Yasawi Sufi tradition** are Turkic and Central Asian and were kept. Rashid Nugmanov (Kazakh film director) matched a name pattern and was kept.

## Thin, repetitive or generic sheets
- **No sheet is thin.** None is under 1,082 words or 13 pointers.
- **Leaner on pointers:** Scorpio (13.8 avg; Control and Secrecy at 13) and Libra (14.1; Domain at 13). After a prompt nudge, Sagittarius to Pisces went back to 15 to 16.
- **Fewer internal regions** (under four of west, east, north, south, Karaganda, Zhetysu, Almaty, Astana by keyword): Aries Beginning; Taurus Domain, Self-worth, Possessiveness (1), Stubbornness, Sensuality; Gemini Information, Duality (1); Cancer Protection, Care; Leo Leadership, Play; Aquarius Hope; Pisces Compassion. Taurus is the weakest sign for regional spread.
- **Pre-modern pointers:** every sheet has at least one by hand count (proverbs, customs, epics, lineage titles, Yasawi, 19th-century sources). Thinnest: Capricorn Merit (one: how the titles *bi*, *batyr* and *sheshen* were won) and Aries Anger (two: *qarğys* and 19th-century *barymta*).
- **Sources reused across signs** (different rows and reasons, no copied row): at most three uses each. Margulan's applied art, the Kazakh ethnographic encyclopedia of categories and terms; two uses each: World Values Survey, Cameron's *The Hungry Steppe*, Kindler's *Stalin's Nomads*, Ohayon, Schatz, Musrepov's *Ulpan*, Nurpeisov's *Blood and Sweat*, the Zar zaman poets, the Assembly of People of Kazakhstan, KazISS surveys, the Generations and Gender Survey and UNICEF. Not generic.

## Depth (whether the sheets exploit the nation)
- **Yes, on the whole.** Terms are in Kazakh Cyrillic with Latin forms and Russian in every sheet, and often also in Uyghur, Uzbek, Koryo-mar, Tatar, German, Chechen or Polish. Pre-modern layers recur: zhyrau and akyn verse, *aitys*, *Zheti zhargy* and *bi* courts, the zhuz and *shezhire*, Yasawi, Abai, Shakarim, Valikhanov, the Zar zaman poets, *kumalak* and the *müshel* cycle. Soviet-era layers recur too: the famine, sedentarization, the deportations, the Virgin Lands campaign, Semipalatinsk and the Aral. So do post-1991 sources: the 2021 census, the Bureau of National Statistics, Zhanaozen, January 2022, qandas resettlement and Latin-script reform.
- **Minorities: sheets naming each group** (out of 130): Russians 130, Uyghurs 127, Germans 116, Koryo-saram 114, Uzbeks 112, qandas/oralman 94, Ukrainians 91, Dungan 91, Tatars 70, Chechens 52, Ingush 35, Poles 25, Meskhetian Turks 11, Belarusians 10, Kyrgyz 9, Bashkirs 9, Kurds 6, Greeks 2. Azerbaijanis and Tajiks get 1 each. Every sheet names at least five groups.
- **Gaps for the later research:** Azerbaijanis, Tajiks, Kurds and Greeks are hardly present. Karakalpaks, Turkmen and the Mangystau Adai get little of their own. The Taurus regional spread is weak.

## Files
Sheets: `Targets/Asia/Central Asia/Kazakhstan/Springboards/01 - Aries/` to `12 - Pisces/` (130). Run log: 12 per-sign lines appended with `>>`, plus one completion line. The progress file's first line was not touched.
