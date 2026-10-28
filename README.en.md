<p align="center">
  <img src="assets/identidade/Megazord-Toolkit-kit-v1/02-icone-aplicativo/megazord-toolkit-icone-256px.png" width="128" alt="Megazord Toolkit">
</p>

<h1 align="center">Megazord Toolkit</h1>

<p align="center">
  <b>Championship Manager 01/02</b><br>
  <a href="README.md">Português</a>
</p>

---

One of the perks of rewriting the whole game's code is really understanding how it works "under the hood" (if you don't know what I'm talking about, have a look at [this thread](https://champman0102.co.uk/viewtopic.php?t=11029)).

I'd like to show you a project I've been working on that grew out of that work: Megazord Toolkit. It's an editor for Championship Manager 01/02 that, as the name suggests, brings together in a single program the features of several tools the community uses: real-time editing of the running game, save editing, the scout and the regen finder.

**Beta:** back up your save before using it, and report bugs [here][bugs].

## What it does

- **Two modes, the same screens:** edits the game while it runs (reading and writing its memory) or a saved `.sav`. A fixed bar shows the mode; what exists in only one mode is shown locked in the other, with an explanation.
- **Picks the game process** from a list, Cheat Engine style. The executable can have any name.
- **Searches people** by part of the name, ignoring accents and case.
- **Full team view in one go:** squad, staff, finances, kits and rivals, with the **kit colours** as the screen theme.
- **Person sheet** with attributes **as the game shows them (1–20)**, using the game's own attribute names.
- **Field-by-field editing:** writes **only what you changed**, with a "before → after" list to check: full contract, club, stadium, nationalities, preferences and the staff's preferred formation.
- **In the game's currency:** the game stores money in pounds and shows it in the currency chosen in the options. The editor does the same sum, so you see and type values in your own currency.
- **Undo:** every write goes into the history, and the **Undo** button (or Ctrl+Z) reverts the last one.
- **Transfers, loans and releases**, of players and staff.
- **Squad in groups:** first team, reserves and not in squad, with actions on one group only; moving a player between groups takes him out of the tactics, as the game does.
- **Release a player in a competition:** when he "cannot play for a second club in this competition", the editor shows which club he is registered for and releases him to the current club.
- **Scout:** searches the whole database by position, age, CA, PA, nationality, club and contract end, with **batch actions** (heal, renew, transfer-list…).
- **Regens:** shows the exact list of players the game itself generated, with the game running or from the save.
- **Quick actions** on the squad and on a person: heal injuries, condition, morale, CA/PA +2, renew or end a contract.
- Light and dark mode, Portuguese and English.

## Requirements

- Windows 10 or 11. The installer includes WebView2; if you use the zip, you need it installed (Windows 11 already has it).
- Championship Manager 01/02 **3.9.68**, unpatched or patched with NickPatcher (such as the CLZ Leagues Patch). On an executable from another version, the editor **warns you and does not open**, so it never writes to the wrong place.

## How to use

1. Install with the installer (`MegazordToolkit-…-setup.exe`) and open Megazord Toolkit; or, with the zip, run `MegazordToolkit.exe`.
2. Pick the game process (with your career loaded) or a `.sav`.
3. Search for a person or pick a club on the side bar. Edit and save.

## Thanks

The project was born out of admiration for the tools that kept the game alive for twenty years. These people's work served as inspiration and study:
- **AnoXic**: CMRTE (Real Time Editor)
- **Graeme Kelly**: SaveGame Editor
- **Michael Nygreen**: CM Scout
- **Yuri Kitashin Jr.**: CMExplorer
- **Dirty Andy**: GPF2 (Generated Players Finder)

---

*Championship Manager* is a trademark of its respective owners. This project is not affiliated with Sports Interactive or Eidos.

[bugs]: https://github.com/CM0102-Rust/Megazord-Toolkit/issues
