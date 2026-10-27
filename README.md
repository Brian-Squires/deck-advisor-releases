# Deck Advisor

> **This is a release-only repository.** Deck Advisor is closed-source software. This repository exists only to publish the compiled Windows app and to collect feedback. The source code is proprietary and is not published here or anywhere else.
>
> **Issues and discussions are welcome.** Report bugs, ask questions and suggest features in [Issues](../../issues) (and [Discussions](../../discussions), if enabled). Pull requests can't be accepted, because there's no source code here to change.

Deck Advisor is a free Magic: The Gathering deckbuilding assistant for Windows. It runs on your own computer and opens in your web browser. No account is needed, and no AI service is involved: the analysis and suggestions are worked out locally.

- Builds Commander, Brawl, Standard, Pioneer, Modern, Legacy, Vintage, Pauper, Historic and Timeless decks, and checks legality, deck size, copy limits, color identity and banned cards.
- Charts the mana curve, colors and the jobs your cards do, and names what the deck is about.
- Suggests cards with the reasons behind each one: combos you're close to, cards that work with what you have, gaps to fill, staples, and cuts to consider. You can limit suggestions to your own collection.
- Imports your collection from most collection apps (Mythic Tools, ManaBox, Moxfield, Archidekt, Deckbox, Dragon Shield, Delver, EchoMTG, TCGplayer and more) or from any CSV or text list.
- Second Wind: see which older cards a new set made better, and which new cards fit your decks.
- Playtest opening hands, set a budget, keep a version history of each deck, and print a deck guide.

**Deck Advisor is free and always will be.** There are no paid features, ads or subscriptions.

## Download and install

Deck Advisor runs on **Windows 10 and 11 (64-bit)**.

1. Open the [**Releases**](../../releases) page and find the latest release (marked **Latest**).
2. Under **Assets**, download `DeckAdvisor-<version>.exe`.
3. Optional: check that the download is intact. Each release also lists the file's SHA-256 checksum in `DeckAdvisor-<version>.exe.sha256`. In PowerShell, run:
   ```powershell
   Get-FileHash .\DeckAdvisor-<version>.exe -Algorithm SHA256
   ```
   The hash should match the one in the `.sha256` file.
4. Save the exe anywhere you like, for example your Desktop or Documents folder. Nothing needs installing.
5. Double-click it. A small window opens, and Deck Advisor opens in your browser at `http://localhost:4310`. Keep that window open while you use the app. To stop, click **Quit** at the top right of the app, or close the window.

**"Windows protected your PC."** The exe isn't code-signed, so Windows SmartScreen may show this the first time. Click **More info**, then **Run anyway**.

**First start.** The app downloads card data from Scryfall and combo data from Commander Spellbook. This takes a few minutes, and the progress shows at the top right. After that it checks for new data every 12 hours, which is how new sets and ban list changes arrive without a new download of the app.

**Updating.** Quit Deck Advisor, download the new exe from [Releases](../../releases), and run it. Your decks and collection are kept separately from the exe, in `%LOCALAPPDATA%\DeckAdvisor`, so they carry over. To back them up, copy `%LOCALAPPDATA%\DeckAdvisor\data\deck-advisor.db` while the app is closed.

**Only download Deck Advisor from this repository's Releases page.** Copies from anywhere else aren't official and may have been tampered with.

## Privacy

Deck Advisor runs entirely on your computer. Your decks and collection never leave it, and there's no account, tracking or analytics. The app only goes online to download card data, combo data, premade deck lists and card images from the services credited below.

## Attributions and acknowledgments

Deck Advisor wouldn't be possible without these projects. Deck Advisor isn't affiliated with, approved by or endorsed by any of them.

- **[Scryfall](https://scryfall.com)**: card data, rules text, legalities, printings, prices, popularity ranking (EDHREC rank, as published by Scryfall) and **all card images**, downloaded from the Scryfall API and its bulk data files. Card images are shown as Scryfall serves them and remain the property of Wizards of the Coast. Following Scryfall's guidelines, Deck Advisor is free and doesn't put Scryfall data behind any paywall. Thank you to the Scryfall team for their outstanding free service.
- **[Commander Spellbook](https://commanderspellbook.com)**: the combo definitions (which cards combo, what each combo needs, and what it produces) that the app's combo detection is built on, from the Commander Spellbook API and bulk export. Thank you to the Commander Spellbook team and its community of contributors.
- **[MTGJSON](https://mtgjson.com)**: the lists of Wizards of the Coast's preconstructed decks shown on the Premade decks page.

All trademarks and data belong to their respective owners. Card data, combo data and images are used as their providers permit and are not covered by Deck Advisor's license.

## Fan Content Policy

Deck Advisor is unofficial Fan Content permitted under the Fan Content Policy. Not approved/endorsed by Wizards. Portions of the materials used are property of Wizards of the Coast. ©Wizards of the Coast LLC.

Magic: The Gathering, its card names, card images, mana symbols and other related marks are trademarks and property of Wizards of the Coast LLC. Read the [Wizards of the Coast Fan Content Policy](https://company.wizards.com/en/legal/fancontentpolicy).

## License

Deck Advisor is proprietary software, free for personal, non-commercial use under the terms in [LICENSE](LICENSE). By downloading, installing or using it, you agree to those terms. In short: use it, enjoy it, share the link to this page; don't resell it, redistribute the exe, or try to take it apart.

Copyright © 2026 Brian Squires. All rights reserved.
