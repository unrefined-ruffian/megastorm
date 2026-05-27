---
name: megastorm
description: Use when brainstorming a problem that would benefit from multiple analytical lenses simultaneously. Triggers on "/megastorm", "megastorm this", "run megastorm", or when the user wants structured multi-perspective ideation on a design, strategy, product, or positioning challenge.
---

# Megastorm

Multi-framework brainstorming via parallel agents. Each framework lens gets isolated context — no cross-contamination. A synthesis agent converges the outputs into ranked insights.

## Architecture

```
Phase 1: Context Agent (sequential, interactive)
  → Read project context + user request
  → Assess completeness → ask targeted questions if needed
  → Confirm problem brief with user before proceeding

Phase 2: Router (sequential, interactive)
  → Read confirmed brief → evaluate available frameworks
  → Suggest 3-5 with one-liner rationale specific to THIS problem
  → Warn if user selects >5 (synthesis degrades)
  → Wait for user confirmation before spawning agents

Phase 3: Framework Agents (parallel)
  → One isolated agent per selected framework
  → Each receives: problem brief + framework file contents
  → Each returns structured output

Phase 4: Synthesis Agent (sequential)
  → Read all framework outputs
  → Find convergence + surface outliers
  → Present ranked results with recommended next move
```

---

## Phase 1: Context Agent

Read whatever is available: CLAUDE.md, project files, user request. Then assess completeness.

