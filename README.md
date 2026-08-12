# Nyx Prime — Web

Browser build of **Nyx Prime** (SOETech) for testing while the Android APK is being fixed.

## Live URL
Hosted on GitHub Pages. See repo Settings → Pages, or the reported URL.

## Features
- **Chat** — send/receive messages, history persisted in localStorage
- **Memory** — store memories with tiers (EGO / CONSCIOUS / SUBCONSCIOUS), search, live stats (TOTAL, EGO, CONSCIOUS, SUBCON)
- **Tasks** — add tasks with priority + due date, toggle complete, delete
- **Settings** — system config + data source: Web (localStorage)
- Dark cyberpunk theme matching the Android app
- Data persists in the browser even after reload (localStorage)

## Run locally
Just open `index.html` in a browser, or serve with any static server:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Data model parity
Mirrors `com.soeteam.nyxprime.core.model`:
- `Memory` sealed class → `MemoryTier { EGO, CONSCIOUS, SUBCONSCIOUS }`
- `Task { title, priority (LOW/MEDIUM/HIGH/URGENT), status }`
- `ChatMessage { role (USER/ASSISTANT/SYSTEM) }`

---
© SOETech · Nyx Prime v1.0
