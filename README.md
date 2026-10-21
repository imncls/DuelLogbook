<p align="center">
  <img src="assets/icon/functiongraphic.png" alt="Duel Logbook" width="640">
</p>

<h1 align="center">Duel Logbook</h1>

<p align="center">
  A companion app for your <b>physical</b> Yu-Gi-Oh! matches: Life Points counter, match tracking, deck library and stats.<br>
  Not a simulator, a tabletop helper.
</p>

<p align="center">
  <a href="https://github.com/imncls/DuelLogbook/releases/latest"><b>Download</b></a> ·
  <a href="#features">Features</a> ·
  <a href="#privacy">Privacy</a>
</p>

---

## Features

**Life Points counter**
- Big, animated LP display with quick damage/gain buttons (you choose the amounts), halve, custom amount, or set an exact value.
- Undo, full change history, and sound/visual feedback for every change.
- A quick counter for casual duels, with no setup and nothing saved.

**Matches**
- BO1, BO3, BO5 or a custom number of wins, with configurable starting LP (8000 by default).
- Each player can switch decks between duels. A duel ends automatically when someone hits 0 LP.
- Notes per duel, and the option to abandon a match.
- Close the app mid-duel and pick up exactly where you left off.

**Decks**
- A shared deck library with Main, Extra and Side Deck: any player can use any deck.
- Add cards by name or ID, or import a `.ydk` file or a plain list of IDs. Card data comes from [YGOPRODeck](https://ygoprodeck.com/).
- Banlist check for TCG, OCG and Goat formats.
- A Master Duel-style card grid for every deck.

**Stats**
- Per profile: win rate over time, streaks, an activity calendar, best and worst opponents, and the decks they've used.
- Per deck: record, matchups against every opposing deck, and who has played it.
- Head-to-head comparisons between two players or two decks.
- An LP chart for every duel in your match history.

**And also**
- Player profiles with optional photos.
- Light and dark themes, in English and Spanish.
- Backups to a JSON file you can share and restore on another device.

## Download

Get the latest version from the [**Releases page**](https://github.com/imncls/DuelLogbook/releases/latest).

| Platform | File | How to install |
|---|---|---|
| Android | `DuelLogbook-vX.Y.Z-android.apk` | Open the APK on your phone. Android will ask you to allow installing apps from that source (your browser or file manager). |
| Windows 10/11 (64-bit) | `DuelLogbook-vX.Y.Z-windows-x64.zip` | Extract the whole zip into a folder and run `duel_logbook.exe`. Keep the files next to it: the app needs them. |

**"Windows protected your PC"?** The Windows build isn't code-signed yet (certificates are expensive for an independent project), so SmartScreen warns about any new unsigned app. Click **More info → Run anyway**. If you'd rather check first, compare your download against the checksum below or scan it on [VirusTotal](https://www.virustotal.com/).

**Windows says `VCRUNTIME140.dll` is missing?** Install Microsoft's [Visual C++ Redistributable (x64)](https://aka.ms/vs/17/release/vc_redist.x64.exe).

### Verifying your download

Every release includes a `SHA256SUMS.txt` file. To check that a file is exactly the one that was published:

    # Windows (PowerShell)
    Get-FileHash .\DuelLogbook-vX.Y.Z-windows-x64.zip -Algorithm SHA256

    # Linux / macOS / Git Bash
    sha256sum -c SHA256SUMS.txt

The hash has to match the one in `SHA256SUMS.txt` (PowerShell shows it in uppercase; that's fine).

## Privacy

- **Everything stays on your device.** No accounts and no server of ours. Profiles, decks, matches and stats are stored locally.
- **The local database is encrypted** with a random key the app generates and keeps in your system's secure storage. There's no password to remember.
- **Card data** comes from the public YGOPRODeck API. Requests contain only the card name or ID you searched for, never personal data. Images are cached so they aren't downloaded again.

The full privacy policy and terms of use are inside the app (Settings → About).

## Disclaimer

Duel Logbook is an independent fan-made project. It is not affiliated with, sponsored by, or endorsed by Konami Digital Entertainment. "Yu-Gi-Oh!" and card/format names are trademarks of their respective owners, used here for descriptive purposes only. Card data and images are provided by [YGOPRODeck](https://ygoprodeck.com/).

## License

[Apache License 2.0](LICENSE)