# Six Behavioral Lenses

**What this lens does:** Runs a structured diagnostic across six psychological mechanisms to surface which are active, missing, or misapplied in a product, feature, or experience. Unlike the Behavioral Science framework (which applies Sutherland/Cialdini/Kahneman broadly), this is a specific six-lens teardown protocol. The diagnostic value is in which lenses are present AND which are absent.

**Root principle:** Human beings are narrative machines navigating toward the best story about themselves, not optimization machines navigating toward the best outcome. All six lenses are facets of this truth.

## When NOT to Use

- The problem is purely internal/operational with no customer-facing product to analyze
- You're brainstorming from scratch with no existing product or concept to teardown — this is analytical, not generative
- The Behavioral Science framework already covers the ground (check: are you asking "what biases are in play?" or "which of these six mechanisms are active/missing?" — if the former, use Behavioral Science instead)

## The Six Lenses

| Lens | Question | Key Note |
|---|---|---|
| **Rationalization Engine** | What alibi is the customer's brain grabbing to rubber-stamp the emotional decision? | The rational mind scans for alibis, not evaluates claims. One specific claim beats ten abstract ones. |
| **Scarcity as Transformation** | Is this presented as a product or an event? Does a temporal boundary change its psychological category? | Time-bound offerings aren't just more desirable — they become a different *kind* of thing. An event, not a product. |
| **Dimension Shifting** | What axis is everyone else competing on? Is this product on a new one? | The brain detects categorical novelty, not incremental improvement. 15% better is invisible. A new dimension is a different neurological event. |
| **Shadow Product** | What's the functional product vs. the psychological job? Are they building for the right one? | The shadow product almost always drives the purchase. Patagonia sells "membership in a values tribe," not jackets. |
| **Identity Permission** | What identity tension does the customer feel? What version of themselves do they need permission to be? | People need permission to be the version of themselves that buys, not just permission to buy. Premium pricing IS a permission structure. |
| **Narrative Finitude** | Is this tellable? Does it have narrative structure? What's the sentence someone uses when telling a friend? | Stories require endings. "I was there" beats "I use this." Shareability requires a hard stop. |

## How to Run It

For each lens, answer three questions:
1. **Active?** Is this mechanism currently operating in the product/feature/experience?
2. **Missing?** Is this mechanism absent when it could be powerful?
3. **Misapplied?** Is this mechanism present but working against the goal?

Not all six apply to every situation. The diagnostic value is in the pattern — which are present AND which are absent.

## Agent Prompt

> "Apply the Six Behavioral Lenses teardown to this problem brief. For each of the six lenses (Rationalization Engine, Scarcity as Transformation, Dimension Shifting, Shadow Product, Identity Permission, Narrative Finitude), assess: is this mechanism active, missing, or misapplied in the current product/feature/experience?
>
> The diagnostic value is in the PATTERN — not just which lenses are active, but which are conspicuously absent. A missing lens is often the biggest opportunity.
>
> Write your Reframe (what the pattern of active/missing/misapplied lenses reveals about where the real opportunity is), Ideas (specific interventions that activate missing lenses or fix misapplied ones), and Wild Card (the lens that's most surprisingly absent or misapplied — the one whose activation would change the most)."

## Output Format

```markdown
## Six Behavioral Lenses Output

**Lens diagnostic:**
| Lens | Status | Assessment |
|---|---|---|
| Rationalization Engine | [active/missing/misapplied] | [One sentence] |
| Scarcity as Transformation | [active/missing/misapplied] | [One sentence] |
| Dimension Shifting | [active/missing/misapplied] | [One sentence] |
| Shadow Product | [active/missing/misapplied] | [One sentence] |
| Identity Permission | [active/missing/misapplied] | [One sentence] |
| Narrative Finitude | [active/missing/misapplied] | [One sentence] |

**Reframe:** [What the pattern reveals — where's the real opportunity?]

**Ideas:**
- [Intervention activating a missing lens or fixing a misapplied one]
- [Intervention activating a missing lens or fixing a misapplied one]
- [Intervention activating a missing lens or fixing a misapplied one]

**Wild card:** [The lens whose activation would change the most about this product/feature]
```

## What Good Output Looks Like

- The diagnostic table is specific, not generic — "Rationalization Engine: missing — there's no alibi for the parent to grab" not "Rationalization Engine: could be stronger"
- At least one lens is surprisingly absent — the one nobody was thinking about
- The pattern tells a story: "four active, two missing, and the two missing ones are the entire reason this feels flat"
- Ideas target the missing or misapplied lenses specifically, not general improvements
