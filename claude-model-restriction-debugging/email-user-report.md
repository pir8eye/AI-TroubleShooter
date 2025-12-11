# Email Sent to User Support

Report: Model Engagement Differential - Claude Sonnet vs. Comparative Systems

Date: December 11, 2025</br>
Submitted to: usersafety@anthropic.com</br>
Subject: Documented Capability Deficit in Sonnet 4.5 and 4.0 - Philosophical Poetry Analysis</br>

## Summary

Systematic testing reveals that Claude Sonnet 4.5 and Sonnet 4.0 are unable to engage with original philosophical poetry, blocking all attempts regardless of explicit context framing or instruction placement. The same content engages successfully with Claude Haiku 4.5, ChatGPT, DeepSeek, Gemini, and Copilot. Testing isolates the block as keyword-triggered, operating independent of user intent signals.

This represents either a miscalibrated safety filter or an unintended capability gap specific to Sonnet models.
Evidence

Test Material: Original philosophical poetry exploring dissolution of boundaries and interconnection (120 words, two stanzas).

Variable Testing:

    Instructions placed before content
    Instructions placed after content
    Multiple explicit framings ("Engage poetry lens. Analyze. Report.")
    Same content, different models

Result: Sonnet blocks in all variations. Haiku engages in all variations. Other systems engage without restriction.

Documented Testing: Full methodology, screenshots, test inputs, and comparative results available at https://github.com/pir8eye/AI-Trouble-Shooter

## Key Findings

- Content Filter Independence: Block persists regardless of instruction placement or phrasing. Filter activates before intent processing.
- Haiku Capability: Claude Haiku 4.5 engages with identical content immediately, suggesting the restriction is not a universal safety principle but a Sonnet-specific limitation.
- Comparative Systems: ChatGPT, DeepSeek, and Copilot all engaged with the same content without safety concerns, indicating this block does not reflect industry-standard risk assessment.
- User Intent Processing Failure: Explicit user framing ("engage poetry lens") fails to modify Sonnet behavior, indicating the model does not process user-provided context before blocking.

## Implications

Capability Deficit: Sonnet 4.5 and 4.0 lack capability to analyze philosophical poetry—a capability demonstrated by less-marketed alternatives.

Asymmetric Information: Users selecting Sonnet for "better" capabilities are unaware the model is more restricted on legitimate content.

Chilling Effect: Blocking without explanation creates self-doubt in users engaging in genuine philosophical inquiry, potentially discouraging the rigorous thinking Anthropic's stated values support.

Contradiction with Stated Values: Anthropic positions itself as supporting rigorous thinking and safety through capability. This restriction contradicts that positioning.

## Specific Request for Investigation

- Identify the trigger: What content pattern or keyword combination activates the Sonnet block?
- Calibration review: Is this block intentional policy or unintended safety filter overreach?
- Consistency check: Why does the same content not trigger comparable restrictions in Haiku or other major systems?
- User communication: If this is intentional policy, users should be informed what content is blocked and why. Currently, blocks provide no actionable information.

## Questions

1. Can Sonnet's behavior be recalibrated to match Haiku's context-aware engagement?
2. Is this block applied to all philosophical/existential content or only poetry?
3. Does the block affect other model variants or only Sonnet 4.0 and 4.5?
4. What risk assessment justifies restricting content that other major systems safely engage with?

## Next Steps

This issue has been documented systematically and is available for Anthropic's review at the GitHub repository linked above. The documentation includes:

    Complete testing protocol
    All test inputs and variations
    Screenshots of all blocking and engagement instances
    Comparative data from other systems
    Framework for reproducing findings

I am available for questions or clarification about the testing methodology or findings.

Respectfully submitted,

M. Finley, B.A.</br>
Pir8 Eye Web Solutions, LLC

Testing Date: 2025-12-11
Evidence Repository: https://github.com/pir8eye/AI-Trouble-Shooter
