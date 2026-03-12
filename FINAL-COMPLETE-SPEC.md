# Claude Code ABQ — March 2026 Meetup: COMPLETE PRESENTATION SPEC

## Project Overview

Build a GitHub-ready repo containing a reveal.js slide presentation and supporting materials for the March 2026 Claude Code ABQ meetup.

**Repo:** https://github.com/MartyBonacci/claude-abq-3-12-26
**Website:** https://claudeabq.dev
**Event:** https://luma.com/eal0lrdd
**Date:** Thursday, March 12, 2026, 6:00–8:00 PM MST
**Location:** Deep Dive Coding Classrooms, CNM STEMulus Center, Downtown Albuquerque
**Presenter:** Marty Bonacci — Organizer, Claude Code ABQ; Lead Instructor, Deep Dive Coding
**Talk Title:** "The Most Valuable Developer on Your Team — Building AI Workflows That Scale"

---

## Repo Structure

```
claude-abq-3-12-26/
├── README.md
├── index.html                         # Reveal.js presentation (main file)
├── images/                            # All presentation images (flat directory)
│   ├── 2-boards-nailed-together-with-3-nails-flush.png
│   ├── 2-boards-partly-nailed-together-with-three-nails-partway-in.png
│   ├── did-they-try-to-nail-them-in-with-an-axe-or-the-claw-end-of-the-hammer.png
│   ├── how-did-they-get-the-nails-to-twist-up-like-this.png
│   ├── LOL-what-happened-here.png
│   ├── nailed-into-the-stacked-wood-with-nails-sideways.png
│   ├── nailed-into-wood-sideways-but-the-wood-is-butted-end-to-end.png
│   ├── nailed-to-table.png
│   ├── nails-bent-dents-in-the-wood.png
│   ├── not-sure-if-this-is-one-or-two-twisted-nails-may-be-pounded-in-with-random-pointy-object.png
│   ├── one-nail-pressed-in-by-hand.png
│   ├── one-zig-zag-nail-may-be-pounded-in-with-random-object.png
│   ├── pressed-in-by-hand.png
│   ├── pressed-in-by-hand-2.png
│   ├── these-boards-are-tipped-on-edge.png
│   ├── this-joint-looks-beatiful-even-though-there-are-no-nails.png
│   ├── too-much-force-broken-board.png
│   ├── two-pieces-of-wood-sandwhiching-a-nail.png
│   ├── what-the-is-going-on-here-nails-in-every-direction-and-smashed-wood.png
│   ├── wood-joints-with-pile-of-manuals.png
│   ├── claude-ai-screenshot.png       # Placeholder — Marty will provide
│   └── claude-code-screenshot.png     # Placeholder — Marty will provide
├── references/                        # Supporting materials
│   ├── extensibility-stack.md
│   ├── example-claude-md.md
│   ├── getting-started.md
│   └── resources.md
└── SPEC.md                            # This file
```

---

## Design System

### Colors
- **Primary background:** Dark navy `#1a1a2e` or near-black `#0f0f1a`
- **Prompt card background:** Slightly lighter `#16213e` with subtle border
- **Text:** White `#ffffff` for headings, light gray `#c0c0c0` for body
- **Accent/highlight:** Teal `#028090` for new prompt lines, links
- **Warm accent:** Coral `#F96167` for emphasis moments
- **Code/mono text:** `#e0e0e0` on dark background

### Typography
- **Headings:** Monospace (Consolas, 'Courier New', monospace) — reinforces terminal/code identity
- **Body text:** Clean sans-serif (system-ui, -apple-system, sans-serif)
- **Code blocks / prompt cards:** Monospace, slightly smaller

### Slide Types
1. **Title slides** — Big text centered on dark background
2. **Prompt slides** — Setup line (small, gray) + card text (monospace, in a subtle card/box)
3. **Image slides** — Full-bleed image, edge to edge, no text (or minimal overlay)
4. **Text slides** — Centered text on dark background, minimal words
5. **Table slides** — Clean table with dark background
6. **Comparison slides** — Two-column layout

### General Rules
- Minimal text on every slide — speaker notes carry the detail
- No bullet point lists — use short lines, whitespace, and typography hierarchy
- Full-bleed images wherever possible
- Dark backgrounds throughout for consistency and projector readability

---

## COMPLETE SLIDE-BY-SLIDE SPEC

Total slides: ~54 (including 32 boards sequence slides)

