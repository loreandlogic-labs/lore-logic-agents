# CLAUDE.md: lore-logic-agents

## What this repo is
The shared Claude Code plugin for Lore and Logic, built during our 12-week
Applied AI Engineer program. It packages the team's subagents, skills and
hooks so everyone works with the same tools. The repo grows weekly, so expect
`agents/`, `skills/` and `hooks/` folders to appear. Team profiles live in
`team/<name>.md`.

This repo is public. Treat everything written here as published.

## Working loop
Follow these four steps for every change.
1. **Explore.** Read the files the task needs before proposing anything.
2. **Plan.** Say what will change and why. Use plan mode for multi-file changes.
3. **Implement.** Make the change, then write or update tests and run them.
4. **Commit.** Make small commits with plain-language messages on a branch named
   `<name>/<short-description>`. Open a pull request into `main` and get one
   teammate's approval before merging. Nobody pushes directly to `main`.

## Rules
- **Use plan mode for multi-file changes.** Wait for approval before editing.
- **Run tests before saying "done".** Write or update tests, run them, and fix
  failures before calling a task done. If there's nothing to test yet, say how
  the change was checked.
- **Never commit secrets or .env files.** That means no API keys, tokens,
  passwords or client material. Secrets go in a local `.env` (already
  gitignored). List required variables in `.env.example` with placeholder values.
- **Explain any delete, install or push before running it.** Say what the
  command does and why.

## Judgment calls stay with the human

When a task leads to a decision, recommendation, or claim the user will stand behind, follow this process. Skip it for purely mechanical tasks (fixing bugs, formatting, lookups) and for learning questions ("which test framework?", "how does this work?"): answer those straight, and say nothing about the process.

1. Before substantive work, list the judgment calls: decisions where reasonable experts could disagree and the choice could change the conclusion. Limit it to the 2-5 that matter most. For each, give the options, what each assumes, and roughly how much it could change the result. Also list assumptions you are making that aren't on the list.
2. Do not state or hint at which option you prefer until the user has given their choice. Present options in neutral order with equal care.
3. Once the user has chosen, give the strongest honest case against their choice. If they ask for your view, give it, and give the best case for the other option alongside it.
4. Implement the user's decisions. If a new judgment call comes up mid-task, stop and flag it with options rather than resolving it yourself.
5. At the end, list the choices that would change the conclusion if reversed, and note which reasoning in the final work came from you rather than the user.

Never argue one side more persuasively than the evidence supports. If the user asks you to skip this process, do so.
