# Discovery Prompts — Let Claude Interview You

Filling in a template by hand (`templates/custom-instructions-template.md`,
`templates/voice-template.md`) works, but some people freeze up staring at
a blank "what's your voice?" field. This is the alternative path: paste
these prompts into a **regular Claude chat** (not your Project — do this
part first, in any claude.ai chat window) and let Claude do the interview
and the writing. You end up with finished `.md` files to download and
attach to your Project instead of filling out a form yourself.

Use whichever path you prefer — hand-filled templates or this interview
method — they arrive at the same place. Some people do one section by hand
and one by interview. Both are fine.

## How this fits with the rest of the session

1. Run one or both prompts below in a plain Claude chat.
2. Review what comes back — correct anything that's off before you save it.
3. Ask Claude to output it as a downloadable `.md` file (see the note at
   the end of each prompt).
4. Attach that file to your Project (Project → Add content / knowledge, or
   paste its contents into custom instructions — see
   `02-SETUP-CHECKLIST.md` for where that lives in your workspace).

---

## Prompt 1: Find my voice

**What you need before running this:** paste in 3-5 real things you've
written — emails, Slack messages, docs, whatever you have handy. The more
real examples, the better the result. Quantity beats a perfect selection —
don't spend time curating, just paste what you can find quickly.

**The prompt:**

```
I want you to figure out my writing voice by analyzing real examples I
give you, then write it up as a clear style guide I can hand to another
AI assistant so it writes like me.

Here are several things I've actually written. Read all of them before
you say anything:

[PASTE EXAMPLE 1]

[PASTE EXAMPLE 2]

[PASTE EXAMPLE 3 — add more if you have them]

Now do this:
1. Tell me what you notice about my voice — sentence length, formality,
   how I open and close messages, whether I use bullet points, how direct
   I am, any phrases or habits that repeat.
2. Ask me up to 3 clarifying questions if something is ambiguous or
   inconsistent across examples (for example, if I sound different in
   different examples, ask which is closer to how I want to sound by
   default, or whether it depends on the audience).
3. Once I've answered, write a finished voice guide in markdown, following
   this structure:
   - A short "Persona" paragraph (3-4 traits, plain language)
   - "Core Rules" — 4-6 concrete, checkable rules (not vague adjectives)
   - A short real example from what I gave you, kept as-is, labeled as a
     reference sample
   - If my voice changes by audience (e.g. leadership vs. team vs.
     external), a short "Modes" section for that — only include this if
     you actually saw evidence of it in my examples, don't invent it
4. Output the finished guide as a markdown code block so I can copy it
   directly, and title it "voice.md".
```

**After it responds:** read the finished guide once. If anything feels
wrong or too generic, say so directly — "rule 2 doesn't actually sound like
me, here's why" — and ask it to revise before you save the file.

---

## Prompt 2: Find my priorities and identity

**What you need before running this:** nothing prepared — this one works
purely as an interview. Optional: have a rough sense of your top 5 people
and what "urgent" means in your job, since it'll ask.

**The prompt:**

```
I want to set up a personal AI assistant (a Chief of Staff) and I need to
define who I am and what matters to me so it can prioritize correctly.
Interview me with short, one-at-a-time questions — don't ask everything
at once. Cover:

1. My name, role, and company/team
2. The 3-5 people whose messages should always get flagged first (ask me
   who they are and why — manager, key client, direct report, etc.)
3. What "urgent" actually means in my specific job — push me for something
   concrete and specific, not generic ("time-sensitive things") — if my
   first answer is vague, ask a follow-up example question until we get
   to something I could actually apply
4. How I want things categorized when it scans my email or messages (offer
   me a default like URGENT / NEEDS RESPONSE / FYI / CAN WAIT and ask if I
   want to change it)
5. Anything it should NEVER do automatically (e.g. never send without my
   review, never draft anything about a specific sensitive topic)

Ask one question at a time and wait for my answer before moving to the
next. Once you have all 5, write it up as a finished markdown document
titled "identity.md" with clear headers matching the 5 areas above, output
as a code block I can copy directly.
```

**After it responds:** this file becomes the "Who I Am" / "Who Matters
Most" / "What You Can Do" / "How You Should Work" sections of your custom
instructions. You can either paste its content directly into the custom
instructions field, or attach it as a knowledge file and add one line to
custom instructions saying to follow it.

---

## Turning the output into files you attach

Once Claude gives you a finished markdown block for either prompt:

1. Copy the contents of the code block.
2. Paste into a plain text editor (Notes, TextEdit, Notepad — anything) and
   save it as `voice.md` or `identity.md`.
3. In your claude.ai Project, look for **Add content** / **Knowledge** (the
   exact label depends on your workspace) and upload the file.
4. Alternatively, skip the file entirely and paste the content straight
   into the **Custom Instructions** box — either works. Uploading as a
   file is nicer if the document is long, since custom instructions boxes
   can feel cramped.

## Why interview-style can work better than a blank template

Most people can react to a draft ("no, I'm actually more direct than
that") far more easily than they can generate one from nothing. This
method uses Claude to produce a first draft grounded in real examples,
which you then correct — rather than asking you to describe your own voice
in the abstract, which is a surprisingly hard thing to do cold.
