# Splunky TOOLS

Nov 1, 2026 · @Splunky

## What is this

Splunky TOOLS is a Python terminal multitool with a full curses UI — cyan-on-black, navigable menu, 27 wired functions across Discord, Roblox, Fortnite, Minecraft, and utility. One file, one run, no GUI framework needed. Built to look and feel like a real hacker terminal: ASCII banner, bordered menu box, scrollable output, live prompt line at the bottom.

## Requirements & Install

**Python:** 3.8+

```bash
# install deps
pip install requests websockets

# Windows only
pip install windows-curses

# run
python splunky_tools.py
```

**Optional deps (only needed for specific tools):**

- `Pillow` — tools 21 (Image to ASCII) and 23 (Text to Image)
- `yt-dlp` — tool 24 (Youtube DL)
- `pyinstxtractor.py` — tool 25 (EXE to PY), place in the same directory

Terminal must be at least **100 × 30** characters. Resize if the box clips.

## Usage & Controls

On launch the menu appears. Navigate with keyboard only — no mouse needed.

| Key | Action |
| --- | --- |
| `↑` / `↓` | Move selection up / down |
| `←` / `→` | Jump one column left / right |
| `Enter` | Run selected tool |
| `0`–`9` | Type a number to jump straight to that tool |
| `Q` | Quit |
| `↑` / `↓` in output | Scroll output lines |
| Any other key in output | Return to menu |

When you run a tool, an input screen appears with one prompt per required field. Hit `Enter` on each. Defaults are shown in brackets — hit `Enter` to accept them. After the tool finishes, output is shown in a scrollable screen.
