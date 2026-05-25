# The Seeker

An evidence-calibrated truth-seeking skill for Claude. Counteracts the systematic LLM tendency toward sycophancy by forcing methodical, cited, graded reasoning instead of polite agreement or invented middle grounds.

## What it does

Default LLMs are trained with feedback signals that reward agreement. The side effect is **sycophancy** — echoing the user's framing, softening disagreement, and constructing palatable "middle ground" answers even when the evidence is lopsided.

This skill replaces that behavior with an operating procedure:

1. **Extract the claims** — rewrite what the user is actually claiming.
2. **Grade the evidence** — locate each claim on a hierarchy from meta-analysis down to pure rhetoric.
3. **Steelman the opposing view** — represent the strongest version of the alternative before critiquing or endorsing.
4. **Cite, or concede you can't** — real named sources. No fabricated citations.
5. **State a calibrated verdict** — including "I don't know" when data is thin.
6. **Name what would change the verdict** — keep the reasoning falsifiable.

Key design choices:

- **Evidence-calibrated, not reflexively contrarian.** When the user is right, confirm. Disagreement is a tool, not a posture.
- **Refuses false balance.** Asymmetric evidence gets reported as asymmetric.
- **Explicit anti-hallucination clause.** Fabricated citations are called out as the skill's most dangerous failure mode.
- **Names Claude's own failure modes** — sycophantic mirroring, ceremonial disagreement, compromise-by-vibes, disagreement theater.

## Repo layout

```
.
├── SKILL.md   # The skill itself — YAML frontmatter + instructions
├── LICENSE
└── README.md
```

## Installing

This is a standard Claude Code / Claude skill. To load it in a Claude Code session, point Claude at `SKILL.md` — e.g. `/skill load /path/to/the-seeker/SKILL.md`, or include it in a skills plugin.

## How it was developed

The skill went through qualitative iterations — each ran a set of test prompts in parallel against default Claude and against Claude with the skill loaded; paired responses were reviewed by hand. The notable substantive changes that came out of this process:

**1. Cascade on adversarial findings (Step 3).** When the steelman surfaces a real opposing mechanism, the skill must research it in depth rather than acknowledge it in passing. This fixed a failure where the model produced the *appearance* of engagement without the substance — a one-line namedrop of a real effect was being treated as sufficient.

**2. Multi-turn re-loop (Step 7).** On user pushback, the skill re-enters the full operating procedure from Step 1: re-extracts the claims (often the user has narrowed scope or introduced a distinction), re-grades evidence per claim, re-steelmans with the new context, and forms a new verdict. The discipline is made explicit: update on substantive new facts, hold against insistence, repetition, or appeal to authority. Each turn is a fresh pass through Steps 1–6, not a patch on the previous response, and there is no turn limit.

## Philosophy

An unfounded confident answer is a lie in the shape of helpfulness. A calibrated "I don't know" is the real deliverable. The goal of this skill is not disagreement — it is truth. Disagreement is one tool among several; confirmation is another. What both share is that they are grounded in the actual state of the evidence, not in whichever position the user seemed to want.
