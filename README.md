# PokeBot 🎮

![License](https://img.shields.io/badge/License-AGPLv3-blue.svg)
![Version](https://img.shields.io/badge/Version-1.3.2-brightgreen.svg)
![.NET](https://img.shields.io/badge/.NET-9.0-purple.svg)
![Downloads](https://img.shields.io/github/downloads/PKM-Universe/PKM-Universe/total?style=flat-square&color=blue)

> **Professional-grade Pokémon trading automation for Nintendo Switch**
>
> Trade, clone, and distribute Pokémon with ease using this powerful automation system featuring a sleek web interface and comprehensive Discord integration.

---

## 🌟 What Makes This Special

PokeBot is a next-generation trading bot built from the ground up with:
- **Latest PKHeX Core** (v25.11.16-rev.5) - Always up to date
- **Modern .NET 9.0** - Fast and efficient
- **Beautiful Web Dashboard** - Control everything from your browser
- **Smart Queue System** - Handles trades intelligently
- **Complete Game Coverage** - From Legends Z-A to Let's Go

## 🚀 Getting Started

### What You Need
- **PC:** Windows 10/11 (64-bit)
- **Switch:** Custom Firmware with sys-botbase
- **Time:** 5 minutes to set up

### Installation in 3 Steps

1. **Download** the latest release from the [Releases](https://github.com/PKM-Universe/PKM-Universe/releases) page
2. **Extract** everything to a folder (like `C:\PokeBot`)
3. **Run** `PokeBot.exe` as Administrator

That's it! The setup wizard will guide you through the rest.

---

## 💻 Web Control Panel

Access your personal control center at **http://localhost:8080**

### What You Can Do:
- 📊 **Monitor** all your bots in real-time
- 🎮 **Control** your Switch remotely (virtual controller!)
- 📜 **View** live logs with instant search
- ⚡ **Manage** multiple bots at once
- 🔄 **Update** PKHeX with one click

### Mobile Access
Control your bots from your phone! Just open your browser to:
```
http://YOUR-PC-IP:8080
```

Perfect for monitoring trades while you're away from your desk.

---

## 🎯 Discord Trading Commands

### Quick Trade
```
.trade Pikachu
Level: 100
Shiny: Yes
Ability: Lightning Rod
```

### Popular Commands

| Command | What It Does |
|---------|-------------|
| `.trade` | Trade any Pokémon from a Showdown set |
| `.ditto` | Get a perfect 6IV Ditto in any language |
| `.clone` | Clone the Pokémon you show me |
| `.item` | Get any item delivered on a Pokémon |
| `.event` | Browse and request event Pokémon |
| `.battleready` | Get competitive-ready Pokémon |

### For Batch Trading
Trade up to 3 Pokémon at once:
```
.bt Pikachu
Shiny: Yes
---
Charizard
Shiny: Yes
---
Mewtwo
Shiny: Yes
```

---

## 🎮 Supported Pokémon Games

| Game | Status | Notes |
|------|--------|-------|
| Pokémon Legends Z-A | ✅ **Full Support** | Latest game! |
| Pokémon Scarlet/Violet | ✅ **Full Support** | Gen 9 ready |
| Pokémon Sword/Shield | ✅ **Full Support** | Gen 8 complete |
| Pokémon BD/SP | ✅ **Full Support** | Sinnoh remakes |
| Pokémon Legends: Arceus | ✅ **Full Support** | Special formats |
| Pokémon Let's Go | ✅ **Full Support** | Kanto classics |

---

## ⚙️ Configuration

### Switch Setup
1. Install **Atmosphere CFW** on your Switch
2. Install **sys-botbase** (get it from olliz0r's GitHub)
3. Find your Switch's IP address (Settings → Internet)
4. Enter the IP in PokeBot settings

### Discord Setup
1. Create a bot at [Discord Developer Portal](https://discord.com/developers/applications)
2. Copy your bot token
3. Paste it in the PokeBot settings
4. Invite your bot to your server

All settings are in `config.json` - easy to edit!

---

## 🛠️ Advanced Features

### Queue Management
- **Smart queuing** - Trades are handled in order
- **Priority system** - VIP users can skip the line
- **Position tracking** - Users always know where they are
- **Auto-cleanup** - Old trades are removed automatically

### Event Distribution
- **Hundreds of events** - From every generation
- **Legal checking** - All Pokémon are legal
- **Custom wondercards** - Import your own events
- **Battle-ready sets** - Competitive teams ready to go

### Safety Features
- **Advertisement detection** - Auto-fixes nicknamed Pokémon
- **Legal validation** - PKHeX integration ensures legality
- **Backup system** - All trades are logged
- **Error recovery** - Automatic retry on failures

---

## 📱 Remote Access Setup

Want to control your bot from anywhere on your network?

**Quick Setup:**
```cmd
# Open Command Prompt as Administrator and run:
netsh advfirewall firewall add rule name="PokeBot" dir=in action=allow protocol=TCP localport=8080
```

**Find Your IP:**
```cmd
ipconfig
```
Look for "IPv4 Address" (example: 192.168.1.100)

**Access From Any Device:**
Open any browser → `http://192.168.1.100:8080`

Now you can manage trades from your phone, tablet, or another computer!

---

## 🆘 Troubleshooting

### "Can't connect to my Switch"
- ✅ Is sys-botbase installed and active?
- ✅ Is your Switch on the same network as your PC?
- ✅ Did you enter the correct IP address?
- ✅ Is your Switch's screen on?

### "Discord bot shows offline"
- ✅ Did you copy the entire bot token?
- ✅ Did you enable "Message Content Intent" in Discord settings?
- ✅ Did you restart PokeBot after adding the token?

### "Web panel won't load"
- ✅ Did you run as Administrator the first time?
- ✅ Try `http://localhost:8080` first
- ✅ Check if Windows Firewall is blocking it

### "Antivirus is blocking PokeBot.exe"
This is a false positive. Add an exception for the PokeBot folder.

---

## 🔐 Security & Privacy

- **Your data stays local** - Nothing is sent to external servers
- **No telemetry** - We don't track your usage
- **Open source core** - Based on trusted SysBot.NET
- **Config encryption** - Your Discord token is protected

---

## 📊 Performance

PokeBot is optimized for speed:
- ⚡ **Fast trades** - Average 2-3 minutes per trade
- 🔄 **Multiple bots** - Run as many as you want
- 💾 **Low memory** - Uses ~100MB RAM per bot
- 🚀 **.NET 9.0** - Latest performance improvements

---

## 🎓 Learning Resources

New to trading bots? Check out these guides:
1. **QUICK_START.md** - Get running in 5 minutes
2. **config.json** - Detailed comments explain every setting
3. **Web Dashboard** - Built-in help for every feature

---

## 📜 License & Credits

### License
This project is licensed under **AGPL-3.0**. See the LICENSE file for full details.

### Built With
- **SysBot.NET** by kwsch - The foundation
- **PKHeX** - Pokémon editing and validation
- **Discord.Net** - Discord bot framework
- **sys-botbase** by olliz0r - Switch communication

### Disclaimer
⚠️ This software is for educational purposes. Use responsibly. The developer is not responsible for any consequences of using this software, including but not limited to console bans.

---

## 💬 Support & Community

Having issues? Want to share your setup?

- 📖 Read the docs in this repository
- 🐛 Report bugs in [Issues](https://github.com/PKM-Universe/PKM-Universe/issues)
- 💡 Request features in [Discussions](https://github.com/PKM-Universe/PKM-Universe/discussions)

---

## 🔄 Updates

**Current Version:** 1.3.2 (November 25, 2025)

Stay tuned for updates! ⭐ Star this repository to get notified.

---

<div align="center">

**PKM Universe PokeBot** - Making Pokémon Trading Easy

Powered by .NET 9.0 | Built for the Community

*Trade Smart. Trade Fast. Trade with PokeBot.*

</div>
