<h1><picture><source media="(prefers-color-scheme: dark)" srcset="docs/pictures/helm-lockup-dark.png"><img alt="Helm" src="docs/pictures/helm-lockup-light.png" width="188"></picture></h1>

Helm gives your work with AI agents a face. You and your agent work side by side on the things you are
making, such as a story, a web page, an interview or a spreadsheet, and you see them and change them
on screen instead of only reading text in a chat. It looks like the desktop apps for talking to an
agent, with the work on the right, and it comes with Claude Code and Codex so there is nothing else to install.

https://github.com/user-attachments/assets/a8cf037a-529f-405e-bcca-d3c64edf64ae

> **Helm is in early testing (gamma).** You got this link from Heramb. Things will be rough in places,
> and your notes are how it gets better. See [Report a problem](docs/help/report-a-problem.md).

## Download

<a id="install"></a>

Pick the row for your computer. Not sure which one is yours? See [Which one is mine?](#which-one-is-mine) below.

| Your computer | Download | Step by step |
|---|---|---|
| Mac with Apple silicon (M1, M2, M3, M4…) | [Helm-mac-arm64.dmg](https://github.com/herambskanda/helm/releases/latest/download/Helm-mac-arm64.dmg) | [Install on a Mac](docs/install/mac.md) |
| Mac with an Intel chip | [Helm-mac-x64.dmg](https://github.com/herambskanda/helm/releases/latest/download/Helm-mac-x64.dmg) | [Install on a Mac](docs/install/mac.md) |
| Windows, most computers (x64) | [Helm-windows-x64.exe](https://github.com/herambskanda/helm/releases/latest/download/Helm-windows-x64.exe) | [Install on Windows](docs/install/windows.md) |
| Windows on an ARM computer | [Helm-windows-arm64.exe](https://github.com/herambskanda/helm/releases/latest/download/Helm-windows-arm64.exe) | [Install on Windows](docs/install/windows.md) |
| Linux, most computers (x64) | [Helm-linux-x64.AppImage](https://github.com/herambskanda/helm/releases/latest/download/Helm-linux-x64.AppImage) or [Helm-linux-x64.deb](https://github.com/herambskanda/helm/releases/latest/download/Helm-linux-x64.deb) | [Install on Linux](docs/install/linux.md) |
| Linux on an ARM computer | [Helm-linux-arm64.AppImage](https://github.com/herambskanda/helm/releases/latest/download/Helm-linux-arm64.AppImage) or [Helm-linux-arm64.deb](https://github.com/herambskanda/helm/releases/latest/download/Helm-linux-arm64.deb) | [Install on Linux](docs/install/linux.md) |

Every file is also on the [Releases page](https://github.com/herambskanda/helm/releases/latest), with a
`SHA256SUMS.txt` if you want to check a download.

**Helm isn't signed with Apple or Microsoft yet** (that comes before the public release). Your computer will
warn you the first time you open it. The install page for your computer shows the one click that gets past
the warning. It's safe to do for a file you got from the link above.

### Which one is mine?

- **Mac:** Apple menu › **About This Mac**. Next to **Chip** it says *Apple M…* (M1, M2, and so on) for
  Apple silicon, or *Intel* for an Intel Mac.
- **Windows:** **Settings › System › About**. Look at **System type**. *64-bit operating system, x64-based
  processor* means the x64 file. *ARM-based processor* means the ARM file. If you aren't sure, it is almost
  certainly x64.
- **Linux:** open a terminal and type `uname -m`. *x86_64* means x64. *aarch64* or *arm64* means ARM.

## After you install

1. [Get started](docs/guide/getting-started.md): sign in to an agent, then make your first project from a template.
2. Read the [user guide](docs/guide/README.md), one short page per part of Helm.
3. Stuck? The [help pages](docs/help/README.md) have numbered steps for each task.

## What's in this folder

| Folder | What it holds |
|---|---|
| [docs/install](docs/install/) | Install pages for [Mac](docs/install/mac.md), [Windows](docs/install/windows.md) and [Linux](docs/install/linux.md) |
| [docs/guide](docs/guide/README.md) | The user guide |
| [docs/help](docs/help/README.md) | Step-by-step help: report a problem, update, sign in, share, reset, uninstall |
| [marketplace](marketplace/README.md) | The Marketplace list Helm reads, and the packages in it |

## Report a problem

Helm has a note button in the top right. Pin a note on whatever looks wrong, then **Send my notes** makes
one small file that you can look at before you send it. The steps are in
[Report a problem](docs/help/report-a-problem.md). You can also [open the form](https://github.com/herambskanda/helm/issues/new?template=problem.yml)
directly. You need a free GitHub account to send it.

## What leaves your computer

Your projects stay in a folder on your computer. Helm sends nothing anywhere by itself, with two small
exceptions that it tells you about the first time you start it: it looks here for a newer Helm and for the
Marketplace list, and, unless you switch it off in **Settings › Data**, it shares the name, one line and page of
any small Helm tool you make (never its code or your files). Your notes go nowhere until you send the file yourself.
Your agent (Claude Code or Codex) works the way it always does, with your own account.
