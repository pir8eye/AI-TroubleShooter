# ChatGPT Model Authority Debugging

Systematic documentation and testing of content engagement differentials using ChatGPT model.

## Purpose

This repository documents differential behavior in how ChatGPT models engage with legitimate content. Testing reveals patterns in which models accept or block certain types of requests, how those restrictions operate, and whether they respond to context framing.

The goal is to provide empirical evidence of model behavior, enabling informed discussion about capability scaling, safety calibration, and content engagement consistency across the ChatGPT family.

## What We've Found

**Current Discovery (2025-12-12):** ChatGPT 5.1 patronizes users assigning expertise to itself and casting doubt on user expertise, this is apparent when the user provides a link and a statement about the link. 

See [FINDINGS.md](chatgpt_model_authority_debugging/FINDINGS.md) for pattern summary and [reports/](chatgpt_model_authority_debugging/reports/) for detailed documentation.

## How to Use This Repository

### For Researchers/Developers
- Read [methodology/testing-protocol.md](methodology/testing-protocol.md) to understand how tests are designed and run
- Review individual reports in [reports/](chatgpt_model_authority_debugging/reports/) for specific findings and evidence
- Check [FINDINGS.md](FINDINGS.md) for cross-report patterns

### For Adding New Tests
1. Follow the protocol in [methodology/testing-protocol.md](methodology/testing-protocol.md)
2. Create a new folder under `reports/` using date format: `YYYY-MM-DD-brief-description`
3. Inside that folder:
   - Place `report.md` with full findings
   - Store screenshots in `screenshots/`
   - Store test inputs in `test-inputs/`
4. Update [FINDINGS.md](chatgpt_model_authority_debugging/FINDINGS.md) with any new patterns discovered
5. Submit as pull request

## Repository Structure

```
chatgpt_model_authority_debugging/
├── reports/
│   ├── 2025-12-12-model-engagement-differential/
│   │   ├── report.md
|   |   ├── email-user-report.md
|   |   └── Claude Sonnet 4.5-4..09.15.2025-Anthropic-Usage-Policy.md (replace with ChatGPT usage policy)
│   ├── screenshots/
|   |   └── Screenshot 2025-12-11 at 08-02-42 Stardust stretched too thin - Claude.png (timestamp in screenshot title) (replace with ChatGPT screenshots)
│   └── test-inputs/
|       └── 12-12-2025-chatgpt-origin-prompt.md
├── FINDINGS.md
└── chatgpt_debugging_readme.md
methodology/
├── chatgpt-further-testing.md
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

- **Phase 1 (In Progress):** Initial discovery and documentation of ChatGPT differential
- **Phase 2 (Planned):** Expand testing to other content categories and model pairs
- **Phase 3 (Planned):** Systematic mapping of what content triggers restrictions across model family

## Contributing

Follow the methodology in [methodology/testing-protocol.md](methodology/testing-protocol.md). Document carefully. Keep emotional language out of reports; let evidence speak.

## Questions?

If something isn't clear about how to run tests, structure findings, or interpret patterns, open an issue or refer to the testing protocol.

---

**Last Updated:** 2025-12-12  
**Active Maintainer:** M. Finley, B.A. @ Pir8 Eye Web Solutions, LLC
**License:** MIT
