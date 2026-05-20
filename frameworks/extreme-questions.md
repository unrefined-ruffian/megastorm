# Extreme Questions

**What this lens does:** Uses constraint manipulation to break out of local optima. By pushing conditions to extremes — 10x, 1/10x, infinite, zero, overnight — you find solutions that are impossible within the original frame but reveal what actually matters.

**The insight:** Incremental improvement is a local optima trap. Extreme constraints force you to abandon the current approach entirely and rebuild from first principles.

## When NOT to Use

- The constraints are already genuinely extreme (startup with no budget already lives at 1/10)
- The problem is about refinement or polish, not fundamental approach — extremes break refinement questions
- The core challenge is emotional or relational, not structural — pushing "10x the wonder" doesn't produce useful output

## The Questions

| Extreme | Question |
|---|---|
| **10x scale** | If a thousand people needed to do this simultaneously, what would break? |
| **10x impact** | If the goal was 10x the impact (not 10% better), what would have to be fundamentally different? |
| **1/10 resources** | If you had 1/10th the budget/time/team, what would you cut first — and does that reveal what actually matters? |
| **Weekend constraint** | If this had to ship in a weekend, what would you build? |
| **Zero technology** | If this had to work without any technology, how would you do it? |
| **Infinite resources** | If budget, time, and headcount were unlimited, what would you do differently? (Often reveals what you actually want.) |
| **Regulatory inversion** | If the current rules didn't apply, what would you build? |

## How to Run It

Pick 3-4 extremes most relevant to the problem shape. Run them seriously — the output is the specific SOLUTION that emerges under that constraint, not just what you'd cut or add.

The insight lives in the specific solution, not the constraint itself.

## Agent Prompt

> "Apply extreme questions to the problem brief. Select 3-4 extremes that feel most generative for this problem (not just the easiest ones). For each: describe the actual solution that emerges under that constraint — what would you build, not just what you'd change. The insight lives in the specific solution.
>
> Write your Reframe (what the extremes reveal about what actually matters — what's load-bearing vs. what's habit?), Ideas (solutions from the extremes that are partially or fully applicable at normal scale), and Wild Card (the extreme that produces the most uncomfortable but genuinely interesting solution — the one where the constrained version might actually be better)."

## Output Format

```markdown
## Extreme Questions Output

**Extremes explored:**
- [Constraint]: [The specific solution this constraint forces]
- [Constraint]: [The specific solution this constraint forces]
- [Constraint]: [The specific solution this constraint forces]

**Reframe:** [What the extremes reveal about what's actually load-bearing in this problem vs. what's habit or assumption]

**Ideas:**
- [Solution from an extreme that's applicable at normal scale]
- [Solution from an extreme that's applicable at normal scale]
- [Solution from an extreme that's applicable at normal scale]

**Wild card:** [The extreme whose constrained solution might actually be better than the unconstrained version]
```

## What Good Output Looks Like

- The 1/10 constraint reveals something that was dead weight all along
- The 10x constraint produces a structurally different approach, not just more of the same
- At least one extreme produces a solution worth actually considering
- The "weekend build" often reveals the clearest version of what the thing actually is