---

### Slide 1: TITLE

**Type:** Title slide

**Content:**
- **Claude Code ABQ** (large, top — monospace)
- **"The Most Valuable Developer on Your Team"** (subtitle)
- **claudeabq.dev**
- **QR code** → https://luma.com/eal0lrdd (generate programmatically)

**Design:** Dark background. Clean. Terminal aesthetic. QR code in bottom corner.

**Speaker notes:** None needed — just let people settle in and scan the QR.

---

### Slide 2: WHY WE'RE HERE

**Type:** Text slide

**Content:**
> **We share what actually works.**
>
> Honest about what's working and what isn't — no hype, no marketing
>
> We focus on Claude Code because it's the best tool right now. Bring us something better and we'll try it.
>
> Developers, non-developers, all levels — if you're curious, you belong here

**Speaker notes:**
"This isn't a fan club. We're not here to sell you on Claude Code. We're here because right now, today, it's the most effective AI coding tool we've found. If someone walks in next month and shows us something that blows it away, we'll be the first ones trying it. Whether you write code for a living or you've never opened a terminal, there's a seat for you."

---

### Slide 3: CALL FOR PRESENTERS

**Type:** Text slide

**Content:**
> **Show us something we can use.**
>
> About 30 minutes
>
> We want workflows, tools, and techniques that developers can implement NOW
>
> You don't need to be an expert — share what's working for you
>
> Talk to Marty

**Speaker notes:**
"We're looking for presenters. Show us a workflow, a tool, a technique that the people in this room can go home and implement. That's what makes this community valuable."

---

### Slide 4: AUDIENCE CHECK

**Type:** Text slide (interactive)

**Content:**
> **Quick show of hands...**
>
> Who writes code professionally?
>
> Who has used any AI coding tool?
>
> Who has used Claude Code specifically?
>
> Who has NEVER written code?

**Design:** Each question could appear as a fragment/reveal if reveal.js supports it. Or just list all four.

**Speaker notes:**
"Quick show of hands so I know who I'm talking to tonight." (Go through each, read the room, acknowledge all groups.) "This talk is for ALL of you — the concepts apply whether you code or not."

---

### Slide 5a: CLAUDE.AI vs CLAUDE CODE — VISUAL

**Type:** Comparison slide (side by side)

**Content:**
- **Left side:** Screenshot of Claude.ai chat interface
- **Right side:** Screenshot of Claude Code terminal session
- Labels: "Claude.ai" and "Claude Code" above each

**Design:** Split screen, dark background, images centered in each half.

**Image files:** `images/claude-ai-screenshot.png` and `images/claude-code-screenshot.png`
*Note: Marty will provide these screenshots — they don't exist yet. Use placeholder boxes at build time.*

**Speaker notes:**
"Two ways to use the same AI. On the left, Claude.ai — a chat in your browser. On the right, Claude Code — running in your terminal, inside your project."

---

### Slide 5b: CLAUDE.AI vs CLAUDE CODE — TABLE

**Type:** Table slide

**Content:**

| | **Claude.ai** | **Claude Code** |
|---|---|---|
| **Where** | Browser / mobile app | Your terminal |
| **What it does** | Answers, writes, analyzes | Reads your code, runs commands, edits files |
| **Context** | Only what you paste in | All the files in your project + understanding of your environment and OS |
| **Agency** | You copy-paste the output | It makes the changes directly |
| **Analogy** | Texting a smart friend | A developer sitting at your machine |

**Design:** Clean table on dark background. Two columns clearly differentiated. Maybe Claude.ai column slightly dimmer, Claude Code column slightly brighter/accented to emphasize the focus of this community.

**Speaker notes:**
"The key difference is that third row — context. Claude.ai only knows what you paste in. Claude Code can see all the files in your project, understands your environment, your OS. That context is everything."

---

### Slide 6: WHAT ANTHROPIC RELEASED

**Type:** Text slide (rapid fire list)

**Content:**
> **Since Our Last Meetup (Feb 12)**
>
> **Sonnet 4.6** — upgraded coding, agents, 1M context window
>
> **Claude Code Review** — parallel AI agents reviewing every PR
>
> **Ultrathink is back** — sets effort to high for one turn
>
> **Auto memory** — per-project, across sessions
>
> **Skills 2.0** — unified commands & skills, bundled `/simplify` `/batch` `/loop`
>
> **Effort levels** — simplified to low/medium/high
>
> **`/btw`** — ask side questions without interrupting work

