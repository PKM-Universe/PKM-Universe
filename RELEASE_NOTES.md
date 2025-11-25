# Eric's PokeBot - Release Notes

## Version 1.0.0 - Initial Release
**Release Date:** November 25, 2025

### What's Included

This is the first official release of Eric's PokeBot, a comprehensive Pokémon trading automation system.

### 📦 Download

**File:** `EricPokeBot-v1.0.0.zip` (24 MB)

**What's in the package:**
- PokeBot.exe - Main application
- All required DLL dependencies
- PKHeX.Core.dll (v25.11.16) - Latest PKHeX integration
- Discord.Net libraries for bot functionality
- Configuration template

### ✨ Key Features

#### Web Control Panel
- Access via `http://localhost:8080`
- Real-time bot status monitoring
- Virtual Switch remote control
- Live log viewer with search
- Batch operations (Start/Stop/Idle all)
- One-click updates for PKHeX/ALM

#### Discord Integration
- Full command support for trading
- Queue management system
- Event Pokémon distribution
- Battle-ready Pokémon library
- Clone, dump, and trade commands
- User statistics and medals
- Role-based permissions

#### Multi-Game Support
- ✅ Pokémon Legends Z-A (PLZA)
- ✅ Pokémon Scarlet/Violet (SV)
- ✅ Pokémon Sword/Shield (SWSH)
- ✅ Pokémon Brilliant Diamond/Shining Pearl (BDSP)
- ✅ Pokémon Legends: Arceus (PLA)
- ✅ Pokémon Let's Go Pikachu/Eevee (LGPE)

### 🎮 Discord Commands

**Trading:**
- `.trade` / `.t` - Trade Pokémon from Showdown set
- `.hidetrade` / `.ht` - Private trade without embed
- `.batchTrade` / `.bt` - Trade up to 3 Pokémon
- `.egg` - Trade eggs
- `.dittoTrade` / `.dt` - Get perfect Ditto
- `.itemTrade` / `.it` - Get items

**Utilities:**
- `.clone` / `.c` - Clone your Pokémon
- `.dump` / `.d` - Dump Pokémon to file
- `.fixOT` / `.fix` - Fix OT/nickname

**Events:**
- `.listevents` / `.le` - Browse events
- `.eventrequest` / `.er` - Request event
- `.battlereadylist` / `.brl` - Browse competitive sets
- `.battlereadyrequest` / `.brr` - Request battle-ready

**Queue:**
- `.tradeList` / `.tl` - View queue
- `.medals` / `.ml` - View your stats

### 🔧 System Requirements

**Minimum:**
- Windows 10/11 (64-bit)
- .NET 9.0 Runtime (included)
- 100 MB free disk space
- Internet connection

**For Trading:**
- Nintendo Switch with Custom Firmware (Atmosphere)
- sys-botbase installed on Switch
- Local network connection to Switch

**For Discord:**
- Discord bot token
- Discord server with proper permissions

### 📋 Installation Steps

1. **Download** `EricPokeBot-v1.0.0.zip`
2. **Extract** all files to a folder (e.g., `C:\PokeBot`)
3. **Run** `PokeBot.exe` as Administrator (first time)
4. **Configure** your Switch IP and Discord token in settings
5. **Test** connection to your Switch
6. **Start** trading!

### 🌐 Network Access Setup

To access from mobile or other devices:

```cmd
# Allow through firewall
netsh advfirewall firewall add rule name="PokeBot Web" dir=in action=allow protocol=TCP localport=8080

# Find your IP
ipconfig
```

Then access from any device: `http://YOUR-PC-IP:8080`

### ⚙️ Configuration

The `config.json` file includes:
- Discord bot settings
- Switch IP addresses
- Role permissions
- Trade settings
- Queue limits
- Logging options

### 🐛 Known Issues

None reported in this initial release.

### 📝 Notes

- First run requires Administrator privileges for network setup
- Ensure sys-botbase is running on your Switch before connecting
- Discord bot token must be configured for Discord features
- Some antivirus software may flag the executable (false positive)

### 🙏 Credits

- **SysBot.NET** by kwsch - Original framework
- **PKHeX** - Pokémon editing core
- **Discord.Net** - Discord integration
- **sys-botbase** by olliz0r - Switch communication

### 📜 License

This project is licensed under AGPL-3.0. See LICENSE file for details.

### ⚠️ Disclaimer

This software is for educational purposes only. Use at your own risk. The author is not responsible for any bans or issues resulting from use of this software.

### 🔜 Future Plans

- Automatic queue balancing across multiple bots
- Enhanced mobile UI
- Additional game support
- Custom event creation tools
- Advanced statistics dashboard

---

**Built with:** .NET 9.0
**PKHeX Version:** 25.11.16-rev.5
**Build Date:** November 25, 2025
**Release by:** Eric

🤖 Generated with [Claude Code](https://claude.com/claude-code)
