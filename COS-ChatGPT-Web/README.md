# Personal Chief of Staff — ChatGPT (web)

The same Chief of Staff pattern as [`../COS-Claude-Web/`](../COS-Claude-Web/), set up in **ChatGPT** in your browser. No terminal, no coding.

**You only edit one file: `YOUR-INFO.md`.** Everything else is copy-paste.

## The 5-minute setup

1. Open `YOUR-INFO.md` and answer the questions in plain English. That is the only file you edit.
2. In [chatgpt.com](https://chatgpt.com), open the sidebar → **Projects** → **New project**. Name it "Chief of Staff".
3. Open the project's settings (the **⋯** menu) and choose **Instructions**. Open `custom-instructions.md` in this folder, copy everything below its `---` line, paste it, and save.
4. In the project, use **Add files** and upload these 3 files exactly as they are:
   - `YOUR-INFO.md` (your answers)
   - `knowledge-voice.md`
   - `knowledge-briefings.md`
   - (optional) `knowledge-logbook.md`
5. Turn on **Memory** in Settings → Personalization, so open loops carry between chats.
6. *(Optional)* In Settings → Apps, connect Gmail, Google Calendar or Slack. Skip this if you want to stay on pasted text or uploaded files only.
7. Start a new chat inside the project and type: **"morning briefing"**.

**No Projects on your plan?** Use a Custom GPT instead: **Explore GPTs → Create → Configure**. Paste the instructions into **Instructions** and upload the same files under **Knowledge**. Custom GPTs cannot use Memory, so keep open loops in `knowledge-logbook.md` and re-upload it when it changes.

## What's in here

| File | Do you edit it? | What it does |
|---|---|---|
| `YOUR-INFO.md` | **Yes, the only one** | Your name, role, priority people, and rules, in plain English |
| `custom-instructions.md` | No, paste as-is | Goes into the Project instructions; tells the assistant to read `YOUR-INFO.md` |
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

Say: "Remember that I promised the pricing recap to [person] by Friday." Later: "What do I still owe people?" Uses ChatGPT Memory (Settings → Personalization → Memory).

## Safety

It drafts, never sends. Do not paste anything into a public tool that your company's policy forbids. If your workplace only allows one assistant, use that one.

## If menus don't match your screen

ChatGPT changes its menus often. Look under Settings for the same feature under a slightly different name.

Want scheduled routines and slash-style commands? See [`../COS-ChatGPT-Codex/`](../COS-ChatGPT-Codex/).

MIT — see [`../LICENSE`](../LICENSE).
