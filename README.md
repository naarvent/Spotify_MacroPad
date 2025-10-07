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
   git clone https://github.com/yourusername/spotify-macropad.git
   cd spotify-macropad

2. **Install dependencies:**
   pip install spotipy keyboard

3. **Create an app on the Spotify Developer Dashboard**  
   - Copy your Client ID, Client Secret, and define a Redirect URI (for example, http://localhost:8888/callback).

4. **Edit the configuration:**
   Open spotify_macropad.py (or the English version) and replace:
   CLIENT_ID = "YOUR_CLIENT_ID"
   CLIENT_SECRET = "YOUR_CLIENT_SECRET"
   REDIRECT_URI = "YOUR_REDIRECT_URI"

5. **Run the script:**
   python spotify_macropad.py

   The first time you run it, a browser window will open asking for Spotify authorization.

---

## 🎹 Default Keybindings

### 🇪🇸 Spanish Version (spotify_macropad.py)
Key | Action
----|--------
Re Pag | Toggle active state
Av Pag | Play / Pause
↑ / ↓ | Volume up / down
← / → | Previous / Next track
Supr | Toggle shuffle
Right Shift | Change repeat mode
Inicio | Like / Unlike current track
Ç | Mute / Unmute

### 🇬🇧 English Version (spotify_macropad_en.py)
Key | Action
----|--------
Page Up | Toggle active state
Page Down | Play / Pause
↑ / ↓ | Volume up / down
← / → | Previous / Next track
Delete | Toggle shuffle
Right Shift | Change repeat mode
Home | Like / Unlike current track
Right Ctrl | Mute / Unmute

---

## 💾 File Structure

By default, the script creates the following directory in your user folder:
Documents/naarvent’s projects/SpotifyMacroPad/
 ├── .spotify_oauth_cache     (authentication data)
 └── track_history.txt        (track history)

---

## 🧩 Technical Details

- Built with Python 3.10+
- Requires Spotify Premium (for playback control via API)
- Uses keyboard for global key detection
- Logs playback history automatically
- Includes fallback logic when playback is inactive

---