**If brief is complete** (goal + audience + constraints + what's been tried are all clear):
→ Write the problem brief, confirm with user, proceed to Phase 2

**If partially complete:**
→ Write what you have, ask 2-3 targeted questions only
→ Good targets: "Who's the primary audience?", "What's the binding constraint — time, money, or adoption?", "What's already been tried that didn't work?"

**If almost nothing provided:**
→ Run a mini-interview (max 5 questions)
→ Priority order: goal → audience → constraints → tried-and-failed

**Problem Brief format:**
```
**Problem:** [One precise sentence]
**Goal:** [What success looks like]
**Audience:** [Who this is for]
**Constraints:** [What limits the solution space]
**Already tried:** [What's been attempted, if known]
**Context:** [Any relevant background]
```

Always confirm the brief with the user before moving to the router.

---

## Phase 2: Router

Read the confirmed brief. Before selecting frameworks, classify the problem shape:

**Problem shape classification** — name what kind of problem this is in one sentence. Examples:
- "This is a wonder/delight design problem — optimizing for emotional experience, not efficiency."
- "This is a positioning/strategy problem — the product works, the framing doesn't."
- "This is a root cause problem — something's broken and we don't know why."
- "This is a new market problem — we're looking for a wedge into unfamiliar territory."

State the classification explicitly. It makes framework selection legible and challengeable by the user.

Then, for each framework in the `frameworks/` directory adjacent to this SKILL.md, ask: "Does this lens reveal something useful about THIS type of problem?"

**Available frameworks:**
- `inversion.md` — Make it terrible first, then flip
- `six-hats.md` — Six cognitive modes (De Bono)
- `five-whys.md` — Drill to root cause
- `extreme-questions.md` — Novel solutions via constraint pushing
- `reframe.md` — Change the perspective, change the problem
- `jobs-to-be-done.md` — What job is this actually hired to do?
- `behavioral-science.md` — Rory Sutherland / Cialdini / Kahneman cognitive bias lens
- `six-behavioral-lenses.md` — Six-lens product teardown (shadow product, identity permission, scarcity, dimension shifting, rationalization, narrative finitude)
- `identity-persuasion.md` — Story-as-identity-deal: who does the user become?
- `anti-incumbent.md` — Map every attribute incumbents share, invert them all, find the breakout product in the negative space

Select 3-5 frameworks. For each, write ONE sentence explaining why it fits THIS problem specifically — not a generic framework description.

**Router output format:**
```
Here are the frameworks I'd run on this:

1. **[Framework]** — [One sentence: why this lens on THIS problem]
2. **[Framework]** — [One sentence: why this lens on THIS problem]
3. **[Framework]** — [One sentence: why this lens on THIS problem]

Want to add, remove, or swap any? (Going above 5 will dilute the synthesis — I'd hold firm on that ceiling.)
```

Wait for user confirmation before spawning Phase 3 agents.

---

## Phase 3: Framework Agents

Spawn one Agent per confirmed framework. Each agent is fully isolated — it does NOT see other agents' outputs.

Each agent receives:
1. The confirmed problem brief (paste it in full)
2. The contents of its framework file (read before starting)
3. This instruction:

> "Apply [framework name] to this problem brief. Be specific and provocative — generic insights are worthless here. Your output should contain ideas that could not have come from surface-level thinking."

**Required output format per agent:**
```markdown
## [Framework Name] Output

**Reframe:** [How this lens sees the problem differently than stated]

**Ideas:**
- [Specific, actionable idea with brief reasoning]
- [Specific, actionable idea with brief reasoning]
- [Specific, actionable idea with brief reasoning]

**Wild card:** [The most provocative or unexpected output from this lens — the idea that makes you slightly uncomfortable]
```



Run all framework agents in parallel for speed.

---

## Phase 4: Synthesis Agent

Read ALL framework outputs. Your job is convergence and curation — not summary.

**Step 1 — Find convergence:**
What ideas appeared (in different forms) across multiple frameworks? Multiple lenses pointing the same direction is a signal. Name which frameworks agreed.

**Step 2 — Find tension:**
Where did frameworks disagree or pull in opposite directions? Tension between lenses is as valuable as convergence — it reveals genuine trade-offs the user needs to decide, not just options to pick between. Name the specific disagreement and what each side reveals. If no meaningful tension exists, say so briefly and move on — don't manufacture conflict.

**Step 3 — Surface outliers:**
What high-value ideas came from only ONE framework? Don't bury these — single-lens insights can be the most novel.

**Step 4 — Rank:**
Order by: novelty × feasibility × alignment with stated goal

### Synthesis Output: Two-Tier Structure

The synthesis has two tiers: a TLDR that hits like a hammer, and a Deep Dive with the full reasoning. The TLDR is NOT a compressed summary — it's the actual insights written with full force, just without the analysis scaffolding. Every punch lands in the TLDR. The Deep Dive is where the reasoning chains, evidence, and nuance live.

**The rule: if the TLDR doesn't make the user react, the synthesis failed.** Compression that kills the juice is worse than length.

```markdown
## Megastorm Results: [Problem title]

## TLDR

### Where the frameworks converged
[Each convergence gets its own **bold claim as header** + 2-3 sentences of insight written with force. The claim should land on its own. The sentences explain WHY this matters for THIS problem. Don't water it down.]

### Where the frameworks disagreed
[Same format — bold claim + brief tension. If no meaningful disagreement, omit this section entirely rather than writing "no tensions found."]

### High-value single-lens insights
[Compressed — one line per insight. Framework name + the idea. These are teasers that earn their detail in the Deep Dive.]

### The wild card
[The most provocative idea from the whole session — written with full dramatic force. This is the one that makes someone stop scrolling. Give it room to breathe.]

### Tiny Experiment
[One specific, low-cost action that tests the biggest insight before building anything. Include:
1. What to do (concrete steps)
2. Rationale — why THIS test validates THIS insight]

## Deep Dive

### [Convergence point 1 — expanded]
[Full reasoning chain: which frameworks agreed, how they arrived at the same conclusion from different angles, what the implications are for design/strategy decisions]

### [Convergence point 2 — expanded]
[Same depth]

### [Tensions — expanded]
[The full trade-off analysis if tensions exist]

### [Single-lens insights — expanded]
[The full reasoning behind each outlier idea — why it deserves attention despite only one framework surfacing it]
```

---

## Framework Library

Frameworks live in the `frameworks/` directory adjacent to this SKILL.md. Each file is a standalone lens definition.

**To add a new framework:** Create a new `.md` file in `frameworks/` following the pattern:
- Name + what this lens does (one sentence)
- The key question(s) it asks
- How to run it (3-5 steps)
- The agent prompt
- What good output looks like

The router will automatically consider any file in the directory.

---

## Common Mistakes

| Mistake | Fix |
|---|---|
| Skipping Phase 1 confirmation | Brief must be confirmed before framework selection |
| Running >5 frameworks | Synthesis becomes noise above 5; warn and hold firm |
| Framework agents seeing each other's outputs | They must be isolated — parallel, not sequential |
| Router using generic framework descriptions | Every rationale must be specific to THIS problem |
| Synthesis agent summarizing instead of converging | Find what multiple lenses agreed on, not what each said |
