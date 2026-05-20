# MCGA — Make Commits Great Again

[![skills.sh](https://skills.sh/b/h1km4t1ll0/make-commits-great-again)](https://skills.sh/h1km4t1ll0/make-commits-great-again)

Claude Code skill: commit messages in the style of Donald Trump's tweets.

Serious technical meaning, dramatic delivery. CAPS, em dashes, "SAD!", "TREMENDOUS!", "the previous team KNEW", and the best fix in history — believe me.

## Example

**Before:**

```
refactor: move payment validation out of checkout route
```

**After:**

```
refactor: checkout-route — WALL OF LOGIC. DEMOLISHED!

Validation living inside HTTP handlers. DISASTER. Hard to test. Years of neglect.
Extracted validatePayment. Thin route. Clean boundaries. Fast tests.

Drained the swamp. NOBODY has done it better!
```

## Install

```bash
npx skills add h1km4t1ll0/make-commits-great-again
```

## Usage

In Claude Code, after staging or making changes:

```
make a commit
```

or

```
mcga
```

The skill kicks in automatically, reads your current `git diff`, picks a Conventional Commits type (`feat`, `fix`, `refactor`, `chore`, `docs`, etc.) and produces a Trump-style message. You confirm before the actual `git commit` runs.

## Features

- Conventional Commits prefix stays intact (`fix:`, `feat:`, `refactor:`, etc.) — only the part after the colon goes Trump.
- Auto-detects the user's language — generates the message in Russian, English, Spanish, German, or whatever language the conversation is in.
- Vocabulary arsenal with rotation: never opens or closes two commits in a row with the same phrase.
- Five headline shapes, several rhetorical patterns (triplets, repetition, negation flips, rhetorical questions, asides) — varied output, not the same template every time.
- Adapts tone to the type of change: trivial diffs (typos, whitespace) don't get called "DISASTER", breaking changes get a proper `BREAKING CHANGE:` footer.
- Hard guardrails: no profanity, no emojis, no attacks on real people / teams / companies, no politics, no invented technical facts.

## What it will NOT do

- Mention real politicians, people, countries, races, religions.
- Use insults against anyone.
- Add `Co-Authored-By: Claude` or `Generated with Claude Code` trailers.
- Use emojis.
- Use `!!!` or `???` — one mark in a row max.
- Invent things that aren't in the diff. The style is dramatic, the facts are real.

## When NOT to use it

- Serious production repository with strict commit hygiene rules. Your team will not be amused.
- Open-source projects with public contribution guidelines that require neutral commit messages.
- Anywhere a hiring manager might `git log` you.

For those cases, ask Claude for a "regular commit" or "conventional commit" — the skill steps aside and produces a neutral message.

## Compatibility

Works with any agent that supports the open Agent Skills standard:

- Claude Code
- Cursor
- Codex
- GitHub Copilot
- Windsurf
- Gemini CLI
- and others

## Manual install

If you don't want to use the CLI, copy `mcga/SKILL.md` into one of:

- `~/.claude/skills/mcga/SKILL.md` (user-level, all projects)
- `<project>/.claude/skills/mcga/SKILL.md` (project-level, commit it to the repo)

## License

[WTFPL](https://www.wtfpl.net/) — Do What the Fuck You Want to. Make commits great again.

## Disclaimer

This is a joke skill. The style references a public figure's well-known communication patterns; the skill itself does not endorse any political position, person, or platform. No real people are attacked or named inside generated commit messages.