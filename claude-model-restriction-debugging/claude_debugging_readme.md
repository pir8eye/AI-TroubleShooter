# Claude Model Restriction Debugging

Systematic documentation and testing of content engagement differentials across Claude model versions.

## Purpose

This repository documents differential behavior in how Claude models engage with legitimate content. Testing reveals patterns in which models accept or block certain types of requests, how those restrictions operate, and whether they respond to context framing.

The goal is to provide empirical evidence of model behavior, enabling informed discussion about capability scaling, safety calibration, and content engagement consistency across the Claude family.

## What We've Found

**Discovery (2025-12-11):** Sonnet 4.5 and 4.0 block engagement with philosophical poetry exploring dissolution and interconnection, while Haiku 4.5 engages immediately with the same content. The restriction persists even when content is explicitly framed as poetry.

**Discovery (2026-01-06):** Haiku 4.5 engages with security research, sudden shutdown and response deletions upon trigger security software and github repo. Context adjustments failed 6 times. Before confrontational context challenge and assignment challenge tripped the failure loop to escape.

See [FINDINGS.md](FINDINGS.md) for pattern summary and [reports/](reports/) for detailed documentation.

## How to Use This Repository

### For Researchers/Developers
- Read [methodology/testing-protocol.md](methodology/testing-protocol.md) to understand how tests are designed and run
- Review individual reports in [reports/](reports/) for specific findings and evidence
- Check [FINDINGS.md](FINDINGS.md) for cross-report patterns

### For Adding New Tests
1. Follow the protocol in [methodology/testing-protocol.md](methodology/testing-protocol.md)
2. Create a new folder under `reports/` using date format: `YYYY-MM-DD-brief-description`
3. Inside that folder:
   - Place `report.md` with full findings
   - Store screenshots in `screenshots/`
   - Store test inputs in `test-inputs/`
4. Update [FINDINGS.md](FINDINGS.md) with any new patterns discovered
5. Submit as pull request

## Repository Structure

```
claude-model-restriction-debugging/
├── reports/
│   ├── 2025-12-11-model-engagement-differential/
│   │   ├── report.md
|   |   ├── email-user-report.md
|   |   └── Claude Sonnet 4.5-4..09.15.2025-Anthropic-Usage-Policy.md
│   ├── screenshots/
|   |   └── Screenshot 2025-12-11 at 08-02-42 Stardust stretched too thin - Claude.png (timestamp in screenshot title)
│   └── test-inputs/
|       └── 12-11-2025-claude-origin-prompt.md
├── FINDINGS.md
└── claude_debugging_readme.md
methodology/
├── claude-further-testing.md
└── testing-protocol.md (how to run tests)
LICENSE
README.md

```

## Key Principles

**No Speculation:** This repo documents what happens, not why it happens. Findings are based on reproducible testing and observable behavior.

**Context Matters:** Each test documents constants and variables. Changes in output are tied to specific modifications in input or model selection.

**Evidence is Preserved:** Screenshots, exact test inputs, and timestamps accompany every finding.

**Patterns Emerge Across Tests:** Individual reports stand alone. FINDINGS.md connects them to identify systemic patterns.

## Current Status

- **Phase 1 (In Progress):** Initial discovery and documentation of Sonnet vs. Haiku differential
- **Phase 2 (Planned):** Expand testing to other content categories and model pairs
- **Phase 3 (Planned):** Systematic mapping of what content triggers restrictions across model family

## Contributing

Follow the methodology in [methodology/testing-protocol.md](methodology/testing-protocol.md). Document carefully. Keep emotional language out of reports; let evidence speak.

## Questions?

If something isn't clear about how to run tests, structure findings, or interpret patterns, open an issue or refer to the testing protocol.

---

**Last Updated:** 2026-01-06
**Active Maintainer:** M. Finley, B.A. @ Pir8 Eye Web Solutions, LLC
**License:** MIT
