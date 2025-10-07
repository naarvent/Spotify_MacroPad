# 🎧 Spotify MacroPad

A **Python** script that lets you control Spotify using keyboard shortcuts.  
It allows you to play/pause, skip tracks, adjust volume, toggle shuffle or repeat, like songs, mute/unmute — all without leaving your current app.

There are **two versions**:
- 🇪🇸 `spotify_macropad.py` → for **Spanish** keyboard layout.  
- 🇬🇧 `spotify_macropad_en.py` → for **English** keyboard layout.

---

## 🧠 What It Does

Spotify MacroPad turns your keyboard into a control panel for Spotify.  
When active, it listens for specific keys and sends commands to Spotify via the **official Spotify Web API** (using [Spotipy](https://spotipy.readthedocs.io/)).

Main features:
- ▶️ Play / Pause  
- ⏭️ Next track  
- ⏮️ Previous track (or restart if within 3 seconds)  
- 🔊 Volume up / down  
- 🔁 Cycle repeat mode  
- 🔀 Toggle shuffle  
- ❤️ Like / Unlike current song  
- 🔇 Mute / Unmute  
- 🔘 Toggle active state (enable/disable script)

---

## ⚙️ Installation

1. **Clone the repository or download the files:**
   ```bash
   git clone https://github.com/yourusername/spotify-macropad.git
   cd spotify-macropad
