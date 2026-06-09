# Techstars Application Coach — a Claude Skill

A [Claude Skill](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills) that coaches founders through writing a strong Techstars accelerator application and turns it into a submittable document.

It works two ways:

- **Coach mode** — builds answers from scratch, one question at a time, asking you for the raw specifics each question needs.
- **Critique mode** — takes a draft you paste in, names the single biggest weakness of each answer, and rewrites it stronger using your own facts.

The skill covers all **11 application questions** (problem, product, team, traction, business model / TAM, target audience / ICP, competitors, competitive advantage, why now, customer acquisition, milestones), enforces the form's character limits, and produces a finished `.docx` (optionally a Google Doc) you can paste straight into the portal.

It is based on the Techstars Application Guide by Andres Barreto (Techstars alum and Managing Director).

## What's in here

```
techstars-application-coach/
├── SKILL.md                      # the workflow: modes, writing style, the quality bar
└── references/
    ├── questions.md              # the full rubric for all 11 questions + character limits
    ├── bottom-up-tam.md          # the proper bottom-up TAM method (question 5)
    └── moats.md                  # honest competitive-advantage / moat coaching (question 8)
```

`SKILL.md` governs the workflow; the reference files carry the substance and are loaded only when a given question needs them.

## The one idea behind it

Almost every weak application answer fails the same way: it's generic when it should be specific, and it asserts when it should show evidence. The skill's whole job is to drag every answer from vague claim to specific, quantified, evidence-backed detail — and to make it fit the character limit.

## Install on Claude

> Skills require **Code execution and file creation** to be enabled. They're available on Free, Pro, Max, Team, and Enterprise plans.

### Option A — Claude.ai (web or desktop)

1. Download `techstars-application-coach.zip` from this repo (or zip the `techstars-application-coach/` folder yourself — see note below).
2. In Claude, open **Settings → Capabilities** and make sure **Code execution and file creation** is on.
3. Go to **Customize → Skills** (on some plans this is under **Settings → Capabilities → Skills**).
4. Click **Upload skill** (the **+** button) and select the zip.
5. Claude reads `SKILL.md` and lists the skill. Toggle it **on**.

Start a new chat and trigger it naturally, e.g. *"Help me apply to Techstars"* or *"Review my Techstars application answers."*

### Option B — Claude Code

Skills follow the [Agent Skills open standard](https://code.claude.com/docs/en/skills). Drop the skill folder into either location:

```bash
# Personal (available in every project)
mkdir -p ~/.claude/skills
cp -r techstars-application-coach ~/.claude/skills/

# — or — project-scoped (checked in with your repo)
mkdir -p .claude/skills
cp -r techstars-application-coach .claude/skills/
```

Claude Code loads it automatically when a request matches, or you can invoke it directly.

### Zipping it yourself

The zip's **root must be the skill folder itself** (not a parent folder), and the folder name must match the skill name:

```bash
zip -r techstars-application-coach.zip techstars-application-coach
```

So the archive contains `techstars-application-coach/SKILL.md`, not `some-folder/techstars-application-coach/SKILL.md`.

## Scope

**In:** coaching the 11 questions, critiquing a draft, bottom-up TAM, sharpening an ICP, producing the finished document.

**Out:** pitch decks, investor data rooms, first-round interview prep, and submitting the application itself (you do that at [techstars.com/apply](https://www.techstars.com/apply)).

## Credit

Methodology adapted from the Techstars Application Guide by Andres Barreto. This packaging is provided under the MIT License (see `LICENSE`); the underlying guidance and the Techstars name belong to their respective owners.
