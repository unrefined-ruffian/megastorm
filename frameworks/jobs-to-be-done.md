# Jobs to Be Done

**What this lens does:** Finds the functional, emotional, and social jobs a product or solution is actually hired to perform. People don't buy products — they hire them to make progress in specific circumstances. The job is the unit of analysis, not the customer segment.

**The milkshake insight:** McDonald's discovered people hired milkshakes for the morning commute job — boring drive, needed something to do with one hand for 23 minutes. The competitor wasn't other milkshakes. It was bananas and bagels. Knowing the job reveals who you're actually competing with.

## When NOT to Use

- The product is internal tooling with captive users — the "hiring" metaphor doesn't apply when there's no choice
- The job is already well-defined and validated — JTBD is a discovery tool, not a confirmation tool
- The problem is about technical architecture or implementation, not about what the user wants

## The Framework

| Dimension | Question |
|---|---|
| **Functional job** | What does it actually do? What task does it accomplish? |
| **Emotional job** | How does it make the person feel? What emotional state does it create or relieve? |
| **Social job** | How does it affect how others perceive them? What identity signal does it send? |
| **The circumstance** | When exactly does the job arise? What triggers the hire? What's happening in their life? |
| **The competing hire** | What were they doing before this existed? That's your real competition. |
| **The fire** | What would make them fire this solution and hire something else? |

## How to Run It

1. Define the job precisely: circumstance + desired progress + current obstacle
2. Identify all three dimensions: functional, emotional, AND social
3. Find the real competition (job competitors, not category competitors)
4. Ask the firing question: what would make them switch?

**Trap:** Stopping at the functional job. "I want a drill" is functional. "I want to feel like a competent homeowner in front of my partner" is the real job. The emotional and social dimensions are where differentiation lives.

## Agent Prompt

> "Apply Jobs to Be Done to the problem brief. Define the job precisely — functional job is the starting point, not the destination. Include emotional and social dimensions. Identify the specific circumstance that triggers the hire — what's happening in someone's life when they reach for this solution? Find the real competition (not category, but job). Ask what would make them fire this and hire something else.
>
> Write your Reframe (the job definition that differs from how the problem was stated — what are they actually hiring this to do?), Ideas (solutions optimized for the actual job, especially the emotional and social dimensions), and Wild Card (the competing 'hire' nobody is looking at — the most surprising thing that's competing for this job)."

## Output Format

```markdown
## Jobs to Be Done Output

**The job:**
- Functional: [What it actually does]
- Emotional: [How it makes them feel / what anxiety it relieves]
- Social: [What it signals to others / what identity it supports]
- Circumstance: [When exactly this job arises — the trigger]

**Real competition:** [What they hire instead — the surprising competitor]

**The firing condition:** [What would make them switch]

**Reframe:** [How the actual job differs from the stated problem — what's being hired to do what?]

**Ideas:**
- [Solution optimized for the real job, especially emotional/social dimensions]
- [Solution optimized for the real job, especially emotional/social dimensions]
- [Solution optimized for the real job, especially emotional/social dimensions]

**Wild card:** [The most surprising competitor for this job — the thing eating your lunch that nobody's watching]
```

## What Good Output Looks Like

- The job definition includes emotional and social dimensions that change the solution
- The real competition is genuinely surprising — not an obvious category competitor
- The firing condition reveals a latent vulnerability
- Ideas address the emotional or social job, not just the functional one
