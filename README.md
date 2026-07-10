# Bingo Caller

A self-contained, phone-friendly bingo number caller — spinning ball animation,
roulette-style sound, male/female voice call-outs, and a light/dark theme toggle.

No build step, no dependencies to install. It's just static files.

## Get it live on GitHub Pages (free, ~2 minutes)

1. **Create a new repository**
   - Go to [github.com/new](https://github.com/new)
   - Name it anything, e.g. `bingo-caller`
   - Keep it **Public** (required for free GitHub Pages)
   - Click **Create repository**

2. **Upload these files**
   - On your new repo's page, click **Add file → Upload files**
   - Drag in all the files from this folder:
     - `index.html`
     - `manifest.json`
     - `icon-192.png`
     - `icon-512.png`
     - `apple-touch-icon.png`
   - Click **Commit changes**

3. **Turn on GitHub Pages**
   - In your repo, go to **Settings → Pages** (left sidebar)
   - Under "Build and deployment" → **Source**, choose **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)` → **Save**
   - Wait ~30–60 seconds. Refresh the page — GitHub will show you a live URL like:
     `https://yourusername.github.io/bingo-caller/`

4. **Open that URL on your iPhone**
   - Open it in **Safari** (not another browser app, for best iOS speech-voice support)
   - Everything should now work fully: dark/light toggle, sound, and voice —
     since it's a real hosted webpage, not a local file preview.

5. **(Optional) Add it to your Home Screen**
   - In Safari, tap the **Share** icon → **Add to Home Screen**
   - It'll launch full-screen like a normal app, using the icon included in this package.

## Why this fixes the earlier mobile issues

Opening an `.html` file directly from the Files app on iOS often triggers
**Quick Look**, a restricted preview mode that doesn't run JavaScript and
overrides page styling. Hosting it as a real URL (via GitHub Pages) opens it
as an actual webpage in Safari, where everything — theme switching, the
Web Audio sound effects, and `speechSynthesis` voice call-outs — works as
intended.

## Files in this package

| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML/CSS/JS in one file) |
| `manifest.json` | Lets it install as a standalone app icon on your Home Screen |
| `icon-192.png`, `icon-512.png` | App icons for the manifest |
| `apple-touch-icon.png` | iOS-specific Home Screen icon |
