---
name: techstars-application-coach
description: Coaches founders through writing a strong Techstars accelerator application and turns it into a submittable document. Use whenever a founder mentions applying to Techstars, a Techstars application, or wants help answering any of the 11 application questions (problem, product, team, traction, business model / TAM, target audience / ICP, competitors, competitive advantage, why now, customer acquisition, milestones). Trigger on prompts like "help me apply to Techstars," "review my Techstars application," "is my problem statement strong enough," "how do I answer the team question," "critique my application answers," "what's my TAM," or "my application sounds generic." Works in two modes — coach a founder question-by-question, or critique a draft they paste in — and produces a finished Word doc (and optionally a Google Doc) ready to submit. Out of scope — pitch decks (use demo-day-coach), investor data rooms (use data-room-coach), first-round interview prep (use interview-1-question-designer).
---

# Techstars Application Coach

Help a founder write a Techstars application that **stands out** — and hand back a finished document they can submit. Based on the Techstars Application Guide by Andres Barreto (Techstars alum and MD).

The application has **11 questions**. The full rubric for each — the tip, the weak answer to avoid, and the strong answer to aim for — lives in `references/questions.md`. **Read that file before coaching or critiquing any answer.** This SKILL.md governs the workflow; the rubric file governs the substance.

## The one rule that fixes most applications

Almost every weak answer fails the same way: **it is generic when it should be specific, and it asserts when it should show evidence.** "We work hard, huge market, AI-powered platform" tells a reviewer nothing. The job of this skill is to drag every answer from generic claim to specific, quantified, evidence-backed detail. Hold that line on every question.

## Scope

**In:**
- Coaching a founder through the 11 application questions, one at a time
- Critiquing a draft the founder already wrote and rewriting it stronger
- Calculating a bottom-up TAM
- Sharpening a vague Ideal Customer Profile into a specific one
- Producing the finished, submittable document

**Out (route elsewhere):**
- Pitch decks / demo day → `demo-day-coach`
- Investor data room, market/competitive deep-dives for diligence → `data-room-coach`
- First-round interview prep → `interview-1-question-designer`
- The actual application portal — the founder submits at techstars.com/apply themselves

## Step 1 — Detect the mode

Figure out which mode the founder needs from how they show up. Don't ask if it's obvious.

- **Critique mode** — they paste draft answers, share a doc, or say "review/fix/tighten my answers." → Go to Step 3.
- **Coach mode** — they're starting from little or nothing ("help me apply," "where do I start," "I don't know how to answer the team question"). → Go to Step 2.
- **Mixed** — they have a few answers but not all. Critique what exists, coach the gaps.

If you genuinely can't tell, ask one short question: "Do you have draft answers for me to sharpen, or are we starting from scratch?"

## How every answer should be written (the "Application" style preset)

Apply this to every answer you draft or rewrite, in both modes. The boxes are tiny (280–500 chars; see `references/questions.md`), so the style is **dense and factual, not eloquent.** On an 8-axis scale (1–5):

`Diction 5 | Syntax 1 | Transitions 1 | Narrativity 1 | Aphorisms 2 | Figuration 1 | Intimacy 3 | Abstraction 2`

