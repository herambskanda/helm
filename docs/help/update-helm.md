# Update Helm

[Help](README.md)

Helm checks for a newer version when it starts and once a day. When there is one, it says
**A new Helm is ready · Download**. Nothing downloads or installs by itself.

1. Click **A new Helm is ready · Download**. Your browser opens the page for the new version.
2. Download the file for your computer (the same row you used the first time: see the [download table](../../README.md#install)).
3. **Quit Helm** first. Mac: the menu bar icon › **Quit Helm**. Windows: the notification-area icon › **Quit Helm**. Linux: the tray icon › **Quit Helm**. (Closing the window is not enough, because Helm keeps running in the background.)
4. Install it over the old one:
   - **Mac:** open the `.dmg`, drag **Helm** onto **Applications**, choose **Replace**.
   - **Windows:** run the new `.exe`. It installs over the old one.
   - **Linux AppImage:** replace the old file with the new one, then `chmod +x` it again. **Linux .deb:** `sudo apt install ./Helm-linux-x64.deb` with the new file.
5. If your computer warns you again, do the same one click as the first time: Mac **Open Anyway** (see [Mac](../install/mac.md)), Windows **More info › Run anyway** (see [Windows](../install/windows.md)).
6. Open Helm. Your projects, settings and library are untouched. **Settings › About** shows the new version.

If Helm doesn't show the note, the [newest version's page](https://github.com/herambskanda/helm/releases/latest) always has the files.
