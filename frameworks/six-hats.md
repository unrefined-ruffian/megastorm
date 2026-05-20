# Six Thinking Hats

**What this lens does:** Forces structured movement through six distinct cognitive modes. Prevents groupthink by explicitly separating logic, emotion, creativity, caution, optimism, and process. Each hat produces outputs the other hats suppress.

**The key insight:** Most thinking mixes modes, which is why it's mediocre. A room full of cautious people will never generate a green hat idea. A room full of optimists will never properly stress-test.

## When NOT to Use

- The problem is narrow and emotional — pure delight/wonder problems often don't benefit from the white hat's data demands or the blue hat's process focus
- Time pressure requires depth on one angle rather than breadth across six
- The problem is already well-understood from multiple perspectives — six hats works best when a group is stuck in one mode

## The Six Hats

| Hat | Mode | The Discipline |
|---|---|---|
| **White** | Facts and data only | What do we know? What's missing? No opinions. |
| **Red** | Pure emotion | What's the gut response? No justification required or allowed. |
| **Black** | Devil's advocate | What could go wrong? What are the risks? Be rigorous, not cynical. |
| **Yellow** | Optimism | What's the best case? What are the genuine benefits? |
| **Green** | Creative | Wild ideas, new approaches, provocations. Weird on purpose. |
| **Blue** | Process and control | What's the structure? What's the next step? What are we missing? |

## How to Run It

Cycle through each hat quickly. The constraint of one hat at a time is the entire point — don't blend modes.

**White:** Facts only. If you catch yourself evaluating, you've switched hats.
**Red:** No justification. "I feel uneasy about this" is a complete red hat statement.
**Black:** Rigorous pessimism, not nihilism. Specific risks, not vague doubt.
**Yellow:** Find the genuine value, not cheerleading. Why could this work?
**Green:** The weirder the better. No self-editing.
**Blue:** Step back. What's the shape of this problem? What have we not considered?

## Agent Prompt

> "Apply De Bono's Six Hats to the problem brief. For each hat, give 2-3 specific outputs that could ONLY come from that mode — no blending. White hat stays factual (no opinions). Red hat has no justification (feeling is the data). Green hat must be genuinely strange. Black hat names specific risks, not vague concern.
>
> Write your Reframe (what the full hat cycle reveals about the problem that no single perspective could), Ideas (the strongest outputs from any hat that deserve real consideration), and Wild Card (the green hat idea that's most uncomfortable — the one that sounds crazy but might not be)."

## Output Format

```markdown
## Six Hats Output

**Reframe:** [What the combination of perspectives reveals that no single hat could]

**Ideas:**
- [Strongest idea from the full cycle, noting which hat it came from]
- [Strongest idea from the full cycle, noting which hat it came from]
- [Strongest idea from the full cycle, noting which hat it came from]

**Wild card:** [The green hat idea that's most uncomfortable — the one worth investigating despite the discomfort]
```

## What Good Output Looks Like

- White hat surfaces a data gap nobody mentioned
- Red hat says something true that feels slightly embarrassing
- Black hat names a specific risk, not a vague concern
- Green hat gets genuinely strange — not "add a feature," something structurally different
- Blue hat reveals a meta-problem nobody was talking about
