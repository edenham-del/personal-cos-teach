# Personal Chief of Staff — Gemini CLI

The same Chief of Staff pattern as [`../COS-Claude-Code/`](../COS-Claude-Code/), for **Gemini CLI**. It runs in a folder on your machine and reads plain-text files: `GEMINI.md`, `config.yaml`, `voice.md`, `logbook/`.

## Setup

1. Install and sign in:
   ```
   npm install -g @google/gemini-cli   # or: brew install gemini-cli
gemini           # first run: sign in with your Google account
   ```
2. Copy this folder somewhere you keep notes, for example `~/chief-of-staff/`.
3. Fill in `config.yaml` (your name, role, priority people, channels, thresholds) and `voice.md` (paste something you actually wrote). Fill in the `[BRACKETS]` at the top of `GEMINI.md`.
4. Start the assistant **from inside this folder**: `cd ~/chief-of-staff && gemini`. Gemini CLI reads `GEMINI.md` from the current folder automatically (check with `/memory show`).
5. Type: **morning briefing**.

## Connecting email and calendar (optional)

Connect tools through MCP servers in `.gemini/settings.json` (`"mcpServers"`). Start with Gmail and Calendar. Without them, paste or upload text and it works from that.

## The 5 routines

| Say this | Runs |
|---|---|
| "morning briefing" | `triggers/cos-morning.md` |
| "EOD" | `triggers/cos-eod.md` |
| "urgent check" | `triggers/cos-urgent.md` |
| "week ahead" | `triggers/cos-week.md` |
| "pulse check" | `triggers/cos-composer.md` |

## Slash commands (Gemini CLI only)

Gemini CLI turns `.gemini/commands/*.toml` into slash commands: `/cos`, `/cos-brief topic`, `/cos-find-time with Priya`, and so on. Run `/commands reload` after editing. The same recipes also live as plain files in `commands/`.

## Recipes in `commands/`

`cos`, `cos-brief`, `cos-delegate`, `cos-email-draft`, `cos-find-time`, `cos-focus`, `cos-followup`, `cos-spend`, `cos-thread`.

## Scheduling

Neither tool has a built-in scheduler. To run a routine at 7 AM, use cron or launchd to run `gemini -p "morning briefing"` from this folder. Keep it draft-only.

## Safety

It drafts, never sends. Your first run will ask permission before it edits files or runs commands: read each prompt. Keep it in this folder.

MIT — see [`../LICENSE`](../LICENSE).
