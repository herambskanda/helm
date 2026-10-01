# Install Helm on Windows

[Back to the download table](../../README.md#install) · Mac: [install on a Mac](mac.md) · Linux: [install on Linux](linux.md)

Helm installs for you only, so it doesn't ask for an administrator password. It takes about two minutes.

## 1. Download the right file

**Settings › System › About**, then look at **System type**.

- *x64-based processor* (most computers): download [Helm-windows-x64.exe](https://github.com/herambskanda/helm/releases/latest/download/Helm-windows-x64.exe).
- *ARM-based processor*: download [Helm-windows-arm64.exe](https://github.com/herambskanda/helm/releases/latest/download/Helm-windows-arm64.exe).

Your browser may ask whether to keep the file. Choose **Keep**.

## 2. Run the installer (the one extra step)

Helm isn't signed with Microsoft yet, so Windows warns you the first time. You do this once.

1. Double-click the downloaded `.exe`.
2. A blue window says **Windows protected your PC**. Click **More info**.
3. Click **Run anyway**.
4. There is nothing to choose: the installer puts Helm in your own user folder (no administrator needed),
   adds it to the Start menu and the desktop, and opens it.

If your browser or antivirus won't let you keep the file at all, see [Helm won't open](../help/wont-open.md).

## 3. First start

Open **Helm** from the Start menu. It opens on **Connect an agent**. Sign in to Claude Code (with your Claude
account) or Codex (with ChatGPT). Your browser opens to sign in, and you come back to Helm. See
[Sign in or switch accounts](../help/sign-in.md).

![Connect an agent](../pictures/connect-agent.png)

The first time, Helm also shows a short note called **Helm is in gamma**. It says what is shared and how to
switch it off. Press **Got it**. Then go to [Get started](../guide/getting-started.md).

In Helm, **Ctrl** is the key to use where the guide says ⌘ on a Mac.

## Where Helm keeps things

| What | Where |
|---|---|
| Your projects | A folder called **Helm** in your user folder (`C:\Users\<you>\Helm`). Each project is a folder inside it. You can choose another place in **Settings › Appearance › New projects**. |
| Helm's own things (settings, your library, your notes) | `C:\Users\<you>\.helm`. In File Explorer, type `%USERPROFILE%\.helm` in the address bar. |
| Window size and position | `%APPDATA%\Helm` |

Helm stays in the **notification area** (bottom right, you may need to click the small ^ arrow) after you close
the window, so routines can keep running. **Quit Helm** from that icon's menu really quits.

## Updating

When a newer Helm is out, Helm says **A new Helm is ready · Download**. Click it, download the new `.exe`, and
run it. It installs over the old one. Your projects stay as they are. You may see **More info › Run anyway**
again. See [Update Helm](../help/update-helm.md).

## Uninstalling

Quit Helm (notification-area icon › **Quit Helm**), then **Settings › Apps › Installed apps**, find **Helm**,
and choose **Uninstall**. Your projects in `C:\Users\<you>\Helm` and Helm's own folder `.helm` stay behind on
purpose. To remove everything, see [Uninstall Helm](../help/uninstall.md).

Having trouble? [Helm won't open](../help/wont-open.md).
