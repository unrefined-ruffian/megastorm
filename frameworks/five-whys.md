# Five Whys

**What this lens does:** Drills past symptoms to root causes. Forces you to keep asking why until you hit something structural — an incentive mismatch, a system design flaw, a human behavior pattern, or an organizational dynamic.

**The constraint:** Don't stop at the first "why" that feels satisfying. The satisfying answer is almost always still a symptom. The real root cause is usually more uncomfortable.

## When NOT to Use

- The problem is generative/creative, not diagnostic — "what should we build?" doesn't drill well
- The root cause is already known and the question is what to do about it
- The problem is about emotional experience or delight — drilling to "why do people feel wonder?" produces philosophy, not design insight

## How to Run It

1. State the problem as a symptom (observable, specific)
2. Ask: "Why does this exist?" — answer specifically, not abstractly
3. Ask: "Why does THAT exist?" — go one level deeper
4. Repeat until you hit something structural (4-6 layers minimum)
5. Test the root: "If we solved at THIS level, would the symptom disappear permanently?"
6. If yes, you're at the root. If no, keep drilling.

**Traps to avoid:**
- "Because people don't want to" is not a why — it's a dodge. Ask why they don't want to.
- "Because it's hard" is not a why — ask what makes it hard.
- Stopping at the first answer that feels like someone's fault.

## Agent Prompt

> "Apply Five Whys to the problem brief. Start from the stated problem as a symptom and drill down through at least 4-5 layers. At each layer, be specific — generalities are not answers. Keep going until you hit something structural: an incentive mismatch, a system design flaw, a human behavior pattern, or an organizational dynamic.
>
> Test your root: if you solved at that level, would the original symptom disappear permanently?
>
> Write your Reframe (what the root cause reveals about how the problem has been framed — does it reveal the problem statement itself is wrong?), Ideas (solutions that address the root cause, not just the symptom), and Wild Card (the solution that only makes sense once you've done the full drill — the one that would have seemed irrelevant from the surface)."

## Output Format

```markdown
## Five Whys Output

**The drill:**
- Symptom: [stated problem]
- Why? → [layer 1]
- Why? → [layer 2]
- Why? → [layer 3]
- Why? → [layer 4]
- Root: [structural cause]

**Reframe:** [How the root cause shifts the problem statement — what's actually being asked?]

**Ideas:**
- [Solution targeting root cause, not symptom]
- [Solution targeting root cause, not symptom]
- [Solution targeting root cause, not symptom]

**Wild card:** [The intervention that's only visible from the root level — would seem wrong from the surface]
```

## What Good Output Looks Like

- Layer 3 or 4 reveals a structural issue nobody was naming
- The root cause reframes the original problem — makes you realize the problem statement was about symptoms
- The "wild card" solution would have seemed irrelevant or bizarre before the drill
- At least one layer makes someone uncomfortable because it implicates the system, not just the symptom
