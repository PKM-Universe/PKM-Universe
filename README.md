# Eric's PokeBot

![License](https://img.shields.io/badge/License-AGPLv3-blue.svg)

A powerful Pokémon trading automation system based on SysBot.NET for remote control of Nintendo Switch consoles.

## Features

- **Web-based Control Panel** - Control all your bots via `http://localhost:8080`
- **Discord Bot Integration** - Full Discord command support for trading
- **Multi-Game Support** - Legends Z-A, Scarlet/Violet, Sword/Shield, BDSP, PLA, LGPE
- **Real-time Queue Management** - Track trades from request to completion
- **Event & Battle-Ready Distribution** - Automated distribution of event and competitive Pokémon
- **Clone, Dump, and Trade** - Full PKHeX integration for genning and trading
- **Remote Switch Control** - Control your Nintendo Switch directly from the web interface
- **Automatic Updates** - Keep PKHeX/ALM libraries up to date with one click

## Quick Start

### Requirements
- Windows 10/11 (64-bit)
- Nintendo Switch with CFW (Atmosphere + sys-botbase)
- .NET 9.0 Runtime (included in release)

### Installation

1. Download the latest release
2. Extract all files to a folder
3. Run `PokeBot.exe` as Administrator (first time only, for network access)
4. Configure your Switch IP address and Discord bot token in `config.json`

### First Time Setup

1. **Configure Switch Connection**
   - Open PokeBot
   - Go to Settings
   - Enter your Switch IP address
   - Test connection

2. **Configure Discord Bot**
   - Create a Discord bot at https://discord.com/developers/applications
   - Copy the bot token
   - Paste it in `config.json` under `DiscordSettings.Token`
   - Invite the bot to your server

3. **Set Up Permissions**
   - Configure role permissions in `config.json`
   - Set which roles can use trade, clone, dump, and fixOT commands

### Network Access (Mobile/Remote Control)

To access the control panel from your phone or other devices on your network:

1. **Allow through firewall:**
   ```cmd
   netsh advfirewall firewall add rule name="PokeBot Web" dir=in action=allow protocol=TCP localport=8080
   ```

2. **Find your PC's IP:**
   ```cmd
   ipconfig
   ```
   Look for "IPv4 Address" (e.g., 192.168.1.100)

3. **Connect from any device:**
   Open browser and go to `http://YOUR-PC-IP:8080`

## Discord Commands

### Core Trading Commands

| Command | Description | Usage |
|---------|-------------|-------|
| `.trade` or `.t` | Trade a Pokémon from Showdown set or file | `.trade [code] <showdown_set>` |
| `.hidetrade` or `.ht` | Trade without showing details | `.ht [code] <showdown_set>` |
| `.batchTrade` or `.bt` | Trade up to 3 Pokémon at once | `.bt <sets_separated_by_--->` |
| `.egg` | Trade an egg | `.egg [code] <pokemon_name>` |

### Specialized Commands

| Command | Description | Usage |
|---------|-------------|-------|
| `.dittoTrade` or `.dt` | Get a perfect Ditto | `.dt [code] <stats> <language> <nature>` |
| `.itemTrade` or `.it` | Get Pokémon holding an item | `.it [code] <item_name>` |
| `.mysteryegg` or `.me` | Random perfect IV egg | `.me [code]` |
| `.clone` or `.c` | Clone your Pokémon | `.clone [code]` |
| `.dump` or `.d` | Dump your Pokémon to file | `.dump [code]` |

### Event Commands

| Command | Description | Usage |
|---------|-------------|-------|
| `.listevents` or `.le` | List available events | `.le [filter] [pageX]` |
| `.eventrequest` or `.er` | Request event by index | `.er <index>` |
| `.battlereadylist` or `.brl` | List battle-ready files | `.brl [filter]` |
| `.battlereadyrequest` or `.brr` | Request battle-ready by index | `.brr <index>` |

### Queue Commands

| Command | Description | Usage |
|---------|-------------|-------|
| `.tradeList` or `.tl` | View trade queue | `.tl` |
| `.medals` or `.ml` | View your trade stats | `.ml` |

## Control Panel Features

- **Real-time Bot Status** - Monitor all your bots at once
- **Batch Operations** - Start/Stop/Idle all bots with one click
- **Remote Control** - Virtual Switch controller in your browser
- **Live Logs** - Search and filter bot logs in real-time
- **Screen Control** - Turn Switch screens on/off remotely
- **Update Manager** - One-click updates for PKHeX and ALM

## Configuration

Edit `config.json` to customize:
- Discord bot token and channels
- Switch IP addresses
- Role permissions
- Trade settings
- Queue limits
- And much more...

## Supported Games

- ✅ Pokémon Legends Z-A (PLZA)
- ✅ Pokémon Scarlet/Violet (SV)
- ✅ Pokémon Sword/Shield (SWSH)
- ✅ Pokémon Brilliant Diamond/Shining Pearl (BDSP)
- ✅ Pokémon Legends: Arceus (PLA)
- ✅ Pokémon Let's Go Pikachu/Eevee (LGPE)

## Troubleshooting

### Bot won't connect to Switch
- Verify Switch IP is correct
- Ensure sys-botbase is installed and running
- Check firewall settings

### Discord bot is offline
- Verify bot token is correct in config.json
- Check bot has proper permissions in your server
- Ensure bot is invited with correct scopes

### Web panel won't load
- Run as Administrator first time
- Check firewall allows port 8080
- Try `http://localhost:8080` first

## Credits

Based on [SysBot.NET](https://github.com/kwsch/SysBot.NET) by kwsch

## License

This project is licensed under AGPL-3.0 - see the LICENSE file for details.

## Disclaimer

This software is intended for educational purposes. Use at your own risk. The developers are not responsible for any bans or issues that may arise from using this software.

---

**Version:** 1.0.0
**Build Date:** November 25, 2025
**Built by:** Eric
