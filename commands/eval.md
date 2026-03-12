---
name: eval
description: Run a before/after benchmark comparing a stock skill against its Lyra'd version. Proves the rewrite works with transparent, reproducible scoring.
---

Activate the Lyra Eval benchmark to compare two versions of the same skill.

The user should provide:
1. The stock skill (original version)
2. The Lyra'd skill (rewritten version)
3. Optionally: specific prompts to test, or use the default reflex-trigger set

Run the same prompts through the same model twice — once with the stock skill as system context, once with the Lyra'd version. Score both with the deterministic shadow grader and coherence metrics. Produce a comparison report showing the delta.
