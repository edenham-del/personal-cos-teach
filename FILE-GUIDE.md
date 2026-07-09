# File Guide — What's In This Repo, and How to Use It

Everything in one place: what each file is, who it's for, and when to open
it. If you only read one section, read "Which path am I on?" below.

## Tree

```
Personal_COS_Teach/
├── README.md                        Start here — repo overview, quick links
├── LICENSE                          MIT license
├── FILE-GUIDE.md                    This file
│
├── 00-FACILITATOR-GUIDE.md          FOR THE PRESENTER ONLY — run of show, timing, talk track
├── 01-WHAT-IS-A-PERSONAL-COS.md     FOR ATTENDEES — the concept, plain language
├── 02-SETUP-CHECKLIST.md            FOR ATTENDEES — do this before the session
├── 03-EXERCISES.md                  FOR ATTENDEES — the live-build steps, in order (the main event)
├── 04-DISCOVERY-PROMPTS.md          FOR ATTENDEES — copy-paste prompts that let Claude interview you
│
├── templates/                       Fill-in-the-blank source material for Exercises 1-2
│   ├── custom-instructions-template.md   THE MAIN FILE — always goes in Custom Instructions
│   ├── voice-template.md                 Add-on — attach separately, or merge into the main file
│   └── config-template.md                Add-on, optional — same as above, add later if needed
│
├── examples/
│   └── worked-example-anonymized.md      A fully filled-out fictional example (Jordan Lee, Acme Corp)
│
└── slides/                          Presentation decks — same 24-slide content, two formats
    ├── index.html                        Open in any browser, arrow keys to navigate, N for speaker notes
    ├── Build-Your-Own-Personal-CoS.pptx  Editable PowerPoint version, notes included
    └── README.md                         How to open/present either deck
```

## Which path am I on?

**I'm attending the live session** → You need, in order: `02-SETUP-CHECKLIST.md`
(before it starts) → `03-EXERCISES.md` (during — this drives everything) →
`04-DISCOVERY-PROMPTS.md` only if you want to be interviewed instead of
filling in `templates/` by hand. Skim `01-WHAT-IS-A-PERSONAL-COS.md` if
you want the concept explained first.

**I'm running this as a workshop for my own team** → Start with
`00-FACILITATOR-GUIDE.md` — it has the timing, talk track, and points to
every other file at the right moment. Present from `slides/`. Send
`02-SETUP-CHECKLIST.md` to attendees a few days ahead.

**I just want to build my own personal CoS, alone, no session** → Read
`01-WHAT-IS-A-PERSONAL-COS.md`, do `02-SETUP-CHECKLIST.md`, then work
through `03-EXERCISES.md` top to bottom by yourself. The slides are
optional in this path.

**I want to see a finished example before I start** → `examples/worked-example-anonymized.md`.

## What each file actually does

| File | Type | Read it when... |
|---|---|---|
| `README.md` | Overview | You just landed on the repo and want the 30-second summary |
| `00-FACILITATOR-GUIDE.md` | Presenter script | You are presenting this to a group |
| `01-WHAT-IS-A-PERSONAL-COS.md` | Concept | You want to understand the idea before touching anything |
| `02-SETUP-CHECKLIST.md` | Checklist | Before you open claude.ai — account, Project, Connectors |
| `03-EXERCISES.md` | Step-by-step | You're ready to actually build — this is the spine of the whole kit |
| `04-DISCOVERY-PROMPTS.md` | Copy-paste prompts | You'd rather be interviewed by Claude than fill in a blank template |
| `templates/custom-instructions-template.md` | **Main file** — fill-in-the-blank | Exercise 1 — identity, priorities, standing rules. This is the one file that always goes in the Project's Custom Instructions box, same role as a CLAUDE.md/agent.md |
| `templates/voice-template.md` | Add-on — fill-in-the-blank | Exercise 2 — voice and tone. Attach as a separate knowledge file, or merge into the main file |
| `templates/config-template.md` | Add-on, optional | You want calendar/approval prefs or commitment tracking beyond the basics. Attach separately or merge in |
| `examples/worked-example-anonymized.md` | Reference | You want to see a finished, filled-out setup before doing your own |
| `slides/index.html` | Presentation | You're presenting live and want a browser-based deck with speaker notes |
| `slides/Build-Your-Own-Personal-CoS.pptx` | Presentation | You need to edit slides in PowerPoint/Keynote/Google Slides |

## The actual build order (what feeds what)

```
02-SETUP-CHECKLIST.md
        │  (claude.ai account + Project + Connectors ready)
        ▼
03-EXERCISES.md  Exercise 1 ──┐
        │                     │  EITHER fill in templates/ by hand
        │                     │  OR run 04-DISCOVERY-PROMPTS.md Prompt 2
        ▼                     │  → both produce content for Custom Instructions
03-EXERCISES.md  Exercise 2 ──┤
                               │  EITHER fill in templates/voice-template.md
                               │  OR run 04-DISCOVERY-PROMPTS.md Prompt 1
                               ▼
                     Paste/attach into claude.ai Project → Custom Instructions
                               │
                               ▼
03-EXERCISES.md  Exercise 3   (first real task — morning briefing, uses Connectors)
                               │
                               ▼
03-EXERCISES.md  Exercise 4   (memory — save + recall a correction or commitment)
                               │
                               ▼
03-EXERCISES.md  Exercise 5   (optional — one more real task)
```

Nothing here needs to be built or installed. There's no code to run — every
"build" step is filling in text and pasting it into claude.ai.