**Design:** Each item on its own line. Bold the product name, normal weight for description. Compact but readable. This slide should feel like a rapid-fire news ticker.

**Speaker notes:**
Rapid fire through each item, ~15-20 seconds per item. Highlight the ones most relevant to the audience. "/btw literally dropped yesterday — you can ask Claude a question WHILE it's working without interrupting it or polluting your conversation history."

---

### Slide 7: LAST MONTH

**Type:** Text slide (minimal)

**Content:**
> **tweeter.dev**
>
> *Live-built from scratch. February 12, 2026.*
>
> github.com/MartyBonacci/tweeter-abq-2

**Design:** Could include a screenshot of the finished tweeter app if available. Otherwise just the text, large and centered.

**Speaker notes:**
"Last month, right here in this room, we built a Twitter clone from scratch using Claude Code. Single prompt to start, SpecSwarm to generate the specs and tasks, React Router v7, and we deployed it live during the demo. Source code is on GitHub. For many of you watching that... it felt like watching black magic."

---

### Slide 8: BLACK MAGIC BRIDGE

**Type:** Text slide

**Content:**
> **"This feels like black magic..."**
>
> *...but then you try it and it doesn't work the same way.*
>
> **Let me show you why.**

**Design:** Three lines, stacked. First line large. Second line italic, dimmer. Third line bold, accent color. Could use fragment reveals — show first two lines, pause, then reveal "Let me show you why."

**Speaker notes:**
"When you watch someone use Claude Code effectively, it looks effortless. The AI just seems to know what to do. It generates features, fixes bugs, handles deployment. The natural reaction is 'I want to do that too.' But then you try it... and it doesn't work the same way. Let me show you why."

---

## THE BOARDS SEQUENCE (Slides B-0 through B-31)

### How This Works

Every "beat" is TWO slides:
1. **PROMPT slide** — dark background, setup line + instruction card text
2. **IMAGE slide** — full-screen image, no text

The audience reads the prompt, anticipates what could go wrong, then the image reveals the result. Setup → punchline. NEVER put both prompt and image on the same slide.

### Prompt Slide Design
- Dark background
- Setup line at top: small, gray, italic (e.g., *"New person walks in. I update the card:"*)
- Card text: monospace font, centered, inside a subtle lighter-background card/box
- Previously seen lines in white/light text
- NEW lines highlighted in accent color (teal `#028090`) so the audience sees what changed
- Card text should look like an instruction card — maybe a subtle border or slight background difference

### Image Slide Design
- Full-bleed image, edge to edge
- No text overlay
- Dark background behind image if image doesn't fill completely

### Callback Slides (B-19, B-21, B-23)
- The prompt on all three MUST be visually identical — same card, same text, same layout
- This repetition makes the audience laugh before the image even appears

---

### Slide B-0: THE SETUP

**Type:** Text slide

**Content:**
> Imagine you run a workshop.
>
> Every time you need boards nailed together,
> a brand new person walks in.
>
> They have NO memory of anyone who came before them.
>
> You hand them a card with your instructions.
> They go in the back room.
> You never see what happens in there.
>
> They come back with... a result.

**Speaker notes:**
"Here's how this works. Every time I need boards nailed together, a brand new person walks in. They've never met anyone before them. I hand them a card. They go in the back room. I never see what happens. They come back with a result. Let me show you how this goes."

---

### PHASE 1: What Tool? (B-1 through B-8)

---

### Slide B-1: PROMPT

**Setup line:** *"First person walks in. I hand them this card:"*

**Card text:**
```
Nail these two boards together.
```

---

### Slide B-2: IMAGE

**Image:** `images/two-pieces-of-wood-sandwhiching-a-nail.png`

**Speaker notes:**
"A nail. Between two boards. Together. Instructions followed PERFECTLY. This is what happens when you open a fresh Claude conversation and type 'build me a website.'"

---

### Slide B-3: PROMPT

**Setup line:** *"New person walks in. I update the card:"*

**Card text:**
```
Nail these two boards together.
The nail needs to be nailed into the wood.        ← NEW (highlight)
```

---

### Slide B-4: IMAGE

**Image:** `images/one-nail-pressed-in-by-hand.png`

