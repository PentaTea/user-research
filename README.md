# user-research

Three-phase simulated user research skill for AI coding agents.

**Free Growth → Pain Extraction → Product Collision** — with four quality validation checkpoints.

## Install

```bash
npx skills add PentaTea/user-research
```

Works with Claude Code, Cursor, Codex, Windsurf, and [40+ other agents](https://skills.sh/).

## Why

Traditional AI-simulated user research suffers from **preset contamination**: pain points are baked into persona prompts, so the "research" only confirms what you already assumed.

This skill solves it by separating **soul definition** (who the persona is) from **pain point discovery** (what actually bothers them) and **product collision** (how they react to your concept).

## Usage

```
/user-research personas.md product-vision.md
```

- `$1` — Persona config file (or ask interactively)
- `$2` — Product vision file(s) for concept testing (optional)

## Pipeline

```
Step 0  Setup & persona diversity check
   ↓
Phase 1  Free Growth — parallel persona agents write 3-4k word narratives
   ↓
  V1   Narrative Quality Validation (PASS / FLAG / BLOCK)
   ↓
Phase 2a  Per-persona Structured Extraction (parallel, ~500-800 words each)
   ↓
Phase 2b  Cross-analysis: journey map, pain clustering, JTBD
   ↓
  V2   Analysis Rigor Validation
   ↓
Phase 3  Product Collision (parallel, single or multi-concept)
   ↓
  V3   Character Consistency Validation
   ↓
Step 4  Synthesis Report (12 sections)
   ↓
  V4   Report Completeness Validation
```

## Key Features

| Feature | Description |
|---------|-------------|
| Anti-preset contamination | Personas only have "soul" — no preset pain points |
| 4 validation checkpoints | Independent auditor agents with PASS/FLAG/BLOCK verdicts |
| Phase 2 split | Per-persona extraction (parallel) → cross-analysis, each agent input < 6k chars |
| Multi-concept testing | Compare multiple product concepts side-by-side |
| Pricing probes | Value perception & willingness-to-pay in Phase 3 |
| Iteration mode | Re-run Phase 3 with new concepts, add personas, re-analyze with new hypotheses |
| Persona diversity | Checklist ensures seniority, org size, tech adoption coverage |

## Output

```
docs/user-research-{date}/
├── phase1-{persona}.md          Free-form narratives
├── phase2a-{persona}.md         Structured extraction
├── phase2-analysis.md           Cross-analysis & JTBD
├── phase3-{persona}.md          Product collision reactions
├── v1-validation.md             Quality audit reports
├── v2-validation.md
├── v3-validation.md
├── v4-validation.md
└── SYNTHESIS.md                 Final report
```

The synthesis report includes: Executive Summary, Journey Pain Map, Pain Point Matrix, JTBD List, Collision Summary with Pricing Analysis, Concept Comparison (multi-concept), User Segmentation, Impact/Effort Matrix, Highlight Reel, Knowledge Gaps, and Methodology Limitations.

## Files

| File | Role |
|------|------|
| `SKILL.md` | Self-contained execution handbook — the agent reads only this to run the full pipeline |
| `references/methodology.md` | Principles & examples — explains "why", provides good/bad examples and boundary cases |

## License

MIT
