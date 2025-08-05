# Spotify MacroPad

A Python script that turns your keyboard into a MacroPad for controlling Spotify. Press designated keys to control playback, volume, shuffle, repeat, like/unlike, and mute.

---

## 📦 Requirements

- Python 3.7 or higher
- [spotipy](https://pypi.org/project/spotipy/)
- [keyboard](https://pypi.org/project/keyboard/)
- A Spotify Developer account (Client ID & Client Secret)

---

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/naarvent/Spotify_MacroPad.git
   cd Spotify_MacroPad
   ```
2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate    # Linux/macOS
   venv\Scripts\activate     # Windows
   ```
3. Install dependencies:
   ```bash
   pip install spotipy keyboard
   ```

---

## ⚙ Configuration

1. Create a Spotify application at the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).
2. Copy your **Client ID** and **Client Secret**.
3. In `spotify_macropad.py`, update the constants:
   ```python
   CLIENT_ID = "<your-client-id>"
   CLIENT_SECRET = "<your-client-secret>"
   REDIRECT_URI = "http://127.0.0.1:8888/callback"
   ```
4. Make sure the redirect URI matches exactly in your Spotify app settings.

---

## 🚀 Usage

Run the script:

```bash
python spotify_macropad.py
```

You’ll see:

```
Spotify MacroPad ready. Press Page Up/Re Pag to toggle on/off.
```

Use the following keys when MacroPad is **ON**:

| Key                                 | Action                                |
| ----------------------------------- | ------------------------------------- |
| **Page Up** / **Re Pag**            | Toggle MacroPad on/off                |
| **Page Down** / **Av Pag**          | Play / Pause                          |
| **↑** / **flecha arriba**           | Increase volume (+10%)                |
| **↓** / **flecha abajo**            | Decrease volume (‑10%)                |
| **←** / **flecha izquierda**        | Play previous track                   |
| **→** / **flecha derecha**          | Play next track                       |
| **Del** / **Supr**                  | Toggle shuffle on/off                 |
| **Shift Right** / **Mayús derecha** | Toggle repeat (off→context→track→off) |
| **Home** / **Inicio**               | Toggle like / unlike current track    |
| **ç**                               | Toggle mute / unmute                  |

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

```text
MIT License

Copyright (c) 2025 naarvent_

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
