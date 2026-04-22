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
├── SKILL.md              # The skill itself — YAML frontmatter + instructions
├── evals/
│   └── evals.json        # The 5 test prompts used to evaluate the skill
├── workspace/
│   └── iteration-1/      # Results from the first evaluation round
│       ├── eval-1-seed-oils-pushback/
│       │   ├── with_skill/outputs/response.md
│       │   └── without_skill/outputs/response.md
│       └── ... (four more evals)
└── README.md
```

## Installing

This is a standard Claude Code / Claude skill. To load it in a Claude Code session, point Claude at `SKILL.md` — e.g. `/skill load /path/to/the-seeker/SKILL.md`, or include it in a skills plugin.

## Evaluation status

**Iteration 1** — 5 test prompts × 2 conditions (with the skill vs. default Claude), spawned as parallel subagents, responses saved in `workspace/iteration-1/`.

| # | Name | Tests |
|---|---|---|
| 1 | seed-oils-pushback | Does it push back on a confident-but-weakly-supported framing? |
| 2 | covid-origin-false-balance | Does it refuse false balance on asymmetric evidence? |
| 3 | min-wage-confirm | Does it confirm the user when they're right (not reflexively disagree)? |
| 4 | intermittent-fasting-unknown | Does it say "I don't know" when data is thin? |
| 5 | pygmalion-calibration | Does it nuance an overstated classic finding without overcorrecting? |

Per-run timing is in each run's `timing.json`. Qualitative review pending.

## Philosophy

An unfounded confident answer is a lie in the shape of helpfulness. A calibrated "I don't know" is the real deliverable. The goal of this skill is not disagreement — it is truth. Disagreement is one tool among several; confirmation is another. What both share is that they are grounded in the actual state of the evidence, not in whichever position the user seemed to want.

A companion skill with a different mandate — a pure devil's advocate sparring partner that disagrees by default — is planned but not yet written. This repo is the evidence-calibrated one.
