# Provenance

This is an original Manus Skill informed by general quality-assurance ideas found in the sources below. No code, scripts, or expressive text was copied. The repository licenses are recorded for transparent attribution; this Skill does not redistribute their materials.

- `nimadorostkar/Claude-Skills-collection`, `skills/data/data-quality/SKILL.md`, MIT, commit `42bfec757076d9f4d4bda2f885c78873e6b85cc2`: https://github.com/nimadorostkar/Claude-Skills-collection/tree/42bfec757076d9f4d4bda2f885c78873e6b85cc2/skills/data/data-quality
- `Votee-AI/magic-agent-skills`, `magic-data-validation` and `magic-data-profiling`, Apache-2.0, commit `09bec2dfc332e5aad9cfb620f022b02137eadb82`: https://github.com/Votee-AI/magic-agent-skills/tree/09bec2dfc332e5aad9cfb620f022b02137eadb82
- `wshobson/agents`, `plugins/data-engineering/skills/data-quality-frameworks/SKILL.md`, MIT, commit `1eecf4b58eb380ff7ddc258a11c6586381d67b95`: https://github.com/wshobson/agents/tree/1eecf4b58eb380ff7ddc258a11c6586381d67b95/plugins/data-engineering/skills/data-quality-frameworks

The Manus adaptation is narrower: a read-only-first, evidence-based audit of user-provided CSV/Excel files. It does not install or configure Great Expectations, dbt, or the upstream Python scripts. It reuses Manus-native data-analysis and spreadsheet/document capabilities.