**Speaker notes:**
"A single nail, barely in the wood, would fall over if you breathed on it. They just pushed it in with their hand. We never said to use a tool. Same prompt with one new line, different person, completely different kind of wrong."

---

### Slide B-5: PROMPT

**Setup line:** *"New person. I add another line:"*

**Card text:**
```
Nail these two boards together.
The nail needs to be nailed into the wood.
Pound the nail in.                                ← NEW (highlight)
```

---

### Slide B-6: IMAGE

**Image:** `images/one-zig-zag-nail-may-be-pounded-in-with-random-object.png`

**Speaker notes:**
"They pounded! With SOMETHING. Look at those gouge marks — that's not a hammer. That might be a wrench. A rock. A coffee mug. We said 'pound' but never said WHAT to pound with. We keep assuming they know things they don't know. Just like with AI."

---

### Slide B-7: PROMPT

**Setup line:** *"New person. I finally add what should have been obvious:"*

**Card text:**
```
Nail these two boards together.
The nail needs to be nailed into the wood.
Pound the nail in.
Use a hammer.                                     ← NEW (highlight)
```

---

### Slide B-8: IMAGE

**Image:** `images/not-sure-if-this-is-one-or-two-twisted-nails-may-be-pounded-in-with-random-pointy-object.png`

**Speaker notes:**
"Is that one nail? Two? How do you get metal to DO that? They have a hammer now but they clearly have no idea how to use it. This is the Claude response where you stare at the output and think 'what reasoning process leads HERE?'"

---

### PHASE 2: Two Boards, New Problems (B-9 through B-14)

---

### Slide B-9: PROMPT

**Setup line:** *"New person. I add more detail:"*

**Card text:**
```
Nail these two boards together.
The nail needs to be nailed into the wood.
Pound the nail in. Use a hammer.
Pound them in straight.                           ← NEW (highlight)
```

---

### Slide B-10: IMAGE

**Image:** `images/nailed-into-wood-sideways-but-the-wood-is-butted-end-to-end.png`

**Speaker notes:**
"'Pound them in straight.' And they ARE straight. Perfectly straight. Horizontally. Through the seam of two boards butted end-to-end. We said straight. We didn't say which direction."

---

### Slide B-11: PROMPT

**Setup line:** *"New person. I emphasize TOGETHER:"*

**Card text:**
```
Nail these two boards together.
The nail needs to be nailed into the wood.
Pound the nail in. Use a hammer.
Pound them in straight.
Nail the two boards together.                     ← NEW (highlight)
```

---

### Slide B-12: IMAGE

**Image:** `images/nailed-into-the-stacked-wood-with-nails-sideways.png`

**Speaker notes:**
"The boards are stacked now! They're actually TOGETHER! But the nails are STILL sideways. We keep solving one problem and revealing the next. Six lines of instructions. Still wrong."

---

### Slide B-13: PROMPT

**Setup line:** *"New person. I spell out the direction:"*

**Card text:**
```
Nail these two boards together.
The nail needs to be nailed into the wood.
Pound the nail in. Use a hammer.
Nail the two boards together.
Pound the nails straight down, through both boards. ← NEW (highlight)
```

---

### Slide B-14: IMAGE

**Image:** `images/nailed-to-table.png`

**Speaker notes:**
"'Straight DOWN. Through BOTH boards.' And they went straight down. Through both boards. And through the workbench. And out the bottom of the table. We never said to STOP. But hey — the boards are actually CONNECTED. Seven attempts and we have two boards nailed together. They're also nailed to furniture, but still. Progress."

---

### PHASE 3: Getting Better (B-15 through B-18)

---

### Slide B-15: PROMPT

**Setup line:** *"New person. I write a REAL paragraph this time:"*

