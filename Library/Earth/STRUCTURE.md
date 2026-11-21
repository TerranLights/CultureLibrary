# Library/Earth: folder structure (scaffolded 2026-11-21)

```
Earth/
├── Upper Earth/
│   └── <Region>/                       (Asia is split into its regions: Asia/East Asia, ...)
│       ├── Tepenia-represented/         (culture-nations in Tepenia's census)
│       │   └── <Nation>/
│       │       ├── README.md
│       │       ├── 00 - Real-world baseline/
│       │       ├── 01 - First Interwar (2083-2564)/
│       │       └── Subunits/            (only where needed: the Sinian Federation's member states and Hakka)
│       └── Not Tepenia-represented/     (culture-nations that exist in the world but are not directly in Tepenia)
└── Tepenia/
    ├── 00 - Federation (national)/
    ├── <Subnet> subnet/<City>/{Human culture, Robot culture}/
    ├── <Subnet> subnet/Concordia/Districts/<district>/
    ├── Amundsen-Scott (nexus)/Amundsen Station/
    └── Other locations/
```

- **Regions** follow the DCI's targets (`Springboarding/Targets/`); Middle East, South Asia and South Caucasus are added under Asia for non-represented nations.
- **Inside an era folder** (Upper Earth) or a culture folder (Tepenia): one subfolder per sign (`01 - Aries/` to `12 - Pisces/`) and one file per concept, mirroring the springboards.
- **Names:** latest-period names for nations; current subnet names (to be renamed later); Concordia's districts by structural key.
- **Open:** the list of non-represented nations.
- **Deferred (author, 2026-11-21): a Second Interwar layer for Upper Earth.** Not needed now. If national borders fracture again at the War of Upper Earth (as they did at the Global War of 2083), the new nations' shapes would follow from their cultures in the late First Interwar Period, which must be synthesized first. A task for much later; when it comes, it is a `02 - Second Interwar (2564-2812)/` folder per nation (or new nation folders for successor states).
- The structure will be adjusted and expanded as needed (author).
