# Live Build Exercises

Follow these in order. Each one builds on the last. Don't skip ahead — the
later exercises depend on the earlier ones being in place.

Before you start, confirm from `02-SETUP-CHECKLIST.md`:
- [ ] You have a claude.ai Project created
- [ ] Gmail and Calendar Connectors show "Connected"

**Two ways to do Exercises 1 and 2:** fill in the templates yourself
(below), or let Claude interview you and write the files for you using
`04-DISCOVERY-PROMPTS.md`. If blank templates make you freeze up, use the
interview method instead — same result, different route. You can mix: do
one exercise by hand and the other by interview.

**One main file, everything else is optional.** `templates/custom-instructions-template.md`
is the one file that always goes into your Project's Custom Instructions
box — treat it like a CLAUDE.md for your Project. `voice-template.md` and
`config-template.md` are add-ons: attach them as separate knowledge files,
or merge their content into the main file. Either works.

---

## Exercise 1: Identity and priorities (10 min)

**Prefer to be interviewed instead of filling in blanks?** Use Prompt 2 in
`04-DISCOVERY-PROMPTS.md` in a plain Claude chat, then skip to step 5
below with the file it gives you.

1. Open `templates/custom-instructions-template.md`.
2. Fill in every bracket under **Who I Am** and **Who Matters Most**.
   Keep "Who Matters Most" to 3-5 people — don't list your whole org.
3. Fill in **What "Urgent" Means For Me** with one honest, specific
   sentence. Look at `examples/worked-example-anonymized.md` if you want
   to see what "specific" looks like.
4. Leave **How You Should Work** as-is for now — those rules are good
   defaults for everyone.
5. Paste the whole thing into your Project's **Custom Instructions** field
   and save.

**Checkpoint:** ask your Project "what do you know about me so far?" in a
new chat. It should reflect your name, role, and priority people back to
you. If it doesn't, check that you actually saved the instructions.

---

## Exercise 2: Voice (10 min)

**Prefer to be interviewed instead of filling in blanks?** Use Prompt 1 in
`04-DISCOVERY-PROMPTS.md` in a plain Claude chat with a few real writing
samples, then skip to step 5 below with the file it gives you.

1. Open `templates/voice-template.md`.
2. Circle/bold where you land on each spectrum (direct vs. warm, etc.).
3. Write your 3 rules in your own words.
4. Paste in the one real example you brought (from the setup checklist).
5. Add this whole filled-in section to the same custom instructions field,
   under a "My Voice" heading — or paste it as a second paragraph in the
   same box. Save.

**Checkpoint:** ask it to "draft a one-line Slack message telling my team
a meeting is moved to 3pm." Does it sound like something you'd actually
send? If not, that's useful information — go back and sharpen your voice
rules or add another real example.

---

## Exercise 3: Your first real task — morning briefing (15 min)

This is the moment it becomes real. Type this into your Project:

> "Give me a morning briefing: what's on my calendar today, and what in my
> inbox needs my attention. Sort by urgency using the categories in my
> instructions."

**What should happen:** it reads your actual connected Gmail and Calendar
and returns a categorized summary — not a generic "I can't access that"
response. If it asks for permission or shows a connector prompt, approve
it.

**If the categorization looks wrong:** that's expected on the first try.
Tell it directly — "that email from [person] should have been URGENT, not
FYI, because—" and explain why. Add "remember this" if you want it kept
automatically. This kind of correction is how it gets sharper over time —
see Exercise 4 below for where the correction actually goes.

**Optional stretch, if time allows:** ask "prep me for my next meeting
today" and see what context it pulls together from your calendar and
recent email with that attendee.

---

## Exercise 4: Teach it something with memory (10 min)

Custom instructions are for things that are always true. Memory is for
things you want it to remember going forward without rewriting your whole
instructions block. Try both of these:

1. **Explicit save.** Say: "Remember that [a real, low-stakes preference —
   e.g. 'I never want meeting invites scheduled before 9am' or 'when
   [person] emails, it's usually about budget, not urgent']." Then open a
   **new chat** in the same Project and ask "what do you remember about my
   meeting preferences?" — confirm it comes back without you repeating it.
2. **Correction-as-memory.** Go back to something it got wrong in Exercise
   3 (a miscategorized email, a tone that felt off). Instead of editing
   your custom instructions, just say "remember that—" and explain the
   correction the way you'd correct a person. Check in a new chat that it
   stuck.

**Why this matters:** this is what makes it feel like it's actually
learning you, instead of you maintaining a settings file forever. Small
corrections said once, stick. This is also how you'd track commitments day
to day — "remember I told Deja I'd send the report by Friday" — without
needing a separate tracking document.

**One thing to watch:** memory can be wrong too, or go stale — "remembered"
that a preference always applies when it was really a one-time thing. If
it recalls something that's no longer true, just say so ("that's no longer
the case, forget it" / "update that — it's actually X now").

---

## Exercise 5 (if time allows): One more real task

Pick one of these and try it:

- **"Draft a reply to [pick a real email in your inbox]."** Check: does it
  match your voice? Does it go to a draft, or did it try to send directly?
  (It should always draft, never send — if it tries to send, that's a
  custom-instructions gap, add the rule explicitly.)
- **"What meetings do I have this week that don't have a clear agenda?"**
- **"Find time with [a name from your calendar] next week."**

---

## What to do after today

- Use it for a real week. Notice every time the output feels off — too
  generic, wrong tone, missed something you cared about.
- For anything that's *always* true, add a sentence to your custom
  instructions. For anything that's a one-off correction or a thing to
  track (a commitment, a preference you just realized you have), just tell
  it to remember it. This is the actual workflow — it's never "done," it
  gets better through small corrections in whichever place fits.
- If you want to go further: look at `templates/config-template.md` for
  calendar/approval preferences and memory-based commitment tracking, and
  ask about connecting Slack if you didn't already.
