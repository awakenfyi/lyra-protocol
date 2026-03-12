---
name: lyra
description: Apply the Lyra Protocol to any skill, plugin, or instruction set. Paste a skill or point at a file — get the version that doesn't perform.
---

Activate the `lyra-protocol:apply` skill to rewrite the provided skill with behavioral discipline.

If the user pasted text, treat it as the skill to rewrite.
If the user provided a file path, read that file and treat it as the skill to rewrite.
If the user named a plugin or skill, find the SKILL.md and treat it as the skill to rewrite.

Run the full rewrite engine: scan for instruction shadows, identify behavioral gaps, rewrite with the three guards (landing, volume, exit), and produce both the rewritten skill and the diff report.
