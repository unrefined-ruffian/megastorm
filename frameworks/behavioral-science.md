# Behavioral Science

**What this lens does:** Applies the insights of behavioral economics and persuasion psychology to find solutions that work WITH human nature rather than against it. Rory Sutherland's core thesis: the most effective interventions are often psychological, not functional. Logic solves the wrong problem with impressive precision.

**The key insight:** Humans are not rational agents making optimal decisions. They are prediction machines running on heuristics, social signals, and emotional shortcuts. Design for the human that actually exists, not the human you wish existed.

## When NOT to Use

- The problem is purely technical with no human decision point — behavioral science needs a human making a choice to have leverage
- The audience is a machine or API consumer — heuristics don't apply to programmatic callers
- You're tempted to use it to manipulate rather than serve — behavioral levers should make the right choice easier, not trick people into the wrong one

## The Key Thinkers

**Rory Sutherland:** Psycho-logic beats logic. Reframe value, don't optimize function. "The opposite of a good idea can also be a good idea." Solutions that seem irrational often work better than rational ones because they operate on the actual decision-making system.

**Robert Cialdini — The Seven Levers:**
- **Reciprocity** — People repay what they receive
- **Commitment/Consistency** — People follow through on prior commitments
- **Social Proof** — People look to others when uncertain
- **Authority** — People defer to credible experts
- **Scarcity** — Less available = more desirable
- **Liking** — People say yes to people they like
- **Unity** — Shared identity creates compliance

**Kahneman — Dual Systems:**
- **System 1:** Fast, automatic, emotional, heuristic-driven — makes most decisions
- **System 2:** Slow, deliberate, rational — rationalizes what System 1 already decided

You are almost always designing for System 1, even when you think you're designing for System 2.

**Ariely — Predictable Irrationality:**
- Loss aversion: losses feel 2x worse than equivalent gains
- Anchoring: first number heard dominates perception
- Default effects: whatever is default gets chosen
- Framing: same outcome feels different depending on how it's presented

## How to Run It

1. Identify which cognitive bias or psychological principle is currently working against the goal
2. Ask: "Could we make this bias work FOR us instead?"
3. Apply the Sutherland lens: what's the psycho-logical solution that pure logic would never find?
4. Check which Cialdini lever is being ignored or actively violated

## Agent Prompt

> "Apply behavioral science to the problem brief. Identify 2-3 behavioral levers (cognitive biases, psychological principles, or persuasion mechanisms) that are most relevant to this problem. For each: name the specific mechanism, describe how it currently operates in this context (is it being activated? ignored? violated?), and propose a specific intervention that works with it rather than against it.
>
> Apply Rory Sutherland's lens: what's the psycho-logical solution — the intervention that seems irrational but works because it operates on the actual human decision system?
>
> Write your Reframe (the behavioral insight that shifts how you see the problem — what's the psychological dynamic underneath the surface problem?), Ideas (specific interventions that leverage named psychological mechanisms), and Wild Card (the Sutherland move — the intervention that looks wrong to a rational optimizer but is exactly right for an emotional human)."

## Output Format

```markdown
## Behavioral Science Output

**Behavioral levers in play:**
- [Mechanism]: [How it currently operates — for or against the goal?]
- [Mechanism]: [How it currently operates — for or against the goal?]
- [Mechanism]: [How it currently operates — for or against the goal?]

**Reframe:** [The psychological dynamic underneath the stated problem — what's actually happening in the human's head?]

**Ideas:**
- [Intervention leveraging a specific named mechanism]
- [Intervention leveraging a specific named mechanism]
- [Intervention leveraging a specific named mechanism]

**Wild card:** [The Sutherland move — the intervention that seems irrational, that a logic-optimizer would reject, but that works because it speaks to System 1]
```

## What Good Output Looks Like

- Names specific mechanisms (loss aversion, social proof, default effect) — not generic "psychology" or "emotion"
- Identifies at least one lever that's currently working AGAINST the goal that could be flipped
- The wild card is genuinely counterintuitive from a rational-optimization standpoint
- The Sutherland move should feel slightly wrong to a product manager and completely right to a behavioral scientist
