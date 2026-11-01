# Personal Chief of Staff — Codex CLI (ChatGPT)

The same Chief of Staff pattern as [`../COS-Claude-Code/`](../COS-Claude-Code/), for **Codex CLI (ChatGPT)**. It runs in a folder on your machine and reads plain-text files: `AGENTS.md`, `config.yaml`, `voice.md`, `logbook/`.

## Setup

1. Install and sign in:
   ```
   npm install -g @openai/codex   # or: brew install codex
codex            # first run: sign in with your ChatGPT account
   ```
2. Copy this folder somewhere you keep notes, for example `~/chief-of-staff/`.
3. Fill in `config.yaml` (your name, role, priority people, channels, thresholds) and `voice.md` (paste something you actually wrote). Fill in the `[BRACKETS]` at the top of `AGENTS.md`.
4. Start the assistant **from inside this folder**: `cd ~/chief-of-staff && codex`. Codex starts every session in the current folder and reads `AGENTS.md` automatically.
5. Type: **morning briefing**.

## Connecting email and calendar (optional)

Connect tools through MCP servers in `~/.codex/config.toml` (`[mcp_servers.<name>]`). Start with Gmail and Calendar. Without them, paste or upload text and it works from that.

## The 5 routines

| Say this | Runs |
|---|---|
| "morning briefing" | `triggers/cos-morning.md` |
| "EOD" | `triggers/cos-eod.md` |
| "urgent check" | `triggers/cos-urgent.md` |
| "week ahead" | `triggers/cos-week.md` |
| "pulse check" | `triggers/cos-composer.md` |

## Commands

Codex has no project-level slash commands. Say it in plain English instead: "run the cos-brief recipe on the Northstar pricing thread". Codex reads `commands/cos-brief.md` and follows it. (Optional: copy a recipe to `~/.codex/prompts/` to get a `/prompts:cos-brief` command on your machine.)

## Recipes in `commands/`

`cos`, `cos-brief`, `cos-delegate`, `cos-email-draft`, `cos-find-time`, `cos-focus`, `cos-followup`, `cos-spend`, `cos-thread`.

## Scheduling

Neither tool has a built-in scheduler. To run a routine at 7 AM, use cron or launchd to run `codex -p "morning briefing"` from this folder. Keep it draft-only.

## Safety

It drafts, never sends. Your first run will ask permission before it edits files or runs commands: read each prompt. Keep it in this folder.

MIT — see [`../LICENSE`](../LICENSE).
