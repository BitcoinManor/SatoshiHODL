# 🎮 Satoshi HODL

HODL through chaos. Stack sats. Don’t get rekt.
A tiny browser game built with plain HTML/CSS/JS.

Play in your browser:
https://bitcoinmanor.github.io/SatoshiHODL/

---

## 🚀 Quick Deploy (GitHub Pages)

One-time setup (Option C)

1) Rename files (clean URLs + Pages-friendly):
   - "Satoshi's HODL.html"  →  index.html
   - "Satoshi HODL.js"      →  game.js
   - In index.html, update the script tag to:
       <script src="./game.js"></script>

2) Commit & push to your default branch (usually main):
       git add -A
       git commit -m "feat: Pages-ready rename (index.html, game.js)"
       git push

3) Enable GitHub Pages:
   - Repo → Settings → Pages → Build and deployment
   - Source: Deploy from a branch
   - Branch: main (or master)
   - Folder: / (root)

4) Wait for the green check, then play here:
   https://bitcoinmanor.github.io/SatoshiHODL/

Tip: Prefer keeping the original filename? Put the game in a /docs folder and enable Pages from /docs. Your game will live at the same URL base.

---

## 🗂 Project Structure

After the Option-C rename, your repo should look like this:

SatoshiHODL/
├─ index.html            # entry point (was "Satoshi's HODL.html")
├─ game.js               # game logic (was "Satoshi HODL.js")
├─ styles.css            # UI styles
├─ assets/
│  ├─ images/
│  │  ├─ satoshi_background2.png
│  │  ├─ Satoshi_FG_pic.png
│  │  ├─ Satoshi_Green_Candle.png
│  │  ├─ Satoshi_Red_Candle.png
│  │  └─ Satoshi_Bitcoin_2.png
│  └─ audio/
│     ├─ themeMusic2.mp3
│     ├─ NumberGoUp.mp3
│     └─ earnasatoshi.mp3
├─ LICENSE
└─ README.md

Note: Filenames are case-sensitive on the web. If yours differ, keep the same folder layout and update paths in index.html.

---

## 🧪 Run Locally (dev/testing)

Option A: double-click index.html to open in your browser

Option B: serve locally (avoids some browser security quirks)

Python 3:
    python3 -m http.server 8080
Then open:
    http://localhost:8080/

Node (no install to the repo):
    npx http-server -p 8080

---

## 🕹️ How to Play

- Load the page and… HODL.
- Survive price swings, grab sats, avoid bad candles.
- If audio doesn’t start, click/tap once (browsers block autoplay without interaction).

Controls:
- Desktop: Arrow keys / WASD (if implemented), Space to start/restart.
- Mobile: Tap screen (simple interactions).
  Tip: Add a “Start” button for mobile to guarantee audio unlocks.

---

## 🛠 Tech

- HTML5 for structure
- CSS3 for styling (styles.css)
- Vanilla JavaScript for game loop & events (game.js)
- Audio: .mp3 via HTMLAudioElement
- No frameworks — super portable and easy to host

---

## 📦 Assets & Performance Tips

- Optimize PNGs (TinyPNG / ImageOptim) and MP3s (128–160 kbps is fine)
- Keep total page weight under ~2–3 MB for snappy loads
- Consider power-of-two sprite dimensions if you later move to WebGL/canvas

---

## 📸 Screenshot

Add a screenshot/gif for the README:
    <img alt="Satoshi HODL gameplay" src="./screenshot.png" width="900">

---

## 🗺️ Roadmap Ideas

- Mobile-first layout + larger tap targets
- Difficulty levels / waves
- Mute toggle & volume slider
- High-score persistence (localStorage)
- Pause / Resume
- Particle effects (CSS or canvas)

---

## 🤝 Contributing

PRs welcome! Cleanups, bug fixes, small features, and docs improvements all appreciated.

---

## 📝 License

GPL-3.0 — see LICENSE.

