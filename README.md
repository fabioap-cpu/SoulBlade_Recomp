# SoulBlade-Recomp



**Static recompilation of *Soul Blade* (USA) for the PlayStation 1.**

Built on [PSXRecomp](https://github.com/mstan/psxrecomp) — a MIPS R3000A → C → native x64 static recompilation framework. The game executable is recompiled to produce a single binary that runs without an emulator, delivering perfect native performance.



---

## Requirements

To run a release of SoulBlade-Recomp, you need your own legally obtained copy of:

- **Soul Blade (USA)** — disc image (`.cue`/`.bin`)

No retail BIOS image, game disc image, or game assets are included in or distributed by this repository or its releases.

---

## Status

**Playable with Custom Enhancements.** What works today:

- ✅ **Boots and plays** — The game runs natively with full rendering, input, and memory-card saves.

- ✅ **High Resolution** — Configured for HD scaling via `settings.toml`.
- ✅ **Supersampling & Filtering** — 2x Supersampling with nearest-neighbor filtering to preserve sharp pixel aesthetics.
- ⚠️ **Scope:** USA region only. Other regions are untested.
- ⚠️ **Known Issues:** There is a minor graphical glitch with water rendering. This is an engine-level issue expected to be resolved by the PSXRecomp community in future runtime updates.

---

## Setup

### 1. Download a Release (recommended)

Grab the release archive from [Releases](https://github.com/fabioap-cpu/SoulBlade-Recomp/releases), extract it, and run the executable. 

1. **Provide the game disc** — You must provide your own legal copy of the game. Place your `.cue` and `.bin` files inside the extracted Release folder.
2. **Configure the path** — Open the `game.toml` file and set the `[disc]` path to your `.cue` file:
   ```toml
   [disc]
   path = "Soul Blade (USA).cue"
   ```
3. **Launch** — Run `SoulBlade-Recomp.exe`.


---

## Community Contributions
Any community fix or pull request is welcome! The idea is to further improve the engine code, making all games more compatible and accurate. Feel free to contribute and help expand the scope of native PlayStation recompilation.

---

## Credits
* **Port / Configuration / Engine Fixes:** [fabioap-cpu](https://github.com/fabioap-cpu)
* **Base Recompiler Technology:** [psxrecomp](https://github.com/mstan/psxrecomp) by mstan

