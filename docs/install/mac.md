# Install Helm on a Mac

[Back to the download table](../../README.md#install) · Windows: [install on Windows](windows.md) · Linux: [install on Linux](linux.md)

Helm runs on Macs with Apple silicon and on Intel Macs. It takes about two minutes.

## 1. Download the right file

Apple menu › **About This Mac**. Next to **Chip**:

- *Apple M1* (or M2, M3, M4…): download [Helm-mac-arm64.dmg](https://github.com/herambskanda/helm/releases/latest/download/Helm-mac-arm64.dmg).
- *Intel*: download [Helm-mac-x64.dmg](https://github.com/herambskanda/helm/releases/latest/download/Helm-mac-x64.dmg).

## 2. Put Helm in Applications

1. Open the downloaded `.dmg` file (double-click it in Downloads).
2. A small window shows the Helm icon and an **Applications** folder. Drag **Helm** onto **Applications**.
3. Close that window. You can eject the Helm disk from Finder's sidebar.

## 3. Open it the first time (the one extra step)

Helm isn't signed with Apple yet, so the Mac stops it the first time. You do this once.

1. Open **Applications** and double-click **Helm**. The Mac says it can't verify the app. Click **Done** (don't move it to the Bin).
2. Open **System Settings › Privacy & Security** and scroll down to **Security**.
3. You'll see *"Helm" was blocked*. Click **Open Anyway**, then enter your password or use Touch ID.
4. Click **Open** in the next window. From now on Helm opens with a double-click.

**If Open Anyway doesn't show up,** or Helm says it's damaged, open **Terminal** (Applications › Utilities),
paste this line, press Return, and open Helm again:

```
xattr -dr com.apple.quarantine /Applications/Helm.app
```

It only removes the "downloaded from the internet" mark from Helm.

## 4. First start

Helm opens on **Connect an agent**. Sign in to Claude Code (with your Claude account) or Codex (with ChatGPT).
Your browser opens to sign in, and you come back to Helm. If you already use Claude Code on this Mac, Helm
finds you already signed in. See [Sign in or switch accounts](../help/sign-in.md).

![Connect an agent](../pictures/connect-agent.png)

The first time, Helm also shows a short note called **Helm is in gamma**. It says what is shared and how to
switch it off. Press **Got it**.

Then go to [Get started](../guide/getting-started.md).

## Where Helm keeps things

| What | Where |
|---|---|
| Your projects | A folder called **Helm** in your home folder (`/Users/<you>/Helm`). Each project is a folder inside it. You can choose another place in **Settings › Appearance › New projects**. |
| Helm's own things (settings, your library, your notes) | `/Users/<you>/.helm`. It starts with a dot, so Finder hides it. In Finder, press ⌘ Shift . (full stop) to show hidden folders, or use **Go › Go to Folder…** and type `~/.helm`. |
| Window size and position | `~/Library/Application Support/Helm` |

Helm stays in the **menu bar** (top right of the screen) after you close the window, so routines can keep
running. **Quit Helm** from that icon's menu really quits.

## Updating

When a newer Helm is out, Helm says **A new Helm is ready · Download**. Click it, download the new `.dmg`,
and drag Helm onto **Applications** again, choosing **Replace**. Quit Helm first. Your projects stay as they are.
You may need **Open Anyway** once more. See [Update Helm](../help/update-helm.md).

## Uninstalling

Quit Helm (menu bar icon › **Quit Helm**), then drag **Helm** from Applications to the Bin. Your projects in
`~/Helm` and Helm's own folder `~/.helm` stay behind on purpose. To remove everything, see
[Uninstall Helm](../help/uninstall.md).

Having trouble? [Helm won't open](../help/wont-open.md).
