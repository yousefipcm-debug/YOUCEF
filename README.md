# My System

Personal daily habit tracker & weekly planner — built as a PWA (Progressive Web App).

## Files

```
my-system/
├── index.html      ← Main app (single file, everything inside)
├── manifest.json   ← PWA manifest (app name, icons, theme)
├── sw.js           ← Service worker (offline support)
├── icon-192.png    ← App icon 192x192
├── icon-512.png    ← App icon 512x512
└── README.md       ← This file
```

## Deploy to GitHub Pages

1. **Create a new repo** on GitHub called `my-system`

2. **Push the files:**
```bash
cd my-system
git init
git add .
git commit -m "My System v1"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/my-system.git
git push -u origin main
```

3. **Enable GitHub Pages:**
   - Go to your repo → **Settings** → **Pages**
   - Source: **Deploy from a branch**
   - Branch: **main** / **root**
   - Click **Save**

4. **Your app is live at:** `https://YOUR_USERNAME.github.io/my-system/`

## Install as App on Phone

1. Open the URL in **Chrome** (Android) or **Safari** (iPhone)
2. Android: tap ⋮ menu → **"Add to Home Screen"**
3. iPhone: tap Share → **"Add to Home Screen"**
4. It will appear as a real app with the icon

## Features

- ✅ Daily checklist grouped by category (Spiritual, Fitness, Learning, Work, Daily Fixed)
- ⏰ Bounded tasks with start/end times + browser notifications
- 🔥 Overall streak tracking
- 📊 Weekly bar chart with best day highlight
- ➕ Add custom tasks with category, duration, and bounded/free type
- ⚙️ Editable habits (name, duration, days, bounded/free)
- 🕌 Prayer times display (manually set for Blida)
- 💾 All data saved in localStorage (offline, per browser)
- 📱 PWA — installable on phone as a real app
- 🌙 Dark mode
