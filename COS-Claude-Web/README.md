# Personal Chief of Staff — claude.ai Project

The same Chief of Staff pattern as [`../COS-Claude-Code/`](../COS-Claude-Code/),
adapted for **claude.ai Projects** instead of Claude Code. No proprietary
or company-specific information is in this folder.

**You only edit one file: `YOUR-INFO.md`.** Everything else is copy-paste
— no markdown syntax, no brackets to hunt down, nothing technical.

## The 5-minute setup

1. Open `YOUR-INFO.md` and answer the questions in plain English (your
   name, role, company, the people who matter most, etc.). That's the
   only editing you do in this whole folder.
2. Go to [claude.ai/projects](https://claude.ai/projects) → **+ New
   Project**. Name it "Chief of Staff" or whatever you like.
3. Go to **Settings → Connectors** and turn on Gmail and Google Calendar
   (and Slack, if you use it). Sign in and approve access when asked.
4. Back on your Project page, click **Set project instructions**. Open
   `custom-instructions.md` in this folder, copy everything below its
   `---` line, and paste it in. Save.
5. On the Project page, find **Add content** (or a "+" button) in the
   knowledge section. Upload these 3 files exactly as they are, no
   editing needed:
   - `YOUR-INFO.md` (your answers from step 1)
   - `knowledge-voice.md`
   - `knowledge-briefings.md`
6. Go to **Settings → Capabilities** and make sure **Memory** is turned
   on.
7. Open a new chat inside your Project and type: **"morning briefing"**.
   It should read your calendar and email and give you a real, organized
   summary.

That's the whole setup. If something doesn't work, the most common cause
is step 3 or step 6 — double check both are actually turned on.

**Want to practice with fictional data?** Upload [`../COS-Workshop/scenarios/sales-leader.md`](../COS-Workshop/scenarios/sales-leader.md) as well (and use [`sample-YOUR-INFO.md`](../COS-Workshop/scenarios/sample-YOUR-INFO.md) instead of your own `YOUR-INFO.md`). Then say "morning briefing".

## What's in here

| File | Do you edit it? | What it does |
|---|---|---|
| `YOUR-INFO.md` | **Yes — this is the only one** | Your name, role, priority people, and rules, in plain English |
| `custom-instructions.md` | No — copy as-is | Goes into Custom Instructions; tells Claude to read `YOUR-INFO.md` for the details |
| `knowledge-voice.md` | No — copy as-is (optional 2-min upgrade inside) | How anything drafted on your behalf should sound |
| `knowledge-briefings.md` | No — copy as-is | The 5 briefing formats below |
| `knowledge-logbook.md` | No — copy as-is, and optional | A place to snapshot commitments if you want a backup outside of memory |

## The 5 briefings

Once set up, just say any of these in a chat inside your Project:

| Say this | You get |
|---|---|
| "morning briefing" | Calendar, email triage, Slack highlights, approvals, top 5 actions for today |
| "pulse check" | A quick check: next meeting, any new urgent items, what's happening in Slack |
| "EOD" or "end of day" | What happened today, anything you dropped, tomorrow's calendar, top 3 for tomorrow |
| "urgent check" | A late-day sweep for anything truly urgent — quiet by default |
| "week ahead" | Sunday-night preview of the coming week |

## Tracking things you've promised or delegated

Instead of a spreadsheet, just talk to it:
- "Remember that I promised the report to [person] by Friday"
- "What do I still owe people?"
- "Mark the report as done"

It remembers this using claude.ai's built-in Memory (make sure it's
turned on in Settings → Capabilities).

## If something in this README doesn't match your screen

claude.ai's menus move around sometimes. If you don't see "Connectors" or
"Skills" exactly where this guide says, look under **Settings** generally
— the features are usually there under a slightly different label.

## What this is not

- Not autonomous — it always drafts, never sends, without you reviewing
  first.
- Not tied to any specific company's tools — swap Gmail/Calendar/Slack for
  whatever you actually use.
- Not magic — if `YOUR-INFO.md` is left blank, it has nothing to
  prioritize by.

## For technical readers

If you want to understand the mechanics — how the trigger phrases map to
each section, why a logbook file became a memory-based system, or how to
turn a briefing into a proper claude.ai Skill instead of a knowledge file
— see [`../COS-Claude-Code/README.md`](../COS-Claude-Code/README.md) for
the underlying pattern this was adapted from, and the comments inside
`custom-instructions.md` for the claude.ai-specific adaptations.

## License

MIT — see [`../LICENSE`](../LICENSE).