**Card text (font getting smaller — it's a real paragraph now):**
```
Take two 2x4 boards. Overlap them by 6 inches with
edges flush. Using a 16oz claw hammer and 10d common
nails, drive 3 nails evenly spaced through the
overlap area. Drive them from the top, perpendicular
to the surface. Don't nail into the workbench. Don't
bend the nails. Don't dent the wood.
```

*Note: No lines highlighted — this is a fresh start, all new text.*

---

### Slide B-16: IMAGE

**Image:** `images/2-boards-partly-nailed-together-with-three-nails-partway-in.png`

**Speaker notes:**
"NOW we're getting somewhere! Nails are straight. Wood is lined up. Nails are actually connecting the boards. Mostly. One nail only goes through the top board. They're not driven flush. But this is a B-minus. This is RECOGNIZABLE as the right thing. Look at the prompt though. Full paragraph. And this is for ONE joint."

---

### Slide B-17: PROMPT

**Setup line:** *"New person. I write an entire MANUAL:"*

**Card text (WALL of text — small font, let the audience groan):**
```
PROJECT CONTEXT: We are building a load-bearing
deck frame. All joints must meet IRC code R507.

MATERIALS: Two #2 grade Southern Yellow Pine 2x4
boards, 8 feet long. 10d hot-dipped galvanized
common nails. 16oz claw hammer.

TASK: Create a lap joint. Overlap boards by 6"
with edges flush. Drive 3 nails in a triangular
pattern. All nails perpendicular. Drive until
flush — do not countersink.

TECHNIQUE: Hold nail near the point, tap 2-3
times to set, remove fingers, drive with full
swings. Keep wrist straight. Strike dead center.

QUALITY: Edges flush within 1/16". No gaps. No
protruding heads. No hammer marks. No bent nails.

SAFETY: Wear glasses. Clamp boards first. Keep
fingers 2" from strike zone.
```

---

### Slide B-18: IMAGE

**Image:** `images/2-boards-nailed-together-with-3-nails-flush.png`

**Speaker notes:**
"A full PAGE of instructions. Project context. Materials. Technique. Quality standards. Safety. And it WORKS. Three nails, flush, clean, beautiful. But do you want to hand someone THIS CARD every single time you need ONE nail driven?"

---

### PHASE 4: The Hammer Callback (B-19 through B-24)

*The emotional climax. We write a new detailed prompt focused on quality/alignment but FORGET to mention the hammer. Then try the same prompt THREE TIMES.*

---

### Slide B-19: PROMPT

**Setup line:** *"New job. I write a fresh card focused on quality and alignment:"*

**Card text:**
```
Take two 2x4 boards. Overlap by 6 inches, edges
perfectly aligned and flush. Drive 3 nails in a
triangular pattern through the overlap area. All
nails perpendicular to the surface. Nail heads
flush with wood. No gaps between boards. No marks
on the wood surface. Clamp boards before nailing.
Pre-drill if necessary.
```

*CRITICAL: This prompt deliberately does NOT mention a hammer. Do NOT add one.*

---

### Slide B-20: IMAGE

**Image:** `images/did-they-try-to-nail-them-in-with-an-axe-or-the-claw-end-of-the-hammer.png`

**Speaker notes:**
"WHAT!? We had it! We just had a PERFECT result! What HAPPENED? This is a GOOD prompt! Overlap, alignment, nail pattern, flush heads, clamping, pre-drilling... what went wrong?" (Don't answer yet. Move to next slide.)

---

### Slide B-21: PROMPT

**Setup line:** *"Must be a fluke. New person, same card:"*

**Card text (IDENTICAL to B-19):**
```
Take two 2x4 boards. Overlap by 6 inches, edges
perfectly aligned and flush. Drive 3 nails in a
triangular pattern through the overlap area. All
nails perpendicular to the surface. Nail heads
flush with wood. No gaps between boards. No marks
on the wood surface. Clamp boards before nailing.
Pre-drill if necessary.
```

---

### Slide B-22: IMAGE

**Image:** `images/how-did-they-get-the-nails-to-twist-up-like-this.png`

**Speaker notes:**
"Different person, same prompt, different disaster. Same underlying problem." (Still don't reveal. Build tension.)

---

### Slide B-23: PROMPT

**Setup line:** *"ONE more time. Same card:"*

**Card text (IDENTICAL again):**
```
Take two 2x4 boards. Overlap by 6 inches, edges
perfectly aligned and flush. Drive 3 nails in a
triangular pattern through the overlap area. All
nails perpendicular to the surface. Nail heads
flush with wood. No gaps between boards. No marks
on the wood surface. Clamp boards before nailing.
Pre-drill if necessary.
```

---

### Slide B-24: IMAGE

**Image:** `images/what-the-is-going-on-here-nails-in-every-direction-and-smashed-wood.png`

**Speaker notes:**
(Stare at image. Stare at prompt. Back at image.)
"Wait. Overlap... alignment... nail pattern... perpendicular... flush heads... clamping... pre-drilling... Where's the hammer? There's no hammer in this prompt. We got so focused on the NEW requirements that we forgot to mention THE HAMMER. Three people in a row walked in with a detailed, professional-looking card... and no idea what tool to use. THIS is what happens when you start a new Claude conversation and your 'improved' prompt is missing the one line that was making everything work."

---

### PHASE 5: The Scaling Problem (B-25 through B-26)

---

### Slide B-25: THE BINDER

**Type:** Image slide with brief text overlay

**Image:** `images/wood-joints-with-pile-of-manuals.png`

**Text overlay:** *"The prompt needs EVERYTHING. For every joint type."*

**Speaker notes:**
"The prompt needs the hammer. The technique. The nail spec. The safety rules. For EVERY type of joint. That's how you end up with THIS. The copy-paste-prompt-engineering lifestyle. Forty-seven Google Docs. And if you accidentally delete one line? The hammer disappears."

---

### Slide B-26: THE TEAM PROBLEM

**Type:** Text slide

**Content:**
> You have 5 new hires starting Monday.
> Each one needs to nail boards.
> None of them have met each other.
> None of them have met YOU.
>
> Do you photocopy the binder?
> And hope nobody loses the page about the hammer?

**Speaker notes:**
"Five new hires. Five fresh AI conversations. Nobody has any context. Every single one will nail-sandwich or pretzel-twist unless you hand them the ENTIRE binder. And pray nobody loses the page about the hammer."

---

### PHASE 6: The Solution (B-27 through B-31)

---

### Slide B-27: PROMPT — THE EMPLOYEE MANUAL

**Setup line:** *"Or... what if there was an employee manual?"*

**Card text:**
```
CLAUDE.md:
  "You are a finish carpenter specializing in
   residential decks. You follow IRC code R507.
   You use 10d galvanized nails and a 16oz claw
   hammer. You pre-drill when necessary. You
   always clamp before nailing."

Card: "Nail these boards together with a lap joint."
```

*Design note: Show the CLAUDE.md section in a different style/color than the card section to distinguish permanent context from the one-line prompt.*

---

### Slide B-28: IMAGE — SAME PERFECT RESULT

**Image:** `images/2-boards-nailed-together-with-3-nails-flush.png` *(reuse from B-18)*

**Speaker notes:**
"SAME RESULT. Same perfect joint. Same three nails. But the card is ONE LINE. 'Nail these boards together with a lap joint.' What changed? They read the employee manual FIRST. The CLAUDE.md. Now they KNOW they're a finish carpenter. They KNOW the code. And the hammer will NEVER go missing again — it's in the manual, not on individual cards."

---

### Slide B-29: PROMPT — THE TRAINING PROGRAM

**Setup line:** *"Or... what if there was a training program?"*

**Card text (BIG font, centered):**
```
/nail-boards lap-joint
```

---

### Slide B-30: IMAGE — TRANSCENDENCE

**Image:** `images/this-joint-looks-beatiful-even-though-there-are-no-nails.png`

**Speaker notes:**
(Long pause.) "/nail-boards. One command. And look what came back. They didn't just nail the boards. They understood the project deeply enough to realize a precision wood joint is STRONGER and more beautiful than nails. They went BEYOND instructions because they understood the WHY. That's what happens with deep enough context. AI doesn't just follow instructions — it makes BETTER decisions than you would have specified. All that knowledge? Inside the skill. Runs every time. Runs for everyone. Five new hires? /nail-boards. Building code changes? Update the skill ONCE. The hammer will NEVER go missing."

---

### Slide B-31: THE PUNCHLINE

**Type:** Text slide (use fragments/staged reveal if possible)

**Content — reveal in stages:**

Line 1:
> "The most valuable developer on your team isn't the best coder."

Line 2 (after beat):
> "It's the one who builds the systems that turn EVERY developer into the best coder."

Line 3 (after another beat):
```
CLAUDE.md   →  The employee manual
Skills      →  The training program
Hooks       →  The safety rules that ALWAYS apply
Commands    →  The shortcuts everyone can use
Agents      →  The specialists you delegate to
```

**Speaker notes:**
"THIS is the talk. The magic last month? Not magic. Months of CLAUDE.md files, skills, specs, hooks — so when I type one command, Claude has ALL the context. And I can SHARE them. Anyone who installs SpecSwarm gets everything I've learned. That's not prompt engineering. That's AI workflow architecture."

---

### META MOMENT (optional — Marty uses at his discretion)

Can be inserted verbally at any point, works best after B-24:

"By the way — these images? I tried to get AI to generate them last night. I told it 'no hammer in the scene.' Hammer in EVERY image. I told it to show nails in the finals. No nails. I was LIVING this talk while MAKING this talk."

---

## POST-BOARDS SLIDES (11-22)

---

### Slide 11: THE REAL SKILL

**Type:** Text slide

**Content:**
> **The real skill isn't prompting. It's building training materials.**

**Speaker notes:**
"Everything you just saw in the boards sequence — that's what AI-assisted development actually is. Not writing better prompts. Building the training materials that make every prompt work. CLAUDE.md, skills, hooks, agents — those are your tools."

---

### Slide 12: SPECSWARM

**Type:** Text slide

**Content:**
> **SpecSwarm**
> *Spec-driven development plugin for Claude Code*
>
> Describe → Spec → Plan → Tasks → Build → Review
>
> specswarm.com | github.com/MartyBonacci/specswarm

**Speaker notes:**
"This is the real-world example. SpecSwarm packages everything I've learned about spec-driven development into a plugin anyone can install. You describe what you want, it generates a spec, breaks it into a plan, creates tasks, and Claude executes. This is what I used to build tweeter.dev last month."

---

### Slide 13: TRAIN YOUR NEW HIRE INSTANTLY

**Type:** Text slide

**Content:**
> **What if you could train your new hire instantly?**
>
> `claude plugin install specswarm`

**Speaker notes:**
"Remember the new hires? The ones who kept sandwiching nails and destroying workbenches? What if on their first day, you could give them all of your accumulated knowledge in one command? That's what this is. Months of workflow knowledge, installed in seconds. Every new hire — every new Claude session — starts fully trained."

---

### Slide 14: HOW I BUILT SPECSWARM

**Type:** Text slide

**Content:**
> CLAUDE.md → Commands → Skills → Plugin
>
> *Each layer made the next project faster.*

**Speaker notes:**
"SpecSwarm was itself built with Claude Code. Started as CLAUDE.md instructions, grew into custom commands, evolved into skills, packaged as a plugin. That progression IS the lesson. Start with a good CLAUDE.md. Notice patterns. Extract them. Share them."

---

### Slide 15: THE EXTENSIBILITY STACK

**Type:** Table slide (this is the one people photograph)

**Content:**

| Layer | What | Deterministic? |
|---|---|---|
| **CLAUDE.md** | Project memory | Always loaded |
| **Skills** | Reusable playbooks | Claude decides when |
| **Commands** | /slash triggers | User-triggered |
| **Hooks** | Shell scripts at lifecycle events | Always fires |
| **Subagents** | Isolated workers, own context | Claude delegates |
| **Plugins** | Bundled & shareable | Mixed |

> *"CLAUDE.md for memory. Skills for routines. Hooks for guarantees. Agents for delegation."*

**Speaker notes:**
"This is your reference slide. Take a photo. The key insight is that bottom line — hooks GUARANTEE execution, everything else is probabilistic. If something MUST happen every time, it's a hook, not a prompt."

---

### Slide 16: BOOTCAMP NAMING

**Type:** Text slide (interactive)

**Content:**
> **Help us name the bootcamp.**
>
> "Web Development & AI Tools"
> *or*
> "Web Development + AI Integration"
>
> *Show of hands.*

**Speaker notes:**
"We just added two weeks of AI-assisted development to our web dev bootcamp. We need a name. Show of hands — who likes 'Web Development & AI Tools'? And who likes 'Web Development + AI Integration'?"

---

### Slide 17: THE SPICY QUESTION

**Type:** Text slide (interactive)

**Content:**
> **Should we offer a Vibe Coding Bootcamp?**

**Speaker notes:**
"Now here's the thing — we're still teaching the full web dev curriculum. Our grads can code without AI. That's important. But I'm curious... who thinks we should offer a Vibe Coding Bootcamp?" (Read the room. This is market research.)

---

### Slide 18: DEEP DIVE CODING

**Type:** Text slide

**Content:**
> **Deep Dive Coding**
> *12-week full-stack web development bootcamp*
> *Now with 2 weeks of AI-assisted development*
>
> Right here at CNM STEMulus Center
> deepdivecoding.com

**Speaker notes:**
"We're integrating AI-assisted development into the bootcamp curriculum. Students learn to build WITH AI from day one. If you're interested in transitioning into tech or leveling up, talk to me after."

---

### Slide 19: CALL FOR PRESENTERS (SECOND ASK)

**Type:** Text slide

**Content:**
> **Show us something we can use.**
> *~30 minutes. Talk to Marty.*

**Speaker notes:**
"Remember from the beginning — we need presenters. Workflows, tools, techniques developers can implement now. Talk to me."

---

### Slide 20: Q&A

**Type:** Text slide

**Content:**
> **Questions?**

**Speaker notes:**
"Open floor. No question too basic — this stuff changes every week."

---

### Slide 21: MINGLE

**Type:** Text slide

**Content:**
> **Mingle. Share. Help each other.**
>
> Open your laptops. Show your neighbor what you're working on.
>
> docs.anthropic.com/en/docs/claude-code/getting-started

**Speaker notes:**
"This is the best part. Get up, move around, introduce yourself to someone you haven't met. Show each other what you're building. If you need help getting set up with Claude Code, find someone who's already using it — or find me. This is why we meet in person."

---

### Slide 22: CLOSING

**Type:** Text slide

**Content:**
> **claudeabq.dev**
>
> *(QR code → luma.com/eal0lrdd)*
>
> github.com/MartyBonacci/claude-abq-3-12-26
>
> See you next month.

**Speaker notes:**
"Register for next month. Tonight's slides, images, and reference materials are all in the GitHub repo. Thanks for being here."

---

## PACING GUIDE (2 hours total)

| Time | Slides | Content | Duration |
|------|--------|---------|----------|
| 6:00–6:10 | — | Arrival, settling in | 10 min |
| 6:10–6:20 | 1–4 | Title, purpose, presenters, audience check | 10 min |
| 6:20–6:30 | 5a–8 | Claude.ai vs Code, releases, last month, black magic | 10 min |
| 6:30–6:55 | B-0 through B-31 | **THE BOARDS SEQUENCE** | 25 min |
| 6:55–7:10 | 11–15 | Training materials, SpecSwarm, extensibility | 15 min |
| 7:10–7:20 | 16–19 | Survey questions, bootcamp, presenters | 10 min |
| 7:20–7:40 | 20 | Q&A | 20 min |
| 7:40–8:00 | 21–22 | Mingle, hands-on, closing | 20 min |

---

## SUPPORTING REFERENCE DOCS TO GENERATE

These live in the `references/` folder of the repo.

### extensibility-stack.md
Detailed breakdown: CLAUDE.md, Skills, Commands, Hooks, Subagents, Agent Teams, Plugins. Include the decision framework and examples.

### example-claude-md.md
A well-commented example CLAUDE.md that a newcomer could adapt. Sections for: project overview, tech stack, coding standards, common patterns, things to avoid.

### getting-started.md
Step-by-step for someone who has never used Claude Code: installation, first session, creating first CLAUDE.md, next steps.

### resources.md
All links:
- claudeabq.dev
- luma.com/eal0lrdd
- github.com/MartyBonacci/specswarm
- specswarm.com
- github.com/MartyBonacci/four-minds-pattern
- github.com/MartyBonacci/tweeter-abq-2
- deepdivecoding.com
- docs.anthropic.com/en/docs/claude-code
- docs.anthropic.com/en/docs/claude-code/getting-started

---

## NOTES FOR CLAUDE CODE

1. **Use reveal.js** — load from CDN. Single index.html file.
2. **Generate QR codes** programmatically (use a JS QR library or embed SVG QR codes).
3. **Dark theme throughout** — use the color palette specified above.
4. **Image slides should be full-bleed** — use `data-background-image` on the section.
5. **Prompt card styling** — create a consistent CSS class for the instruction card look: monospace font, subtle background, centered, with highlighted new lines in accent color.
6. **Fragment reveals** — use reveal.js fragments for Slide 8 ("Let me show you why"), Slide B-31 (punchline lines), and Slide 4 (audience questions) if practical.
7. **Speaker notes** — include all speaker notes in reveal.js speaker notes format so they show in presenter view.
8. **Image placeholders** — for screenshots (5a), create placeholder divs noting "screenshot needed" so Marty can drop them in.
9. **All images are in `images/`** (flat directory, no subdirectories) — reference them by their exact filenames as listed in the repo structure above.
10. **Keep it simple** — this needs to work reliably on a projector tomorrow. Don't over-engineer animations or transitions. Slide transitions should be simple fades or slides.
