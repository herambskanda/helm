# Workflows and routines

[Guide](README.md) · previous: [The Control center](control-center.md) · next: [Settings](settings.md)

## Workflow

A **workflow** is steps done in order, written as numbered sentences: "1. Researcher · read the insight and its quotes. 2. Writer · draft the story." Each step says who does it and what. Run one from a workspace page (its workflows are buttons, such as **Run Story from insight**) or from the Control center with **Run now**.

Make or change one in the [Studio](studio.md) under **Workflows**, or ask the agent: "Save these steps as a recipe."

## Routine

A **routine** is something that runs on a schedule: "Check the stories every Friday at 4pm."

- **What to do** (a request or a workflow), **When** (once, every day, every weekday, every week on chosen days, every month, or when something happens), **Who does it**, **If it needs to ask while you're away**, and **Where the results go**.
- **If it needs to ask while you're away:** **Skip it and tell me** (the default) or **Go ahead**. A skipped step is kept on the run, with **Allow this from now on**.
- **Where the results go** is a workspace: each run saves its answer there as a dated document ("Friday update · Fri 25 Sep"). Left empty, the answer stays in the Control center.
- A routine uses only the tools listed on its page, each with a switch.

Ask the agent in a conversation ("Check the stories every Friday at 4pm") and it asks one plain question before making the routine. Then it's in the Studio and on the Control center.

## While Helm is closed

Routines run while Helm is open, **and after you close the window**: Helm stays in the menu bar (Mac), notification area (Windows) or tray (Linux). Its menu shows what ran, what's next, **Open Helm**, **Pause routines for an hour** and **Quit Helm** (which really quits, so routines stop). A routine that fell due while your computer slept runs when it wakes. One that fell due while Helm was fully quit shows as *missed*, with **Run now**.

In **Settings › While Helm is closed** you can turn the keep-running behaviour off, have Helm open when your computer starts (Mac and Windows through the system's own setting, and Linux through an autostart entry), and choose when Helm tells you about a routine: only if it skipped something or didn't finish, every time, or never.

## Hooks

A **hook** is a check that runs when something happens, such as when a story moves to a new status. It can check something in plain words or hand work to a helper. A hook that fails three times in a row is paused, with **Resume**, so a broken hook doesn't keep running paid agents.
