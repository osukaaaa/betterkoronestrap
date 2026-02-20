# betterkoronestrap
# 🐾 KoroneStrap

A **Bloxstrap-style** launcher for [Pekora.zip](https://www.pekora.zip) — built with Python and tkinter.

---

## ✨ Features

- **🏠 Home Page** — One-click Play button that opens pekora.zip (just like Bloxstrap opens Roblox)
- **⚡ Fast Flags** — Add, edit, remove, and import FastFlags with a full GUI
  - Presets for FPS unlock, graphics quality, network tweaks
  - Import from JSON paste
  - Auto-applies flags before every launch
- **⬇️ Install** — Download & run the Pekora bootstrapper with a progress bar
- **⚙️ Settings** — Wine binary selector, prefix path, auto-flag toggle
- **🔍 Debug** — Live system diagnostics: installation paths, Wine version, active flags

---

## 🚀 Quick Start (Run from Source)

### Requirements
- Python 3.8+
- tkinter (usually bundled with Python)

### Windows
```
python koronestrap.py
```

### Linux
```bash
# Install tkinter if missing:
sudo apt install python3-tk     # Ubuntu/Debian
sudo pacman -S tk               # Arch

python3 koronestrap.py
```

### macOS
```bash
brew install python-tk
python3 koronestrap.py
```

---


---

## 🍷 Wine Setup (Linux / macOS)

KoroneStrap uses Wine to run the Windows bootstrapper.

```bash
# Ubuntu / Debian
sudo apt install wine64

# Arch
sudo pacman -S wine

# macOS (via Homebrew)
brew install --cask wine-stable
```

The Settings page lets you pick between `wine64` and `wine`, and set a custom Wine prefix.

---

## 📁 File Locations

| File | Path |
|---|---|
| FastFlags | `~/.koronestrap/fastFlags.json` |
| Config | `~/.koronestrap/config.json` |

---

## 📝 Notes

- The **Play** button opens pekora.zip in your browser — the website handles the actual game launch (same as how Bloxstrap works with Roblox.com)
- FastFlags are auto-applied before every launch if the game is already installed
- Linux URI handling (`pekora-player://`) is supported — run `python3 koronestrap.py --uri <uri>`

---

*Made with ♥ by osuka*
*original by LittleBigDevs*
