# What Is a Personal Chief of Staff?

## The problem

Every morning you probably do some version of this:

- Open email, scan for anything urgent
- Open calendar, check what meetings need prep
- Open Slack, check what you missed
- Try to remember what you promised someone yesterday, and what someone
  promised you

That's not one task. It's four tabs and a memory test, repeated daily. It's
tiring precisely because none of it is hard — it's just scattered and it
never stops.

## The idea

A **personal Chief of Staff** is a Claude Project — a persistent AI
workspace — that you set up once to know three things about you:

1. **Who you are** — your role, your priorities, the handful of people
   whose messages matter most, what "urgent" means for your job specifically
2. **How you communicate** — your tone, your sentence length, whether you
   lead with the ask or the context
3. **Where your real information lives** — your email, calendar, and (if
   you connect it) Slack, via **Connectors**

Once it knows those three things, you can ask it to do real work:
"What's on my plate today," "draft a reply to this," "prep me for my 2pm,"
"what have I dropped that I shouldn't have."

It doesn't replace your judgment. It removes the *assembly* work — finding,
sorting, and summarizing — so you spend your attention on the decision, not
the search.

## What makes this different from just asking Claude a question

Normally, every time you open a chat, you're starting from zero — Claude
knows nothing about you until you tell it. A **Project** changes that:

- **Custom instructions** persist across every conversation in that
  Project. You don't re-explain your role or your priority people every
  time.
- **Connectors** give it live, read access to real systems (your inbox,
  your calendar) instead of you copy-pasting content in.
- **Memory** lets it remember specific things it learns *during* a
  conversation — a correction you made, a commitment you mentioned, a
  preference you stated in passing — without you adding it to custom
  instructions yourself. You can also just tell it "remember this."
- The combination means a two-word prompt like "morning briefing" can
  produce a real, personalized answer — because the context is already
  loaded.

## Custom instructions vs. memory — which one to use

These solve different problems. Knowing which one to reach for matters:

| | Custom instructions | Memory |
|---|---|---|
| What it holds | Stable facts about you — role, priority people, voice, standing rules | Things that happened — a correction, a commitment, a one-off preference |
| How it gets written | You write/paste it yourself, deliberately | It writes itself as you talk to it, or you say "remember this" |
| Good for | "I am the VP of Ops," "always draft, never send" | "I promised Deja the report by Friday," "actually, ignore emails from that newsletter" |
| Changes how often | Rarely — you revisit it occasionally | Constantly — it accumulates as you use it |

Rule of thumb: if it's true every day, it goes in custom instructions. If
it's true *this week* or came up once in conversation, let memory hold it.

## What it is not

- It is not autonomous. In the pattern we're teaching today, it never sends
  an email or a message on your behalf without you seeing and approving it
  first. It drafts. You decide.
- It is not a company-wide tool with access to other people's data. Your
  Project only sees what YOUR connected accounts can see.
- It is not magic. If you don't tell it what matters to you, it will guess
  — and generic guesses are exactly the kind of unhelpful output we're
  trying to avoid. The setup work today (15-20 minutes) is what makes the
  difference.

## The four pieces you'll build today

| Piece | What it answers | Where it lives |
|---|---|---|
| Identity & priorities | "Who is this for, and what matters to them?" | Custom instructions |
| Voice | "How should anything drafted sound?" | Custom instructions |
| Live data access | "What's actually going on right now?" | Connectors (Gmail, Calendar) |
| Memory | "What has it learned from using it?" | Memory (accumulates automatically) |

By the end of this session, you'll have all four, and you'll have run one
real task against your own inbox and calendar.
