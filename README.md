# lore-logic-agents

The shared Claude Code plugin for **Lore and Logic**, built during our 12-week
Applied AI Engineer program.

Over the program this repo becomes a single plugin that packages the team's
Claude Code **subagents**, **skills** and **hooks**, so everyone works with the
same tools.

## Team

- Stacey
- Murdoch
- Lochlan
- Ewan

## This repo grows weekly

This is only the starting structure. Each week of the program adds something
new. Expect folders like `agents/`, `skills/` and `hooks/` to show up as we
build them. If something looks unfinished, it probably is. That's the point.

## Gate 0

Each team member adds a file about themselves at:

```
team/<name>.md
```

Use your first name in lowercase, for example `team/stacey.md`. The program
defines what goes in the file.

Keep it light: your name, your program goal and your flagship idea. No phone
numbers, addresses or work details. This repo is public.

## How to contribute

All changes go through a pull request. Nobody pushes directly to `main`.

1. **Branch.** Start from an up-to-date `main` and create a branch for your change:
   ```bash
   git checkout main
   git pull
   git checkout -b <your-name>/<short-description>
   ```
   For example: `stacey/gate-0`.
2. **Commit and push** your branch:
   ```bash
   git push -u origin <your-branch>
   ```
3. **Open a pull request** into `main`. Say what you changed and why.
4. **Get one approval** from a teammate before merging.
5. **Merge**, then delete the branch.

Keep pull requests small and focused. One change per pull request makes review
quick.

### Don't commit secrets or confidential material

- **No client or confidential work material in any repo, public or private.**
  Making a repo private hides a mistake; it doesn't prevent one.
- **No keys, tokens or passwords.** API keys and other secrets go in a local
  `.env` file, which `.gitignore` already excludes. If you need to show which
  variables are required, add a `.env.example` with placeholder values.
- **If something sensitive gets committed,** remove it, rotate any exposed key
  right away, and tell the team. Deleting a file doesn't remove it from Git
  history, so treat anything that was pushed as exposed.
