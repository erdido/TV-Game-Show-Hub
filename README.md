# 🎬 TV Game Show Hub — College Edition

A fully self-contained, single-file HTML web app that recreates three Italian TV game shows in English — no server, no install, no dependencies. Just open the file in any modern browser and play.

---

## 🎮 The Three Games

### 🔵 Game 1 — Reverse Logic *(Avanti un Altro)*
Pick the **wrong** answer to advance. Picking the correct one sends you straight back to Question 1.

- 21 questions per round, fixed for the entire session (same questions and same answer choices even after restarts or Freeze)
- Voice activated — say answers, **"Freeze"**, or **"Skip"** out loud
- Live prize pool that gets halved at 30s remaining, then drains €1,000/sec
- **Freeze** locks your prize and time; return for a **Last Chance** round with no timer and no skips
- Skipped questions (yellow LEDs) return at the end of the round

### 🎙 Game 2 — The Duel *(L'Eredità)*
Two players race each other on the same word. Letters reveal one by one in **random order** every 2.5 seconds.

- Microphone always on — say the word to win the round instantly
- Independent countdown timer per player (ring display)
- Points scale with how few letters were revealed when you guessed

### 🌊 Game 3 — Word Chain *(Reazione a Catena)*
Teams of 3: one guesser (blindfolded or facing away), two clue-givers who can see the word and give **one word each** as hints.

- **✓ Correct** → +1 point and +5 seconds on the clock
- **✗ Wrong** → −1 point, no time penalty
- **PASS** → skip freely, 3 passes per round
- Authentic *Reazione a Catena* blue TV-style interface

---

## 🚀 How to Run

### Option A — Open directly in browser (easiest)
```
Just double-click game_show_hub.html
```
No server needed. Works in Chrome, Edge, Firefox, Safari.

> **Voice recognition** (Games 1 & 2) requires **Google Chrome** or **Microsoft Edge** — the Web Speech API is not supported in Firefox/Safari.  
> The browser will ask for microphone permission once on first use.

### Option B — Serve locally (if you want a URL)
```bash
# Python 3
python -m http.server 8080

# Node.js (npx)
npx serve .

# Then open: http://localhost:8080/game_show_hub.html
```

### Option C — Host on GitHub Pages (free, shareable link)
1. Create a new GitHub repository
2. Upload `game_show_hub.html` and rename it to `index.html`
3. Go to **Settings → Pages → Source → main branch / root**
4. Your game is live at `https://yourusername.github.io/your-repo-name/`

---

## 🎙 Voice Commands (Game 1)

| Say | Action |
|-----|--------|
| `"A"` or the answer text | Select option A |
| `"B"` or the answer text | Select option B |
| `"Freeze"` | Lock prize and timer |
| `"Skip"` | Skip to next question |

Voice recognition requires Chrome/Edge and microphone permission.

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `A` | Pick answer A (Game 1) |
| `B` | Pick answer B (Game 1) |
| `F` | Trigger Freeze (Game 1) |
| `Enter` | Start game (lobby) / Next word (Game 2) |
| `→` | Correct (Game 3) |
| `←` | Wrong (Game 3) |
| `Space` | Pass (Game 3) |

---

## 🛠 Technical Details

- **Single file** — 100% self-contained HTML + CSS + JavaScript, no external dependencies
- **Web Speech API** — continuous voice recognition, permission requested once
- **Web Audio API** — all sounds synthesized in-browser (tick, ding, buzzer, victory, defeat, tense music)
- **No localStorage / no cookies** — stateless, resets on page refresh
- Tested on Chrome 120+, Edge 120+

---

## 📁 Files

```
game_show_hub.html   ← The entire game (open this)
README.md            ← This file
```

---

## 📺 Based On

| This game | Italian original |
|-----------|-----------------|
| Reverse Logic | *Avanti un Altro* (Mediaset, hosted by Paolo Bonolis) |
| The Duel | *L'Eredità* (RAI 1) |
| Word Chain | *Reazione a Catena* (RAI 1) |

---

*Built as a single-file web app. No frameworks, no build tools, no installation.*
