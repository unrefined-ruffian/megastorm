# Megastorm

**Multi-framework brainstorming for Claude Code. Ten brains, none of them talking to each other, one synthesis agent at the end.**

Most brainstorms collapse into whoever has the loudest voice — or whoever's framework you happened to read most recently. Megastorm runs 3–5 cognitive frameworks in parallel, each in an isolated agent that can't see the others, then converges the output into ranked insights with a synthesis agent. The frameworks can't groupthink because they don't know the others exist.

It's the brainstorming move you'd run if you had ten consultants who hated each other.

---

## What it does

Give it a problem. It:

1. **Reads the problem** — pulls context from your project files, asks targeted questions if the brief is thin.
2. **Picks the right frameworks** — classifies your problem shape ("this is a positioning problem," "this is a root cause problem") and selects 3–5 lenses that actually fit. You can override.
3. **Runs them in parallel, in isolation** — each framework agent gets the brief and its own instructions. They can't cross-pollinate.
4. **Synthesizes** — finds convergence across frameworks (multiple lenses pointing the same way = signal), surfaces tensions (where they disagree is where the real trade-offs live), and ranks the output.

You get a TLDR with the actual punches landing, and a Deep Dive with the full reasoning chains.

## The framework library

Ten lenses ship in the box:

| Framework | What it sees |
|---|---|
| **Inversion** | Make it maximally terrible, then flip everything |
| **Six Hats** | Six cognitive modes — facts, emotion, devil's advocate, optimism, creativity, process |
| **Five Whys** | Drill past symptoms until you hit something structural |
| **Extreme Questions** | What if 10x scale? 1/10 budget? Weekend build? Zero technology? |
| **Reframe** | Change the perspective, change the problem |
| **Jobs to Be Done** | What is this product actually hired to do? |
| **Behavioral Science** | Sutherland / Cialdini / Kahneman — design for the human that exists, not the one you wish existed |
| **Six Behavioral Lenses** | A diagnostic teardown — shadow product, identity permission, scarcity-as-event, dimension shifting, rationalization, narrative finitude |
| **Identity Persuasion** | The product is an identity trade. Who does the user become by engaging? |
| **Anti-Incumbent** | Map every attribute incumbents share, invert them all, find the breakout product in the negative space |

Each framework is a single `.md` file in `frameworks/`. They're modular. The router automatically considers any file in the directory — drop in a new one and it becomes available.

## Install

Megastorm is a [Claude Code skill](https://docs.claude.com/en/docs/claude-code). It installs into your local skills directory.

```bash
git clone https://github.com/unrefined-ruffian/megastorm.git ~/.claude/skills/megastorm
```

That's it. In Claude Code, you can now type `/megastorm` and it'll run.

## Usage

In any Claude Code session:

```
/megastorm

I'm trying to figure out how to make a new coffee shop interesting
in a market where every café looks like every other café. What's
the wedge?
```

Megastorm will:

1. Confirm the problem brief with you (and ask anything missing).
2. Propose 3–5 frameworks with one-line rationale for why each one fits *this* problem (not generic descriptions).
3. Wait for your confirmation, then run the framework agents in parallel.
4. Hand back the synthesis — TLDR up top, full reasoning underneath, and a "Tiny Experiment" suggesting the cheapest test that would validate the biggest insight.

You can also seed the problem with context. If you've got a CLAUDE.md or project notes, megastorm reads them and skips the interview.

## Adding your own framework

Create a new `.md` file in `frameworks/` following the pattern of the existing ones:

- **What this lens does** — one paragraph
- **When NOT to use** — the failure modes
- **The framework** — the actual structure
- **How to run it** — 3–6 steps
- **Agent prompt** — what the parallel agent receives
- **Output format** — what good output looks like

The router will pick it up on the next run.

If you build something useful, PRs welcome.

## Design principles

A few things baked into how this works, in case you want to fork it:

- **Parallel isolation, not sequential.** Frameworks see the brief, not each other. Sequential frameworks contaminate each other's thinking.
- **The router classifies the problem shape first.** Generic framework selection is the failure mode. Every framework should be picked for a stated reason.
- **Five frameworks is the ceiling.** Synthesis degrades above five. The router holds firm on this.
- **TLDR is not compressed summary.** It's the insights written with full force, just without the analysis scaffolding. Compression that kills the juice is worse than length.

## License

MIT. See [LICENSE](LICENSE).

## Credits

Built by [Justin Williams](https://github.com/unrefined-ruffian).

The frameworks stand on shoulders — Charlie Munger (inversion), Edward de Bono (six hats), Sakichi Toyoda (five whys), Clayton Christensen (jobs-to-be-done), Rory Sutherland / Robert Cialdini / Daniel Kahneman (behavioral science), and a lot of marketing-Twitter that recognized Liquid Death for what it was.
