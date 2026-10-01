# Helm won't open

[Help](README.md)

Find your computer, then try the steps in order.

## Mac

1. **"Helm" can't be opened because Apple cannot check it** (or it was blocked): open **System Settings › Privacy & Security**, scroll to **Security**, click **Open Anyway** next to Helm, then **Open**.
2. **Says Helm is damaged, or Open Anyway isn't there:** open **Terminal** and run
   `xattr -dr com.apple.quarantine /Applications/Helm.app`, then open Helm again.
3. **Helm is in Applications?** Open it from there, not from the downloaded disk image.
4. **Opens, then nothing appears:** Helm may already be running. Look for its icon in the menu bar at the top right, click it and choose **Open Helm**. If you see two Helm icons, **Quit Helm** from both, then open it once.
5. **Wrong file?** On an Intel Mac use `Helm-mac-x64.dmg`; on Apple silicon use `Helm-mac-arm64.dmg` ([which is mine?](../../README.md#which-one-is-mine)).

## Windows

1. **"Windows protected your PC":** click **More info**, then **Run anyway**.
2. **The download disappeared or was blocked:** your browser or antivirus held it because Helm isn't signed yet. In Edge or Chrome, open the downloads list and choose **Keep**. In Windows Security › **Virus & threat protection › Protection history**, restore it if it was quarantined.
3. **The installer says the file is blocked:** right-click the `.exe` › **Properties**, tick **Unblock** at the bottom, **OK**, and run it again.
4. **Installed but nothing happens when you open it:** Helm may already be running. Look in the notification area (bottom right; click the small ^), right-click the Helm icon and choose **Open Helm**. Or **Quit Helm** from there and open it again.
5. **Wrong file?** Most computers need `Helm-windows-x64.exe` ([which is mine?](../../README.md#which-one-is-mine)).

## Linux

1. **AppImage does nothing:** it must be runnable. `chmod +x Helm-linux-x64.AppImage`, then `./Helm-linux-x64.AppImage` in a terminal so you can see any message.
2. **A message about libfuse2:** Ubuntu 22.04 `sudo apt install libfuse2`, Ubuntu 24.04 `sudo apt install libfuse2t64`.
3. **.deb says dependencies are missing:** install with `sudo apt install ./Helm-linux-x64.deb` (with `apt`, not `dpkg -i`), which fetches what's needed.
4. **Wrong file?** `uname -m` says *x86_64* for x64 and *aarch64* for ARM.
5. **Starts, then closes right away:** run it from a terminal and keep the text it prints.

## Every system

- **"Something else is already using a port":** another copy of Helm is running. **Quit Helm** from its menu bar, notification area or tray icon, wait a few seconds, and open it once.
- **Restart your computer** and try again.
- **Helm's log** is a plain text file, `logs/core.log` inside Helm's own folder (`.helm` in your home folder). Attach it, or its last few lines, when you [report a problem](report-a-problem.md).
- **Last resort:** [reinstall](../../README.md#install) the newest version. Your projects are safe.
