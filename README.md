# The Culture Library

The central database of **cultures** for the Tepenian universe: how each culture-nation, city and later off-world society understands the world, concept by concept, and how those cultures change over time. Every work set in the universe (games, novels, TV) draws its cultures from here, so that the same people are written the same way everywhere.

## What this repo is (and is not)
- **Results, not methods.** The methods that produce these results live in [Derivation Mechanisms](https://github.com/TerranLights/DerivationMechanisms), above all the [DCI (Deep Culture Investigation)](https://github.com/TerranLights/DerivationMechanisms/tree/main/Environment/DCI%20[Deep%20Culture%20Investigation]). This repo holds what they find.
- **Not canon history.** The Timeline of events, eras and places is kept in the [Tepenian Universe Timeline](https://github.com/TerranLights/TepenianUniverseTimeline). This repo records how people think, value, behave and live in those places and eras.

## How the cultures build on each other
Each layer is derived from the one before it, never invented from scratch:

1. **Upper Earth** (the real world, then the First Interwar Period, 2083 to 2564): cultures researched from real-world sources and then carried forward to the time of the exile to Antarctica.
2. **The Tepenian Federation** (from 2564): the cultures of its cities, synthesized from the Upper Earth cultures of the people who settled them. They are new cultures, not real ones.
3. **Mars and the Belt, then Jupiter, then Saturn, then the Alpha/Proxima Centauri System:** each derived from the layer before, starting from Tepenia's synthesized cultures rather than from real-world research.

## Layout

| Folder | What it holds |
|---|---|
| `Library/` | **The finished results**, by world: `Earth/` (`Upper Earth/` and `Tepenia/`), `Mars/`, `Jupiter/`, `Saturn/` and `x_Alpha-Proxima_Centauri/`. Each world's `README.md` names the works that draw on it; `Library/Earth/STRUCTURE.md` explains the Earth layout. |
| `Springboarding/` | **The DCI's springboard stage**: starting points for the research (search terms, sources, regions and minorities to cover) for each culture-nation, sign by sign and concept by concept, plus the run's own records (`_dispatch/`: progress log, schedule, reports, cost ledger). Springboards are not results: they say where to begin looking, not what is true. |

### Inside `Library/Earth/`
- `Upper Earth/<Region>/` is split into **`Tepenia-represented/`** (culture-nations whose people are in Tepenia's census) and **`Not Tepenia-represented/`** (culture-nations that exist in the world but are not directly represented in Tepenia). Each culture-nation has a real-world baseline and a First Interwar layer.
- `Tepenia/` is organized by subnet and city, with each city's **human culture** and **robot culture** kept apart, Concordia's districts, a national layer shared by the whole Federation, and other locations (towns, highways, ports, the Tower).

## Status
- **Springboarding:** under way (2026-11). Every culture-nation represented in Tepenia gets 130 springboard sheets (twelve signs, one sheet per concept plus a domain sheet per sign).
- **Library:** scaffolded; results are added as the full research and the city syntheses finish. The structure will be adjusted and expanded as needed.
- **Later:** the springboard files and general web-research results are to move to the ArchiveVault repo at some point; for now they stay here.
