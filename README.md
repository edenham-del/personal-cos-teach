# Personal Chief of Staff

A real, working Chief of Staff pattern — set your priorities, your voice,
and connect your tools, and get calendar-and-inbox-aware briefings and
drafts on demand. No proprietary or company-specific information is in
this repo; every name, domain, and ID is a placeholder for you to fill in
with your own.

This repo has two versions of the same pattern, for two different ways of
running an AI assistant:

## [`COS-Claude-Code/`](COS-Claude-Code/) — for Claude Code

Runs inside a project folder on your machine. Uses a `CLAUDE.md`, a
`config.yaml`, a `voice.md`, a `logbook/`, slash commands
(`.claude/commands/`), and scheduled triggers (`triggers/`). Best if
you're comfortable with a terminal and want the full command/trigger
structure, or plan to connect tools via MCP.

## [`COS-Claude-Web/`](COS-Claude-Web/) — for claude.ai Projects

Runs entirely in your browser at claude.ai — no terminal, no coding.
Built for non-technical setup: you edit exactly **one** file
(`YOUR-INFO.md`, plain-English questions) and copy-paste the rest into a
claude.ai Project's Custom Instructions and knowledge base. Best if you
just want this working in 5 minutes.

Both fold down to the same underlying idea: teach an AI assistant who you
are, how you write, and give it access to your real calendar/email/Slack,
so a two-word request like "morning briefing" produces a real,
personalized answer.

## Which one should I use?

- **Never touched a terminal, just want it working today** →
  `COS-Claude-Web/`
- **Comfortable with Claude Code, want slash commands and MCP tools** →
  `COS-Claude-Code/`
- **Not sure** → start with `COS-Claude-Web/`. You can always move to
  `COS-Claude-Code/` later if you outgrow it.

## What this is not

- Not autonomous — every pattern here drafts, never sends, without your
  review.
- Not tied to any specific company's tools — swap Gmail/Calendar/Slack for
  whatever you actually use.
- Not magic — if you don't fill in your own information, it has nothing
  to prioritize by and no voice to match.

## License

MIT — see [`LICENSE`](LICENSE). Free to use, fork, and adapt for your own
setup.

Built by [Siddharth Dixit](https://github.com/siddsdixit).
