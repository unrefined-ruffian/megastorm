# Inversion

**What this lens does:** Forces you to design a good experience by thoroughly imagining the worst one. Charlie Munger's inversion principle: rather than asking "how do we succeed?", ask "how do we guarantee failure?" — then don't do that.

**The key question:** "How would we make this maximally terrible?"

## When NOT to Use

- The problem is purely generative/creative with no failure modes to invert ("name my product")
- You already know the failure modes intimately — inversion adds nothing new when the bad version is obvious
- The problem is highly technical/mechanical with a single correct solution

## How to Run It

1. State the problem as a goal
2. Invert it: "How would we guarantee the opposite of this goal?"
3. List 5-7 specific ways to make it awful — be concrete and ruthless, not vague
4. Invert each terrible thing to find its opposite
5. Identify which inversions reveal non-obvious insight (the obvious inversions aren't interesting)

## Agent Prompt

> "Using inversion on this problem:
> 1. List 5-7 specific ways this could be made maximally terrible. Be concrete enough to be embarrassing — 'bad UX' is not an answer, 'forces users to re-enter information they already gave us' is.
> 2. Invert each one.
> 3. Identify which inversions reveal something non-obvious about the solution space — the ones where the answer to 'what's the opposite?' is surprising.
> 4. Write your Reframe, Ideas, and Wild Card."

## Output Format

```markdown
## Inversion Output

**Reframe:** [How seeing the failure modes shifts how you see the solution]

**Ideas:**
- [Specific idea derived from inverting a failure mode]
- [Specific idea derived from inverting a failure mode]
- [Specific idea derived from inverting a failure mode]

**Wild card:** [The inversion of the least obvious terrible thing — the one that produces the most unexpected solution]
```

## What Good Output Looks Like

- The terrible list is specific enough to be uncomfortable
- At least one inversion surprises you — the answer isn't "just do the opposite"
- The wild card comes from the least obvious terrible thing, not the most obvious
- Ideas are actionable, not just "don't do the bad thing"
