# Animal Crossing Amiibo Generator for emuiibo

Simple Python script to generate localized virtual Amiibos for **Animal Crossing** on Nintendo Switch.

If you use [emuiibo](https://github.com/XorTroll/emuiibo), you know that creating folders and editing JSON files manually can be tedious. I wrote this tool to automate the boring stuff.

It creates the necessary folder structure, generates the `amiibo.json` with unique IDs, and downloads the artwork for you. Plus, it handles name localization—so if you want "Canela" instead of "Isabelle", this tool has you covered.

## What it does

*   **Translations:** Automatically finds the correct name for your region (e.g., Spanish, French, German).
*   **Downloads Artwork:** Grabs the official Amiibo card/figure images.
*   **Random UUIDs:** Generates unique IDs so you can register them in-game without conflicts.
*   **Clean Organization:** Sorts everything into folders ready to drop onto your SD card.

## How to use

### Requirements
Just Python 3.

### Running the script
Open your terminal and run:

```bash
python3 ac_amiibo_gen.py
```

It will ask you a few simple questions (like which language you want and where to save the files).

**Advanced users:**
You can also run it with arguments to skip the questions:

```bash
# Example: Generate US Spanish (Mexican) Amiibos
python3 ac_amiibo_gen.py --locale USes --out ./MyAmiibos --no-random-uuid
```

## Credits

This tool wouldn't exist without these awesome projects:

*   **[XorTroll/emuiibo](https://github.com/XorTroll/emuiibo):** The original homebrew that makes virtual Amiibos possible.
*   **[AmiiboAPI](https://www.amiiboapi.com/):** For providing the database of characters and images.
*   **[alexislours/translation-sheet-data](https://github.com/alexislours/translation-sheet-data):** For the massive list of villager name translations.

## License

GNU General Public License v2.0 (GPLv2)
