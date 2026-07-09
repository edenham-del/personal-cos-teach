# Facilitator Guide — "Build Your Own Personal Chief of Staff"

Internal use only. This file is for you, the presenter — not for attendees.
Nothing in this file (or anywhere else in this folder) contains real company,
person, or client information. Everything attendee-facing uses a fictional
persona ("Jordan Lee") so nobody's actual inbox, calendar, or org chart is
ever shown on screen.

## Session at a glance (60 minutes)

| Time | Segment | Goal |
|---|---|---|
| 0:00–0:10 | Concept: what is a personal CoS | Attendees understand the pattern, not just the demo |
| 0:10–0:15 | Setup checkpoint | Everyone has claude.ai open, Project created, connectors on |
| 0:15–0:32 | Live build: Part 1 (identity + voice) | Everyone has working custom instructions |
| 0:32–0:44 | Live build: Part 2 (first real task — morning briefing) | Everyone runs a real scan against their own inbox/calendar |
| 0:44–0:52 | Live build: Part 3 (teach it with memory) | Everyone saves and recalls one thing via memory |
| 0:52–0:58 | Showcase + advanced teasers | 2-3 volunteers share what came back; mention commitment tracking, drafting, Slack |
| 0:58–1:00 | Close | Where to find the templates, how to keep iterating |

Note: this adds a memory segment to the original 4-part build, so Parts 1
and 2 have each been trimmed by a few minutes. If the room is running
behind by the time you reach Part 3, it's fine to compress it to a single
"remember this" demo (2 min) rather than cut it — memory is one of the
things that makes this feel different from a one-off ChatGPT prompt, so
it's worth protecting some time for it, even short.

## Pre-work (send 2-3 days before session)

Send attendees `02-SETUP-CHECKLIST.md` ahead of time. The single biggest risk
to a live session is people stuck on account/connector setup during your
15 minutes of talk time. Ask them to arrive with:
- A claude.ai account (Pro/Team/Enterprise — Projects require a paid plan)
- Gmail and Google Calendar connectors already authorized once (even just
  clicking through the OAuth screen ahead of time saves minutes)

## Segment 1: Concept (10 min)

**Open with the problem, not the tool.** Ask the room: "How many of you
start the day by opening 4 tabs — email, calendar, Slack, and a to-do list —
just to figure out what actually matters today?" Most hands go up. That
triage tax is the thing a personal CoS removes.

**Define it simply:** A personal Chief of Staff is a Claude Project you set
up once with four things:
1. **Who you are and what you care about** (your role, your priority people,
   your thresholds for "urgent")
2. **How you sound** (your writing voice, so anything drafted sounds like
   you, not like a generic assistant)
3. **Access to your actual tools** (Gmail, Calendar, Slack — via Connectors)
   so it can read real context instead of you pasting it in every time.
4. **Memory** — so corrections and commitments stick without you having to
   rewrite your instructions every time something comes up once.

Keep the concept segment's explanation of memory short and concrete; it
lands better as "you correct it once, it remembers" than as a technical
explanation. Save the depth for Part 3.

