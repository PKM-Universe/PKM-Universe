# How to Upload Eric's PokeBot to GitHub

Follow these steps to create your own GitHub repository with releases, just like hexbyt3/PokeBot!

## Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. **Repository name:** `EricPokeBot` (or your preferred name)
3. **Description:** "Professional Pokémon trading bot for Nintendo Switch - Discord integration, web control panel, multi-game support"
4. **Visibility:** Public (or Private if preferred)
5. **Do NOT** initialize with README (we already have one)
6. Click **"Create repository"**

## Step 2: Connect Local Repository to GitHub

GitHub will show you commands. Use these in Git Bash or Command Prompt:

```bash
cd "C:\Users\ericr\OneDrive\Desktop\EricPokeBot-Release"

# Add the remote repository (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/EricPokeBot.git

# Push your code
git branch -M main
git push -u origin main
```

**Example:**
```bash
git remote add origin https://github.com/EricR/EricPokeBot.git
git branch -M main
git push -u origin main
```

You'll be prompted for your GitHub credentials.

## Step 3: Create a Release

### Option A: Via GitHub Website (Easiest)

1. Go to your repository on GitHub
2. Click **"Releases"** on the right sidebar
3. Click **"Create a new release"**
4. Click **"Choose a tag"** → Type `v1.0.0` → Click "Create new tag: v1.0.0"
5. **Release title:** `v1.0.0 - Initial Release`
6. **Description:** Copy and paste from `RELEASE_NOTES.md`
7. **Attach binaries:**
   - Drag and drop `C:\Users\ericr\OneDrive\Desktop\EricPokeBot-v1.0.0.zip`
   - The file will upload (24 MB)
8. Check **"Set as the latest release"**
9. Click **"Publish release"**

### Option B: Via Command Line (Advanced)

Install GitHub CLI first: https://cli.github.com/

```bash
# Create a tag
git tag -a v1.0.0 -m "Initial release of Eric's PokeBot"
git push origin v1.0.0

# Create release with GitHub CLI
gh release create v1.0.0 \
  "C:\Users\ericr\OneDrive\Desktop\EricPokeBot-v1.0.0.zip" \
  --title "v1.0.0 - Initial Release" \
  --notes-file RELEASE_NOTES.md
```

## Step 4: Customize Your Repository

### Add a Description
1. Click the ⚙️ (gear icon) near the top right
2. Add description: "Professional Pokémon trading bot for Nintendo Switch"
3. Add topics (tags): `pokemon`, `trading-bot`, `discord-bot`, `sysbot`, `switch`, `automation`
4. Save changes

### Add a Website (Optional)
If you want to add a link to your Discord or website:
1. Same settings page
2. Website field
3. Add your Discord invite: `https://discord.gg/YOUR-INVITE`

### Create a Banner (Optional)
Add a cool banner image to your README:
1. Create or find a banner image (1280x640 recommended)
2. Upload to GitHub Issues (drag and drop)
3. Copy the URL
4. Add to top of README.md:
```markdown
![Banner](https://github.com/user-attachments/assets/YOUR-IMAGE-URL)
```

## Step 5: Add Download Badge

Add this to your README.md to show download count:

```markdown
![Downloads](https://img.shields.io/github/downloads/YOUR-USERNAME/EricPokeBot/total?style=flat-square&color=blue)
```

## Your Release is Live! 🎉

People can now:
- ⭐ Star your repository
- 👀 Watch for updates
- 🍴 Fork for their own modifications
- 📥 Download releases from the Releases page
- 🐛 Report issues
- 💬 Discuss in Discussions (if enabled)

## Future Releases

When you have updates:

1. Make your changes to the source code
2. Build a new release
3. Update version in README.md and RELEASE_NOTES.md
4. Create new zip file (e.g., `EricPokeBot-v1.1.0.zip`)
5. Commit changes:
   ```bash
   git add .
   git commit -m "Release v1.1.0: Added new features"
   git push
   ```
6. Create new tag and release:
   ```bash
   git tag -a v1.1.0 -m "Version 1.1.0"
   git push origin v1.1.0
   ```
7. Create GitHub release for v1.1.0 and upload new zip

## Promote Your Release

Share your repository:
- 🎮 Discord servers
- 📱 Reddit (r/PokemonROMhacks, r/SwitchHacks)
- 🐦 Twitter/X
- 📺 YouTube tutorials

---

**Your repository will look just like hexbyt3/PokeBot!** 🚀

Need help? Check GitHub's documentation: https://docs.github.com/
