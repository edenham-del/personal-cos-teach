# Personal Chief of Staff — Gemini (web)

The same Chief of Staff pattern as [`../COS-Claude-Web/`](../COS-Claude-Web/), set up in **Gemini** in your browser. No terminal, no coding.

**You only edit one file: `YOUR-INFO.md`.** Everything else is copy-paste.

## The 5-minute setup

1. Open `YOUR-INFO.md` and answer the questions in plain English. That is the only file you edit.
2. Go to [gemini.google.com](https://gemini.google.com) → **Explore Gems** → **New Gem**. Name it "Chief of Staff".
3. In **Instructions**, open `custom-instructions.md` in this folder, copy everything below its `---` line, and paste it in.
4. Under **Knowledge**, click **Add files** and upload these 3 files exactly as they are:
   - `YOUR-INFO.md` (your answers)
   - `knowledge-voice.md`
   - `knowledge-briefings.md`
   - (optional) `knowledge-logbook.md`
5. **Save** the Gem, then open it and start a chat.
6. *(Optional)* In Settings → Apps / Extensions, connect Gmail and Google Calendar. Skip this to stay on uploaded files only.
7. Type: **"morning briefing"**.

**Gems cannot remember between chats.** Keep open loops in `knowledge-logbook.md`: ask the Gem for an updated copy at the end of a chat, save it, and replace the file under Knowledge. Gem knowledge files are read-only to the Gem.

## What's in here

| File | Do you edit it? | What it does |
|---|---|---|
| `YOUR-INFO.md` | **Yes, the only one** | Your name, role, priority people, and rules, in plain English |
| `custom-instructions.md` | No, paste as-is | Goes into the Gem instructions; tells the assistant to read `YOUR-INFO.md` |
| `knowledge-voice.md` | No (optional 2-minute upgrade inside) | How drafts written on your behalf should sound |
| `knowledge-briefings.md` | No | The 5 briefing formats |
| `knowledge-logbook.md` | Optional | A snapshot of your open loops, for tools without memory |

## The 5 briefings

| Say this | You get |
|---|---|
| "morning briefing" | Calendar, email triage, highlights, approvals, top 5 actions |
| "pulse check" | Next meeting, anything new and urgent |
| "EOD" | What happened, what you dropped, top 3 for tomorrow |
| "urgent check" | A late-day sweep, quiet by default |
| "week ahead" | A preview of the coming week |

## Tracking promises

Say: "Remember that I promised the pricing recap to [person] by Friday." Later: "What do I still owe people?" Uses Gemini's saved info (Settings → Personal context).

## Safety

It drafts, never sends. Do not paste anything into a public tool that your company's policy forbids. If your workplace only allows one assistant, use that one.

## If menus don't match your screen

Gemini changes its menus often. Look under Settings for the same feature under a slightly different name.

Want scheduled routines and slash-style commands? See [`../COS-Gemini-CLI/`](../COS-Gemini-CLI/).

MIT — see [`../LICENSE`](../LICENSE).
