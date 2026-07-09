# Build Your Own Personal Chief of Staff

A teaching kit for setting up a personal AI Chief of Staff using
**claude.ai Projects** — no coding required. Built for a company AI Week
session; shared publicly so anyone can run the same session or just build
their own.

This repo contains no proprietary or company-specific information. Every
example uses a fictional persona ("Jordan Lee, VP of Operations at Acme
Corp"). Fork it, use it internally, adapt it for your own team.

## What you'll build

A claude.ai Project that knows:
1. **Who you are** — your role and the handful of people whose messages
   matter most
2. **How you write** — so anything it drafts sounds like you
3. **Your real email and calendar** — via Connectors, so it can act on
   real context instead of things you paste in
4. **What it's learned from you** — via Memory, so corrections and
   commitments stick without you rebuilding your setup every time

By the end, you can ask it things like "give me a morning briefing," "draft
a reply to this," or "remember that I promised this by Friday" — and get a
real, personalized answer back.

## Two ways to use this repo

### Option A — Just want to build your own, right now

1. Go to [claude.ai](https://claude.ai) and create a new **Project**
   (requires a paid plan — Pro, Team, or Enterprise).
2. Turn on the **Gmail** and **Google Calendar** Connectors for that
   Project (Settings → Connectors, or inside the Project itself, depending
   on your workspace).
3. Open [`03-EXERCISES.md`](03-EXERCISES.md) and follow it top to bottom.
   It'll point you at the templates in [`templates/`](templates/) as you
   go, and at [`04-DISCOVERY-PROMPTS.md`](04-DISCOVERY-PROMPTS.md) if you'd
   rather be interviewed by Claude than fill in blanks yourself.
4. Optional: skim [`01-WHAT-IS-A-PERSONAL-COS.md`](01-WHAT-IS-A-PERSONAL-COS.md)
   first if you want the concept explained before diving in.

Point your browser at this repo, keep it open in a second tab, and work
through the files in order. That's the whole "setup."

### Option B — Running this as a live workshop for a group

Use [`00-FACILITATOR-GUIDE.md`](00-FACILITATOR-GUIDE.md) — a full run of
show for a 60-minute hands-on session, with timing, talk track, and
anticipated questions. Send [`02-SETUP-CHECKLIST.md`](02-SETUP-CHECKLIST.md)
to attendees a few days ahead so account/connector setup doesn't eat into
your session time.

A ready-to-present slide deck covering the same material is in
[`slides/`](slides/) — see [`slides/README.md`](slides/README.md) for how
to open/present it.

## File guide

See [`FILE-GUIDE.md`](FILE-GUIDE.md) for the full file tree, what each file
does, and the build order end-to-end. Short version:

| File | What it's for |
|---|---|
| [`01-WHAT-IS-A-PERSONAL-COS.md`](01-WHAT-IS-A-PERSONAL-COS.md) | The concept, in plain language — start here if you're new to this |
| [`02-SETUP-CHECKLIST.md`](02-SETUP-CHECKLIST.md) | Account and Connector setup, do this first |
| [`03-EXERCISES.md`](03-EXERCISES.md) | Step-by-step build — the main event |
| [`04-DISCOVERY-PROMPTS.md`](04-DISCOVERY-PROMPTS.md) | Prompts that let Claude interview you and write your voice/identity files for you, instead of filling in blanks |
| [`templates/`](templates/) | Fill-in-the-blank files for custom instructions, voice, and preferences |
| [`examples/`](examples/) | A fully filled-out fictional example (Jordan Lee, Acme Corp) so you can see a finished setup |
| [`00-FACILITATOR-GUIDE.md`](00-FACILITATOR-GUIDE.md) | Run-of-show for presenting this as a live session |
| [`slides/`](slides/) | Slide deck covering the same material |

## What this is not

- Not autonomous — every pattern in this kit drafts, never sends, without
  your review.
- Not a data pipeline into any shared system — a Project only sees what
  YOUR connected accounts can see, and Memory is scoped to your own
  account.
- Not specific to any one company's tools or org chart — everything here
  is intentionally generic so you can adapt it to your own role.

## License

MIT — see [`LICENSE`](LICENSE). Free to use, fork, and adapt for your own
team or company.

Built by [Siddharth Dixit](https://github.com/siddsdixit).
