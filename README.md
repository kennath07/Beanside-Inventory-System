# Beanside Coffee — Inventory PWA

## Deploy to GitHub Pages (Step-by-step)

### 1. Create GitHub Repo
1. Go to https://github.com
2. Click **New repository**
3. Name it: `beanside-inventory`
4. Set to **Public**
5. Click **Create repository**

### 2. Upload Files
Upload all these files to the repo:
- `index.html`
- `manifest.json`
- `sw.js`
- `icon-192.png`
- `icon-512.png`

Click **Add file > Upload files**, drag all 5 files, then **Commit changes**.

### 3. Enable GitHub Pages
1. Go to repo **Settings**
2. Click **Pages** (left sidebar)
3. Under **Source**, select `main` branch, folder `/ (root)`
4. Click **Save**
5. Wait ~1 minute. Your URL will be: `https://YOUR_USERNAME.github.io/beanside-inventory/`

### 4. Fix Service Worker Path
After deploying, open `sw.js` and update the start_url in `manifest.json`:
- Change `"start_url": "/"` to `"start_url": "/beanside-inventory/"`

### 5. Install on Android Tablet
1. Open Chrome on tablet
2. Go to your GitHub Pages URL
3. Tap the **three dots (⋮)** menu
4. Tap **"Add to Home screen"**
5. Tap **Add**

App now works offline. Data saved on tablet only.

---
## Features
- 📦 Stock view with search + category filters
- ✏️ Manual stock adjustment with notes
- 🔴 Low/Critical stock alerts
- 📋 End-of-day report (screenshot-ready)
- 🕑 Activity log (last 200 entries)
- 📴 Fully offline after first load
