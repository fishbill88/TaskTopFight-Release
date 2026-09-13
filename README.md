# TaskTopFight — releases

Windows builds of TaskTopFight, an idle fighting game that lives along the top
edge of your taskbar.

## Download

Grab `TaskTopFight-Setup-<version>.exe` from the
[latest release](https://github.com/fishbill88/TaskTopFight-Release/releases/latest)
and run it. It installs for the current user only — no admin prompt, no install
wizard, no options to pick.

Windows shows a SmartScreen warning the first time ("More info" → "Run anyway").
These builds are not code-signed yet.

## Updates

The app updates itself. It checks shortly after launch and every few hours,
downloads in the background, and installs silently — your hero, level, stage,
gear and gold come back exactly as you left them, down to whether you had the
playable area hidden. There is nothing to click and nothing to restart.

## Beta builds

These releases are the ones chosen to go out. Every change lands first in
[TTF-Beta-Release](https://github.com/fishbill88/TTF-Beta-Release), and only
gets promoted here once it has been run for a while.

To take the early builds instead, tick **Participate in beta test** in the
game's ⚙ settings panel. It is off by default, it is remembered per machine
rather than per account, and it takes effect without reinstalling anything.
Unticking it does not roll you back — the app never downgrades, so you simply
stop receiving builds until this feed catches up.

## What is in a release

| file | |
|---|---|
| `TaskTopFight-Setup-<version>.exe` | the installer — this is the one you want |
| `latest.yml` | the update feed the installed app polls |
| `*.blockmap` | lets an update download only the changed parts, not the whole 80 MB |
| `TaskTopFight-RoomServer-<version>.zip` | the Tower room server, from the same commit |

The last two are for the app, not for you. Don't delete them from a release:
that breaks auto-update for everyone still on an older build.

## Hotkeys

The strip is click-through, so it never gets in the way of real work — which
also means keys reach it only through these:

| | |
|---|---|
| `Ctrl+Alt+S` | settings |
| `Ctrl+Alt+T` | let the mouse reach the strip |
| `Ctrl+Alt+P` | pause |
| `Ctrl+Alt+Q` | save and quit |

---

Releases here are published by the **promote** workflow in the beta repo, run by
hand. Nothing in this repository is edited by hand.
