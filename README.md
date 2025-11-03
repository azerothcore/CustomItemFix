# CustomItemFix

A World of Warcraft addon that fixes the display issue where custom items show a question mark icon instead of their proper texture. This addon is designed for WoW 2.4.3 (The Burning Crusade) and is particularly useful for players on private servers with custom items.

## What It Does

CustomItemFix automatically detects and replaces question mark icons on custom items with their correct textures throughout the game interface. It fixes icons in:

- **Inventory/Bags**: Displays proper icons for custom items in your bags and containers
- **Action Bars**: Shows correct icons when custom items are placed on action bars
- **Bank**: Fixes item icons in your bank and bank bags
- **Equipment**: Displays proper textures for equipped custom items
- **Spellbook**: Fixes attack/auto-shot icons to show your weapon textures instead of question marks
- **Tooltips & Dragging**: Ensures proper textures when hovering over or dragging custom items

The addon works by hooking into the game's UI functions and retrieving the correct item texture information from the server, even when the client doesn't have the texture information cached locally.

## Features

- **Automatic Detection**: No configuration needed - the addon automatically finds and fixes all custom items
- **Real-time Updates**: Icons are updated dynamically as you interact with items
- **Lightweight**: Minimal performance impact using secure function hooks
- **Auto-equip Support**: Enables right-clicking custom armor/weapons in bags to auto-equip them
- **Comprehensive Coverage**: Fixes icons across all major UI elements where items appear

## Installation

### Method 1: Manual Installation

1. Download the latest release or clone this repository
2. Locate your World of Warcraft installation directory
3. Navigate to the `Interface\AddOns\` folder
   - Example: `C:\Program Files\World of Warcraft\Interface\AddOns\`
4. Copy the `CustomItemFix` folder into the `AddOns` directory
5. Launch World of Warcraft
6. At the character selection screen, click "AddOns" and ensure CustomItemFix is checked/enabled
7. Log in to your character - you should see the message: "Display IDs Fixer by Ethos Loaded Successfully!" in orange text

### Method 2: Git Clone

```bash
cd "C:\Program Files\World of Warcraft\Interface\AddOns\"
git clone https://github.com/azerothcore/CustomItemFix.git
```

### Verifying Installation

Once installed correctly, you should:
- See the success message in your chat window when logging in
- Notice that custom items in your bags now display their proper icons instead of question marks
- Be able to use custom items on action bars with correct icons

## Compatibility

- **Game Version**: World of Warcraft 2.4.3 (The Burning Crusade)
- **Interface Version**: 20400
- **Server Type**: Works best with private servers (like AzerothCore) that have custom items

## Troubleshooting

**Issue**: Addon doesn't load
- Make sure the folder is named exactly `CustomItemFix` (case-sensitive)
- Check that the folder is in the correct `Interface\AddOns\` directory
- Enable the addon from the AddOns menu at character select

**Issue**: Icons still show question marks
- Ensure the server supports proper item information retrieval
- Try reloading the UI with `/reload` command
- Some items may still show question marks if the server hasn't configured them properly

## Credits

**Original Author**: Ethos (2008)

Special thanks to:
- Ona for inspiration
- Halestorm for bug reporting and support
- The WoW addon development community

## License

Copyright (c) 2008 by Ethos.

Permission is granted to copy, distribute and/or modify this document under the terms of the GNU Free Documentation License, Version 1.2 or any later version published by the Free Software Foundation with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.

## Contributing

This project is maintained by the AzerothCore community. If you find bugs or have improvements, please submit issues or pull requests to the repository.

## Related Projects

- [AzerothCore](https://github.com/azerothcore/azerothcore-wotlk) - The open-source WoW server emulator
