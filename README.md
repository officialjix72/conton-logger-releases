# CONTON Logger

Shows what your PS4 says while you play with CONTON mods, spots crashes and problems as they happen,
and makes one bug report file you can send me. That file is what lets me actually fix the bug
instead of guessing.

**[Download the newest version](https://github.com/officialjix72/conton-logger-releases/releases/latest)**

Get `CONTON-Logger-<version>.zip`, unzip it anywhere you like (Documents is fine) and run
`CONTON-Logger.exe` inside the folder. Windows 10 or 11, nothing to install.

---

## Getting started

1. On your PS4, load GoldHEN and turn on the **klog server** in GoldHEN's settings.
2. Find your PS4's IP address: *Settings > Network > View Connection Status*.
3. Type the IP in the logger and press **Connect**.
4. **Connect before you start the game.** The PS4 doesn't keep old messages, so the logger can only
   save what happens while it is connected.
5. Play like normal. If something goes wrong, a red bar appears at the top and the list on the right
   tells you what happened. Click any line and the box at the bottom explains it.

The logger has two ways of talking. **Simple** explains everything in plain words. **Technical**
shows the raw log, line numbers, CONTON codes and crash addresses. Switch at the top right.

## Sending me a bug report

1. Press **Report a bug** at the top right, or **Report this crash** on the red bar.
2. Write what happened and what you were doing right before. A sentence or two is enough.
3. Add screenshots or phone videos if you have them: drag them onto the window, press *Add files*,
   or press *Paste screenshot*. As many as you like.
4. Press **Create report**.
5. Press **Post on GitHub**. The bug report form opens here, and the logger shows you the file:
   drag it into the form. You can also send the file on Discord.

That one file has everything I need: the log with the time of every line, crash details, what the
logger found, your notes and your pictures.

Videos can make the file big. If it's too big for Discord, post it here instead.

## Windows or my antivirus complains

The program isn't code-signed (that costs money every year), so Windows SmartScreen may say
"Windows protected your PC" the first time. Click **More info**, then **Run anyway**.

Some antivirus programs are wary of any new program that isn't signed. If yours removes it, restore
it from the antivirus quarantine and add an exception for the logger's folder.

To check your download is the real one, compare its SHA-256 with `SHA256SUMS.txt` on the release
page. In PowerShell:

```
Get-FileHash .\CONTON-Logger.exe
```

## Your privacy

The logger never sends anything anywhere by itself. It only opens a web page when you press a
GitHub button. Your logs and reports stay on your PC until you send them.

With *Hide my network details and PC username* on (it is by default), reports have IP and MAC
addresses, account IDs, online IDs, e-mail addresses and your Windows user name removed. Pictures
and videos are added exactly as they are, so check they don't show anything private.

## Where things are saved

Everything stays in the logger's folder:

| Folder or file | What's in it |
| --- | --- |
| `logs` | every capture, each line with the time it arrived |
| `logs\raw` | an untouched copy of what the PS4 sent (can be turned off in Settings) |
| `reports` | your bug reports |
| `CONTON-Logger.ini` | your settings |

If the folder isn't writable, the logger uses `Documents\CONTON Logger` instead.

---

CONTON Logger by **OfficialJix** / JixStudios. The Exo 2 typeface is used under the SIL Open Font
License 1.1.