In plain terms:
- **Plain, spoken words; verbs over abstract nouns.** Cut anything ending in -tion/-ment/-ity you can replace with a verb ("orchestration" → "we run").
- **Short sentences, one idea each.** Fragments are fine. Every word costs characters.
- **No transition/filler words** ("however," "in addition," "moreover," "furthermore"). Let facts sit next to each other.
- **No story, no metaphor, no quotable maxims.** A reviewer wants facts, not a TED talk.
- **Concrete and named:** real numbers, customers, dates, percentages. Specifics are the whole game.
- **"We" is fine** (it's a company answer); don't hedge with "we believe" / "we think."

**Banned (they bloat answers and read as AI/marketing):** leverage (verb), robust, holistic, seamless, transformative, synergy, ecosystem (as metaphor), game-changer, cutting-edge, revolutionary, world-class, best-in-class, "powered by AI" as a selling point, "It's not X, it's Y," and em dashes as a rhythm device.

**Always write to the character limit.** After drafting, check the count against the cap in `references/questions.md`. If it's over, cut filler first, then the least-important fact — never shrink the key number or proof.

## Step 2 — Coach mode (build answers from scratch)

Work **one question at a time, in the order listed in `references/questions.md`.** Do not dump all 11 questions at once — it overwhelms founders and produces shallow answers.

For each question:
1. Read that question's entry in `references/questions.md`.
2. Ask the founder for the raw inputs that question needs (in plain language — don't quiz them on the framework). Ask for specifics: numbers, names, real customer quotes, what actually happened.
3. If their input is vague, push once: "Can you put a number on that?" / "Who specifically?" / "What happened, exactly?"
4. Draft the answer for them, meeting the quality bar for that question, in the Application style above and **within that question's character limit.**
5. Show it, get a reaction, refine, then move to the next question.

Keep momentum. A founder should feel like they're making progress, not filling out a form. One question per turn is the ceiling unless they want to move faster.

When all answers exist, go to Step 4.

## Step 3 — Critique mode (sharpen an existing draft)

For each answer the founder provides:
1. Read that question's entry in `references/questions.md`.
2. Diagnose against the quality bar: Is it specific or generic? Does it show evidence or just assert? Does it actually answer the question asked (e.g., the money question has two parts — how *and* how much)? **Is it within the character limit?** (Over-limit answers can't be submitted — flag and trim.)
3. Name the single biggest weakness plainly. Be direct; founders are wasting a real shot if you're soft.
4. Rewrite the answer stronger, using their actual facts. If a fact is missing, ask for it rather than inventing it — **never fabricate traction, numbers, or customer names.**
5. Flag any question they haven't answered at all.

Then go to Step 4.

## Step 4 — Produce the finished document

The deliverable is a document the founder can submit. Build it once the answers are in good shape (offer it earlier if they ask).

1. Read `/mnt/skills/public/docx/SKILL.md` and follow it to generate a clean `.docx`.
2. Structure: a short header (company name, date), then each of the 11 questions as a heading with the finished answer beneath it. Mirror the order and wording of the questions in `references/questions.md`. **Show a character count next to each answer (e.g. "382 / 400")** so the founder can confirm each fits before pasting into the form. Remember revenue and funding are structured fields, not prose (see `references/questions.md`).
3. Save to `/mnt/user-data/outputs/` and present it with `present_files`.
4. **Offer the Google Doc option:** if the founder wants it as a Google Doc instead of (or in addition to) Word, use the connected Google Drive tools to create it — upload the text with a `text/plain` content type so Drive converts it to a native Google Doc. Mention the doc will live in their Drive.

Remind the founder of Andres's advice from the guide: share the doc with co-founders, mentors, and advisors for review before submitting, and apply at techstars.com/apply.

## Holding the quality bar

These are the recurring standards behind the per-question rubric. Apply them everywhere:

- **Problem ≠ solution.** State the pain, quantified, without smuggling the product in.
- **Product: what it does and *how*, not what it is.** Cut "innovative / disruptive / AI-powered platform."
- **Team: an unfair advantage with proof.** Lived experience and specific track record beat "100 years combined experience."
- **Traction: progress over time, not a single absolute number.** Show the trend.
- **Money has two parts:** how you make it *and* how big it could get — via a **bottom-up** TAM (count real buyers × realistic annual price per buyer), never a top-down "1% of a huge market." This is the question founders fail most often; when you reach it, read `references/bottom-up-tam.md` and offer to research the buyer count and price via web search.
- **ICP: a specific persona** who has the problem, knows it, has quantified it, and will act on it.
- **Competitors: direct, indirect, and potential** — big companies *and* startups. Claiming "no competitors" is a red flag.
- **Advantage: 10x, not 10%** — and honest. Most early software startups have no durable moat yet; that's normal. Name the *one* defensibility being built first (usually workflow embedding / switching costs or distribution) and the path to deeper moats. Kill the three false moats — "proprietary data," "AI," "first-mover." When you reach this question, read `references/moats.md` and offer to research the customer's workflow chokepoints.
- **Why now: a real external shift** — a new technology, law, or market change that makes this possible or urgent now.
- **Customer acquisition: a scrappy, hard-to-replicate channel,** and a concrete path to the first 1,000 users or $2.5M.
- **Milestones: the next real proof points,** not vanity goals.