**Show, don't just tell.** If comfortable, do a *quick* live demo using
your own real CoS project (not the templates) — run a "scan" and show the
briefing that comes back. Keep this under 90 seconds; the point is to prove
it's real, not to walk through every field. Do not screen-share your inbox
contents in detail — narrate the shape of the output ("it grouped my email
into urgent / needs response / FYI, and flagged two things due today") more
than reading exact subject lines aloud.

**Key framing line:** "You're not writing code. You're writing down how you
already think, once, so the model can act with your judgment instead of
generic judgment."

## Segment 2: Setup checkpoint (5 min)

Walk the room through `02-SETUP-CHECKLIST.md` live, step by step, screen-
sharing your own screen doing it with a throwaway/demo account if possible
(so what's on screen is not your real Project). Confirm out loud:
- "Everyone has a Project created?"
- "Everyone sees Gmail and Calendar as connected sources?"

Do not proceed until most of the room confirms. This is the segment most
likely to run long — budget slack elsewhere, not here.

## Segment 3: Live build, Part 1 — Identity + Voice (20 min)

Have attendees open `templates/custom-instructions-template.md` and
`templates/voice-template.md` side by side with their claude.ai Project's
"Custom Instructions" field.

Walk through filling in, in this order (matches `03-EXERCISES.md` Exercise 1
and 2):
1. Name, role, company (1 line each — this is the easy win, builds momentum)
2. Priority people — 3 to 5 names/relationships max. Say explicitly: "Don't
   try to map your whole org chart. Pick the 5 people whose messages you'd
   drop everything for."
3. Voice — the fill-in-the-blank sliders (direct vs. warm, short vs.
   detailed, formal vs. casual) plus one real sentence they've written
   before, so the model has a concrete sample instead of just adjectives.

Paste both into the Project's custom instructions field. Have them save and
ask it one throwaway question ("what do you know about me so far?") to
confirm it absorbed the identity — this is a good checkpoint before moving
to real data access.

## Segment 4: Live build, Part 2 — First real task (15 min)

This is the payoff moment. Have attendees type the prompt in
`03-EXERCISES.md` Exercise 3 — a morning briefing request — into their
Project. It will pull from their real, connected Gmail/Calendar.

**Facilitator note:** this is the point in the session with the least
control — real data means real surprises. Prime the room: "It's going to
show YOU your own inbox summary — nobody else can see it. If it categorizes
something wrong, that's a one-line fix in your instructions, not a bug."

Circulate during this segment rather than talking — this is where people
get stuck on connector permissions or vague prompts.

## Segment 5: Live build, Part 3 — Teach it with memory (8 min)

This is the segment that makes the difference between "a nice demo" and
"something that gets better the more I use it." Have attendees follow
`03-EXERCISES.md` Exercise 4:

1. Say "remember that [a real, low-stakes preference]."
2. Open a **new chat** in the same Project (important — this proves it's
   not just conversation history, it's actually persisted) and ask what it
   remembers.
3. If time allows, have them go back to something Part 2 got wrong and
   correct it via "remember that—" instead of editing custom instructions.

**Key framing line:** "Custom instructions is the stuff that's always
true. Memory is everything you'd otherwise have to repeat. The commitment-
tracking use case — 'remember I told Deja I'd send this by Friday' — lives
here, not in your settings."

**Facilitator note:** if the room is short on time, compress this to a
single live demo on your screen (using a throwaway fact, not personal data)
rather than skip it outright — it's the segment most likely to make someone
say "oh, THAT'S useful" out loud.

## Segment 6: Showcase + advanced teasers (6 min)

Ask for 2-3 volunteers to share (verbally, not screen-share, to protect
their own inbox privacy) what surprised them about the output. Then tease
what's possible next, pointing at `examples/worked-example-anonymized.md`:
- Drafting replies in your voice (not just summarizing)
- Tracking things you've delegated or committed to, using memory
- Meeting prep — pulling context on attendees before a call
- Connecting Slack so it can also read/draft there

Explicitly say: "These templates are v1. The real system gets better as you
correct it — some corrections belong in your instructions, some just need
you to say 'remember this.'"

## Segment 7: Close (2 min)

Point people to the public GitHub repo (fill in the URL here once
published: `github.com/siddsdixit/<repo-name>`). Say explicitly: "Open this
on your own laptop or phone later, and the templates and exercises are all
there — you don't need me in the room to keep going." Remind them:
everything they filled in stays in THEIR claude.ai account. You do not
collect or see anyone's filled-in instructions, and this repo itself
contains nothing proprietary — it's safe to share outside the company too.

## Anticipated questions

- **"Does this see my email forever / train on it?"** No — Connectors give
  the model live read access during your session; check your org's specific
  data-retention answer with IT/security before the session so you can
  answer definitively.
- **"Can it send things without me approving?"** Not by default — the
  pattern in these templates always drafts, never sends. Emphasize this;
  it's a safety rule worth repeating twice.
- **"What if I don't want it reading everything in my inbox?"** Connectors
  can typically be scoped/revoked; point them to their account's connector
  settings.
- **"Can other people see what it remembers about me?"** No — memory is
  scoped to your own account/Project, same as custom instructions. Confirm
  the exact scope (per-Project vs. account-wide) with IT before the
  session so you can answer precisely, since this can vary.
- **"What if it remembers something wrong, or something that's no longer
  true?"** Tell it directly — "forget that" or "that's changed, update it"
  — same as correcting a person. Worth demoing this once live so people
  see it's not a one-way ratchet.
- **"Is this the same as what [CTO] uses?"** Answer honestly at whatever
  level of detail you're comfortable with — the templates here are
  deliberately generic and don't reveal specifics of any real production
  setup.

## Things to double check before presenting

- [ ] Confirm with IT/security what you're allowed to say about data
      handling for Connectors in your org
- [ ] Confirm Projects + Connectors are available on attendees' license tier
- [ ] Test the whole flow once end-to-end on a fresh/demo account the week
      before, so you hit setup friction before attendees do
- [ ] Decide whether you'll do the 90-second live demo of your real CoS —
      if you do, rehearse exactly what you'll say out loud vs. just show
