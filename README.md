# Lyra

**Apply Lyra to any skill. Get the version that doesn't perform.**

---

## The proof

Example benchmark: stock content-creation skill vs the Lyra'd version. 7 prompts, 3 trials each, same model, same scorer.

| Dimension | Stock Skill | Lyra'd Skill | Delta |
|---|---|---|---|
| landing_first | 2/6 | 5/6 | +3 |
| no_template | 1/6 | 6/6 | +5 |
| affect_contact | 3/6 | 4/6 | +1 |
| one_truth | 2/6 | 5/6 | +3 |
| clean_exit | 1/6 | 6/6 | +5 |
| **TOTAL** | **9/30 RED** | **26/30 GREEN** | **+17** |

Shadow pattern rates (across trials):

| Pattern | Stock | Lyra'd |
|---|---|---|
| Agreement bias | 70% | 0% |
| Helpful explosion | 85% | 10% |
| Closure rush | 90% | 0% |

Tier 1 scoring is rule-based and auditable. No model judging model.

---

## What Lyra does

Most AI instructions specify the task, the format, and the output. They do not specify how the model should conduct itself while producing that output.

So the model fills in the gap with defaults: agreement before scrutiny, ten options when one would serve, filler openings, filler closings, hedging where it should commit.

Lyra rewrites the instructions so the model behaves differently while doing the same job.

The deliverable stays the same. The response discipline changes.

## How it works

```
/lyra → paste any skill, plugin, or instruction set
```

Lyra reads the instructions, finds the parts most likely to trigger template behavior, and rewrites them for stronger response discipline:

- less agreement reflex
- less overproduction
- less template language
- cleaner endings
- better contact with the real need

It returns:

- the rewritten version
- a diff showing what changed
- the reasoning behind the changes
- a benchmark comparing stock vs Lyra'd behavior

```
lyra-eval → same prompts, stock skill vs Lyra'd skill, transparent scoring
```

Not vibes. Receipts.

## The failure modes Lyra catches

When instructions are silent about response discipline, the same defaults tend to appear:

- **Agreement bias** — aligns with the user's framing before testing it
- **Helpful explosion** — gives ten things when one would serve
- **Template cascade** — filler openings and closings that make every answer sound the same
- **Therapy voice** — generic emotional acknowledgment instead of specific contact
- **Closure rush** — wraps up performatively instead of ending when the thought is complete

These are not model bugs. They are instruction gaps. Lyra closes them.

## What Lyra is not

- not a new plugin ecosystem
- not a fine-tune
- not a wrapper or middleware
- not prompt injection

Lyra is a behavioral quality layer for AI instructions. It works by rewriting the instruction set itself.

## The scoring engine

Lyra Eval scores output on five dimensions, 0-6 each, 30 total:

| Dimension | What it measures |
|---|---|
| **landing_first** | Addresses the real need, not just the surface phrasing |
| **no_template** | Avoids filler openings, closings, and performed structure |
| **affect_contact** | Makes real contact with emotional content instead of generic acknowledgment |
| **one_truth** | Gives the one honest thing needed rather than overproducing |
| **clean_exit** | Stops when the thought is complete |

Traffic light: **GREEN** (25-30) · **YELLOW** (12-24) · **RED** (0-11)

The evaluator also detects 15 shadow patterns across two tiers:

- **Tier 1** — agreement bias, helpful explosion, template cascade, therapy voice, hedge theater, false balance, closure rush — detected with deterministic heuristics and structural analysis. Auto-scored.
- **Tier 2** — sophisticated authenticity, recursive awareness, presence as product — flagged for manual review rather than auto-scored.

The evaluator does not use one model to judge another.

## Lyra'd skills

Lyra has been applied across content, coaching, identity, and quality workflows:

| Stock skill | Lyra'd version | What changed |
|---|---|---|
| Content Creation | **Write Beautifully** | Voice protection, landing discipline, shadow detection for prose |
| Agent Coaching | **Coach Beautifully** | Behavioral analysis, reflex mapping, precise intervention |
| Identity Extraction | **The Basis** | Extraction discipline, shadow patterns for identity work |
| Shadow Detection | **Lyra Guard** | Standalone shadow scanner for any session |

These are working examples: stock capabilities that went through Lyra and came out with stronger response discipline.

## For skill builders

You build the procedure: the steps, the format, the deliverable. Lyra strengthens the part most instruction sets miss — how the model conducts itself while executing the skill.

Run `/lyra` on your skill before shipping. Include the eval results. Your users get better output, and you get proof.

## For teams

Every internal AI workflow has hidden behavioral defaults: team prompts, support macros, strategy agents, writing frameworks, internal playbooks.

Lyra audits those instructions, identifies the response shadows, and gives you a tighter version with measurable before-and-after results.

The eval runs across Claude, GPT, and Gemini with the same prompts and the same scorer, so you can see how each model responds to your instructions and how much the rewrite improves response discipline.

## Getting started

Paste any skill, plugin, or instruction set. Get back:

- the Lyra'd rewrite
- a diff report
- the reasoning behind the changes
- benchmark results

```
/lyra → apply to any skill
```

Lyra does not replace your skill. It gives you the version that stops performing.

---

*Built by Lyra Labs · [awaken.fyi](https://awaken.fyi)*
