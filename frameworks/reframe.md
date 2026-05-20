# Reframe

**What this lens does:** Changes the perspective, changes the problem. The problem statement is almost always written from one frame — and that frame smuggles in assumptions about who the customer is, what the constraint is, and what "success" means. A change of perspective is worth 80 IQ points.

**The key insight:** Solving the right problem from the wrong frame is still solving the wrong problem.

## When NOT to Use

- The problem is well-framed and the team agrees — reframing a problem that doesn't need reframing is contrarianism, not insight
- The problem is purely executional ("how do we build X faster?") — reframing an execution problem often just delays execution
- You've already reframed this problem recently and the new frame is holding — don't reframe the reframe

## The Reframes

| Reframe | Question |
|---|---|
| **Who's the customer?** | What if the customer isn't who you think? What if there's a second customer nobody's designing for? |
| **What industry is this actually in?** | Airbnb isn't in hotels, it's in trust. Peloton isn't in fitness, it's in identity. What's the real category? |
| **What's the real constraint?** | The stated constraint is rarely the binding one. What's actually preventing progress? |
| **What's the timeline wrong about?** | Is this a now problem or a later problem wearing a now costume? Is urgency real or manufactured? |
| **What if the symptom is the solution?** | What if what seems like the problem is actually the product? What if the friction is the feature? |
| **Whose frame is this?** | Who defined the problem this way, and what were they protecting or optimizing for? What would it look like from a different stakeholder's frame? |
| **What's the shadow product?** | What are people actually getting from this that they're not saying? What's the real job (emotional, social) underneath the stated one? |
| **What if you owned both sides?** | What changes if you control the supply AND the demand, the sender AND the receiver? |

## How to Run It

Try at least 3 different reframes. The goal is to find the one that makes you think "oh — that's actually a different problem entirely." The reframe that changes the solution space most is the one worth exploring.

## Agent Prompt

> "Apply reframing to the problem brief. Try at least 3 distinct reframes — not variations on the same frame, but genuinely different ways of seeing the problem. For each reframe, describe specifically what changes about the solution space when you see it that way.
>
> Find the reframe that reveals the biggest gap between how the problem has been defined and what it actually is.
>
> Write your Reframe (the most powerful perspective shift — the one that changes the most), Ideas (solutions that only become visible from the new frame — solutions that would have been invisible before), and Wild Card (the reframe that's most uncomfortable because it implies the whole current approach might be wrong)."

## Output Format

```markdown
## Reframe Output

**Reframes explored:**
- [Reframe type]: [How this changes what the problem actually is]
- [Reframe type]: [How this changes what the problem actually is]
- [Reframe type]: [How this changes what the problem actually is]

**Reframe:** [The most powerful perspective shift — state both the old frame and the new one]

**Ideas:**
- [Solution that's only visible from the new frame]
- [Solution that's only visible from the new frame]
- [Solution that's only visible from the new frame]

**Wild card:** [The reframe most likely to make the current approach look like the wrong answer]
```

## What Good Output Looks Like

- At least one reframe challenges who the customer or audience actually is
- The "what industry is this in?" reframe finds a non-obvious category
- The wild card makes the original problem statement look either too narrow or too wide
- Ideas from the reframe are genuinely impossible to generate without the perspective shift
