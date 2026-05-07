# 🎬 TV Game Show Hub — College Edition

> Three Italian TV game shows reimagined in English. One file. No install. Just open and play.

**[▶ Play Now](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/)** — replace with your GitHub Pages link after setup.

---

## 🎮 The Three Games

### 🔵 Game 1 — Reverse Logic *(Avanti un Altro)*

Pick the **wrong** answer to advance. Picking the correct one resets you to Question 1 — while the timer and money keep running.

| Feature | Detail |
|---------|--------|
| Questions | **548** across geography, science, history, philosophy, literature, sport, music, cinema and more |
| Smart shuffle | Questions rarely repeat across consecutive rounds |
| Questions & answers | Locked for the entire session — same choices even after a reset or Freeze |
| Voice commands | Say the answer, **"A"** or **"B"**, **"Freeze"** to lock prize, **"Skip"** to defer |
| Voice matching | Fuzzy — works with partial or imperfect speech |
| Skips | **3 maximum** per round. Skip counter shown on screen. Disabled during Last Chance |
| Timer & money | Prize halved at 30s remaining, then −€1,000/sec |
| Freeze | Locks clock + prize. Return to questions for a **Last Chance** round — no timer, no skips, one wrong answer ends the game |
| Skipped questions | Dot turns yellow, question moves to end of queue. Returns at the end of the round |
| Win condition | Answer all 21 questions (always choosing the wrong option) to claim the prize |

### 🎙 Game 2 — The Duel *(L'Eredità)*

Two players race each other. Letters reveal one by one in random order every 2.5 seconds — but the last letter is **never revealed**. You must say the complete word to win.

| Feature | Detail |
|---------|--------|
| Words | **552** academic vocabulary words with definitions |
| Smart shuffle | Words rarely repeat across consecutive rounds |
| Microphone | Always on — say the word to win the round instantly |
| Letter hints | Stop when only 1 letter remains — player must still guess |
| Timers | Each player has an independent countdown ring. Only the active player's timer ticks |
| Winner | The player whose timer **runs out first loses**. Survive longest to win |
| Switching | Correct guess instantly switches to opponent. Press Next Word / Enter to skip |

### 🌊 Game 3 — Word Chain *(Reazione a Catena)*

Teams of 3: one guesser (blindfolded or facing away), two clue-givers who can see the word and give **one word each** as hints.

| Feature | Detail |
|---------|--------|
| Words | **511** words across every academic subject |
| Smart shuffle | Words rarely repeat across consecutive rounds |
| Correct | +1 point and +5 seconds added to the clock |
| Wrong | −1 point, no time penalty, next word loads |
| Pass | Skip freely — only **3 passes** per round, no penalty |
| Win | Highest score when time runs out wins |

---

## 🚀 How to Play

### Option A — Open the file directly *(easiest)*
Download `index.html` and double-click it. Done.

> **Voice recognition** requires **Google Chrome** or **Microsoft Edge**.  
> The browser asks for microphone permission once — never again after that.

### Option B — Play via GitHub Pages *(free permanent link, shareable with anyone)*

1. Create a free account at [github.com](https://github.com)
2. Click **+** → **New repository** → name it (e.g. `game-show-hub`) → set to **Public** → **Create repository**
3. Before uploading, **rename the file on your computer** from `game_show_hub.html` to **`index.html`**
4. Click **Add file → Upload files** → upload `index.html` and `README.md` → **Commit changes**
5. Go to **Settings → Pages → Source → Deploy from a branch → main / root → Save**
6. Wait ~60 seconds, refresh — your link is live:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

Share that link — anyone opens it in Chrome or Edge and plays immediately, no download needed.

---

## 🎙 Voice Commands — Game 1

| Say | Action |
|-----|--------|
| The answer text (or part of it) | Select that option |
| `"A"` | Select option A |
| `"B"` | Select option B |
| `"Freeze"` | Lock the prize and stop the clock |
| `"Skip"` | Defer the current question (max 3 per round) |

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `A` | Pick answer A (Game 1) |
| `B` | Pick answer B (Game 1) |
| `F` | Trigger Freeze (Game 1) |
| `Enter` | Start game from lobby / Next word (Game 2) |
| `→` | Correct (Game 3) |
| `←` | Wrong (Game 3) |
| `Space` | Pass (Game 3) |

---

## 🛠 Technical Details

| | |
|--|--|
| Format | Single self-contained HTML file (~215 KB) |
| Dependencies | None — no frameworks, no CDN, no build tools |
| Voice | Web Speech API — one permission request, stays live for the whole session |
| Audio | Web Audio API — all sounds synthesized in-browser, no audio files |
| Shuffle | Smart tracker pushes recently-seen items to the back of the pool |
| Storage | None — stateless, resets on page refresh |
| Browser support | Chrome 100+, Edge 100+ (voice); all browsers for non-voice gameplay |

---

## 📺 Based On

| This game | Italian original | Network |
|-----------|-----------------|---------|
| Reverse Logic | *Avanti un Altro* — hosted by Paolo Bonolis | Mediaset |
| The Duel | *L'Eredità* | RAI 1 |
| Word Chain | *Reazione a Catena* | RAI 1 |

---

## 📱 Install as an App (PWA)

This game is a **Progressive Web App** — it installs like a native app on any device.

**On iPhone / iPad (Safari):**
1. Open the GitHub Pages link in Safari
2. Tap the **Share** button → **Add to Home Screen**
3. Tap **Add** — the game appears on your home screen like any app

**On Android (Chrome):**
1. Open the link in Chrome
2. Tap the **⋮ menu** → **Add to Home Screen** (or look for the install banner)
3. Tap **Install** — it appears in your app drawer

**On Desktop (Chrome or Edge):**
1. Open the link
2. Click the **install icon** (⊕) in the address bar
3. Click **Install** — it opens as a standalone window with no browser UI

Once installed the game works **completely offline** — no internet needed after first load.

---

## 📁 Files

```
index.html     ← The entire game (rename from game_show_hub.html before uploading)
manifest.json  ← PWA manifest (app name, icon, display mode)
sw.js          ← Service worker (offline caching)
icon-192.png   ← App icon — home screen / app drawer
icon-512.png   ← App icon — splash screen / store listing
README.md      ← This file
```

All five files must be uploaded to the same GitHub repository folder for the PWA to work correctly.

---

*No frameworks. No server. No install needed. Open the link, install once, play forever — even offline.*
