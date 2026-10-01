# The Marketplace list

[Back to the start](../README.md)

This folder is what Helm reads when you open the **Marketplace**.

| File | What it is |
|---|---|
| `marketplace.json` | The list: each item's name, version, kind, one plain line, who it's for, what it may reach, and where its package is |
| `packages/*.zip` | One package file for each item. Helm downloads one when you click **Get** |

You don't need to open these files. Helm reads them for you, and shows what an item may reach before you install it.

## What's listed

| Item | Kind | What it is |
|---|---|---|
| Product kit | Template | A whole project for product work: Discover, Define, Prototype and Measure |
| Everyday workbenches | Set of workbenches | Documents, tables, images, PDFs, slides and web pages: the workbenches most projects start with |
| Data and media workbenches | Set of workbenches | Notebooks that run Python, dashboards, recordings with their transcripts, and videos |
| Research kit | Workspace | Interviews with their transcripts, quotes pulled out, and what repeated each week |
| Decision log | Workbench | One decision per artifact: what, why, the options weighed, and when to look again |
| Checklist view | Capability | The task list in any Markdown file as a checklist you tick, with how much is done |
| Competitive analyst | Subagent | Reads competitors' public pages and says what changed since last time |
| Launch emails | Workflow | Drafts three launch emails from a story and its release notes, checks them, then waits for you |
| Friday update | Routine | Every Friday at 16:00, a short update on what changed this week, ready to send |
| British spelling | Hook | After any text changes, points out American spellings and their British ones |

A tick beside the maker means Heramb or Helm made it. The exact list is in `marketplace.json`, which can be
a little newer than this table.

## Who lists what

Heramb approves every listing. Items from friends are checked before they appear: the files are looked at, and what each may reach is written next to it.

- To **get** something, see [Get something from the Marketplace](../docs/help/get-from-marketplace.md).
- To **share** something, see [Share something to the Marketplace](../docs/help/share-to-marketplace.md).
