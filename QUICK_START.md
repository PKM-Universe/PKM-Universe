# Quick Start Guide - Eric's PokeBot

Get up and running in 5 minutes!

## Step 1: Download & Extract (1 min)

1. Download `EricPokeBot-v1.0.0.zip`
2. Extract to `C:\PokeBot` (or anywhere you like)
3. You should see `PokeBot.exe` and many DLL files

## Step 2: First Run (1 min)

1. Right-click `PokeBot.exe` → **Run as Administrator**
2. Click "Allow" when Windows Firewall prompts appear
3. The application will start and create a `config.json` file

## Step 3: Configure Switch (2 mins)

### On your Switch:
1. Ensure you have **Atmosphere CFW** installed
2. Install **sys-botbase** (download from olliz0r/sys-botbase)
3. Reboot Switch with CFW
4. Find your Switch IP:
   - System Settings → Internet → Connection Status
   - Note the IP (e.g., `192.168.1.50`)

### In PokeBot:
1. Click **Settings** (or Hub tab)
2. Find "IP" field
3. Enter your Switch IP address
4. Click **Test Connection**
5. You should see "✅ Connected!"

## Step 4: Configure Discord (1 min - Optional)

### Create Discord Bot:
1. Go to https://discord.com/developers/applications
2. Click "New Application"
3. Name it (e.g., "Eric's PokeBot")
4. Go to "Bot" tab
5. Click "Reset Token" → Copy the token
6. Enable these under "Privileged Gateway Intents":
   - Server Members Intent
   - Message Content Intent

### In config.json:
1. Open `config.json` in Notepad
2. Find `"Token":` under Discord settings
3. Paste your bot token between the quotes
4. Save the file
5. Restart PokeBot

### Invite Bot to Server:
1. In Discord Developer Portal → OAuth2 → URL Generator
2. Select scopes: `bot`, `applications.commands`
3. Select permissions: `Send Messages`, `Embed Links`, `Attach Files`, `Use Slash Commands`
4. Copy the URL and open in browser
5. Select your server and authorize

## Step 5: Start Trading!

### From Discord:
```
.trade Pikachu
Level: 100
Shiny: Yes
```

### From Web Panel:
1. Open browser to `http://localhost:8080`
2. Navigate to your bot
3. Click "Start"
4. Monitor trades in real-time!

## Common Issues

### "Can't connect to Switch"
- ✅ Is sys-botbase installed?
- ✅ Is Switch on CFW?
- ✅ Is IP address correct?
- ✅ Are both on same network?

### "Discord bot offline"
- ✅ Is token correct in config.json?
- ✅ Did you restart PokeBot after adding token?
- ✅ Did you enable Privileged Intents?

### "Web panel won't load"
- ✅ Did you run as Administrator first time?
- ✅ Did you allow firewall access?
- ✅ Try `http://localhost:8080` first

### "Antivirus blocking PokeBot.exe"
- This is a false positive
- Add exception for PokeBot folder
- Or temporarily disable antivirus during first run

## Next Steps

- 📖 Read full [README.md](README.md) for all commands
- 🎮 Configure which games to support
- 👥 Set up Discord role permissions
- 📱 Enable mobile access (see README)
- 📊 Check out the web dashboard features

## Need Help?

- Check [RELEASE_NOTES.md](RELEASE_NOTES.md) for detailed info
- Review config.json comments for all settings
- Make sure sys-botbase is properly installed on Switch

---

**Happy Trading!** 🎮✨

Built by Eric | Powered by SysBot.NET & PKHeX
