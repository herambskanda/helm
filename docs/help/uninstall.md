# Uninstall Helm

[Help](README.md)

Uninstalling Helm leaves your projects alone.

## 1. Quit Helm for real

Menu bar (Mac), notification area (Windows) or tray (Linux) icon › **Quit Helm**.

## 2. Remove the app

- **Mac:** drag **Helm** from **Applications** to the Bin (Trash).
- **Windows:** **Settings › Apps › Installed apps › Helm › Uninstall**.
- **Linux AppImage:** delete the file. **Linux .deb:** `sudo apt remove helm`.

## 3. What stays behind, and how to remove it

Only do this if you want everything gone. Your projects are your own work, so check you don't need them first.

| What | Where (Mac and Linux / Windows) | Remove it? |
|---|---|---|
| Your projects | `~/Helm` / `C:\Users\<you>\Helm` | Only if you're sure. This is your work. |
| Helm's own things (settings, library, notes) | `~/.helm` / `C:\Users\<you>\.helm` | Yes, to forget Helm |
| Window settings | Mac `~/Library/Application Support/Helm`, Linux `~/.config/Helm` / Windows `%APPDATA%\Helm` | Yes |
| A `.helm` folder and `helm.yaml` inside each project | in the project | Leave them. Helm adds them, and they hold the project's setup and its conversations. Without Helm they do no harm |

Your Claude Code and Codex accounts are unaffected: you sign in to those yourself, and Helm didn't create them.
