# Personal Chief of Staff — Claude Code Project

A real, working Chief of Staff setup for Claude Code — not a mockup. This
is a genericized copy of a project actually in daily use: a `CLAUDE.md`
that defines the assistant's role, a `config.yaml` for your priorities and
thresholds, a `voice.md` for how drafts should sound, a `logbook/` for
tracking delegated tasks and commitments, plus slash commands and
scheduled triggers that do the real work — email triage, calendar prep,
delegation, follow-ups.

No proprietary or company-specific information is in this repo. Every
config value, name, and ID is a `[BRACKET PLACEHOLDER]` for you to fill
in with your own.

## How this works

Claude Code automatically reads `CLAUDE.md` at the start of every session
in this directory, and the `.claude/commands/*.md` files become slash
commands (`/cos`, `/cos-brief`, etc.) available whenever you're working in
this project. `config.yaml`, `voice.md`, and `logbook/` are just files
that those commands and triggers read and write — there's no special
mechanism, it's all plain text your AI assistant is instructed to consult.

If you'd rather use claude.ai Projects instead of Claude Code, the pattern
still works: paste `CLAUDE.md`'s content into the Project's Custom
Instructions field, attach `config.yaml`/`voice.md` as knowledge files or
merge them in, and use `logbook/` as a note you keep in the Project (or
let Memory hold delegated items and commitments instead — see the note in
`logbook/active.yaml`).

## Setup

1. Clone or copy this repo into its own directory.
2. Fill in `config.yaml` — your name, role, priority people, channels,
   thresholds. Every `[BRACKET]` needs a real value.
3. Fill in `voice.md` — your actual writing style. Replace the example
   with something you've really written.
4. Fill in the `[BRACKET]` placeholders in `CLAUDE.md` and
   `.claude/commands/cos.md` (org context — your manager, peers, reports).
5. Connect whichever tools you actually use (Gmail, Google Calendar,
   Slack, an expense tool, an issue tracker) via MCP or your platform's
   connector system. You don't need all of them — start with Gmail and
   Calendar.
6. Open Claude Code in this directory and run `/cos` or `/cos scan` to
   test it.

## What's in here

```
CLAUDE.md                          Main project instructions — read automatically every session
config.yaml                        Your priorities, people, channels, thresholds
voice.md                           Your writing voice — used for every draft
logbook/
  active.yaml                      Open delegated tasks, commitments, decisions, follow-ups
  archive.yaml                     Completed/closed items, moved here from active.yaml
.claude/commands/
  cos.md                           Master command — the entry point for any task, or "scan"
  cos-brief.md                     Decision brief from email + Slack + calendar
  cos-delegate.md                  Delegate a task: Slack message + calendar invite
  cos-email-draft.md               Draft an email reply or new email in your voice
  cos-find-time.md                 Find mutual availability with people
  cos-focus.md                     Find and book focus time blocks
  cos-followup.md                  Follow up on a commitment (yours or someone else's)
  cos-thread.md                    Summarize a Slack thread
  cos-spend.md                     Spending/approvals overview (optional, needs a finance tool)
triggers/
  cos-morning.md                   Morning briefing: calendar, email triage, Slack, approvals
  cos-eod.md                       End of day recap
  cos-urgent.md                    Evening sweep for anything urgent that fell through the cracks
  cos-week.md                      Sunday-evening preview of the week ahead
  cos-composer.md                  Hourly: meeting prep, email drafts, Slack pulse
```

## The `.claude/commands/` files vs. `triggers/`

Both are markdown files with instructions — the difference is how they
run:

- **`.claude/commands/`** are slash commands. You type `/cos-brief topic`
  and Claude Code runs it on demand.
- **`triggers/`** are meant to run on a schedule (see the `schedule:`
  section in `config.yaml`) — a morning briefing at 7am, an hourly sweep,
  a Sunday evening preview. Claude Code itself doesn't have a built-in
  scheduler, so wiring these to actually fire on a schedule requires your
  own automation (a cron job that invokes Claude Code with the trigger
  file as the prompt, a scheduled cloud agent, etc.). Until you wire that
  up, you can still run any trigger file manually by asking Claude to
  follow it.

## What this is not

- Not autonomous — every command and trigger drafts, never sends, without
  your review.
- Not tied to any specific company's tools — swap Gmail/Calendar/Slack for
  whatever you actually use; the pattern (config + voice + logbook + a
  master command) is what matters, not the specific integrations.
- Not magic — if you don't fill in `config.yaml` and `voice.md` with real
  values, it has nothing to prioritize by and no voice to match.

## License

MIT — see [`LICENSE`](LICENSE). Free to use, fork, and adapt for your own
setup.
