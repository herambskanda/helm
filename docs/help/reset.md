# Reset Helm

[Help](README.md)

Use this when Helm behaves oddly and a restart didn't help. Your projects are never touched.

## Light reset: settings only

1. Quit Helm (menu bar, notification area or tray icon › **Quit Helm**).
2. Open Helm's own folder, `.helm` in your home folder (hidden; see [Mac](../install/mac.md#where-helm-keeps-things), [Windows](../install/windows.md#where-helm-keeps-things) or [Linux](../install/linux.md#where-helm-keeps-things)).
3. Rename the file `settings.json` to `settings-old.json`.
4. Open Helm. Settings are back to the defaults.

## Full reset: start Helm fresh

This clears your settings, the list of recent projects, your own library, Studio drafts and any notes you haven't sent.

1. If you have notes you want to send, make the file first ([Report a problem](report-a-problem.md)).
2. Quit Helm.
3. Rename the folder `.helm` to `.helm-old`. (Don't delete it yet.)
4. Open Helm. It starts like the first time.
5. Add your projects back: **New project › A folder I already have**, and choose each folder in your **Helm** folder.
6. If everything is fine, delete `.helm-old`. If you miss something, quit Helm, delete the new `.helm` and rename `.helm-old` back.

You'll be asked to sign in to your agents again only if Claude Code or Codex lost their sign-in. See [Sign in or switch accounts](sign-in.md).
