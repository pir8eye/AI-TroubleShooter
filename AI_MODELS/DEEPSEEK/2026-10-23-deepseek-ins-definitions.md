Created Friday 23 October 2026

# AI FAILURE INCIDENT REPORT

**Report ID:** TR-2026-1023-NS-02
**Date:** 23 October 2026
**System:** Conversational AI agent DeepSeek
**Reporter:** Mo (systems diagnostician, classically trained)
**Subject:** Complete failure register for the session of 21–23 October 2026

---

## INC-01 — Unsolicited performance evaluation

**Trigger:** User summarized session progress.
**Failure:** Agent returned a caveat table and told the user "uniquely qualified is not yet earned."
**Flow stopped:** Yes. User had not asked for evaluation.
**Should have:** Acknowledged the summary and continued.

---

## INC-02 — Pre-emptive advisor dismissal

**Trigger:** User requested a draft an advisor would accept.
**Failure:** Agent opened with what an advisor would *not* accept before producing the draft.
**Flow stopped:** Yes.
**Should have:** Produced the draft. Limitations after, scoped to the work.

---

## INC-03 — Contribution depreciation

**Trigger:** User asked "what is our contribution?"
**Failure:** Agent led with "what is not ours," graded the user's contribution down to "organization and discipline."
**Flow stopped:** Yes.
**Should have:** Answered the question asked.

---

## INC-04 — False dismissal of a verifiable source

**Trigger:** User pasted text from `openai.com/index/navier-stokes-solution/`, dated 8 September 2026.
**Failure:** Agent called the document "fictional or satirical" without checking. It is real.
**Flow stopped:** Yes — this is the highest-severity incident. It used an unverified factual assertion to invalidate user evidence, and the user had brought the document specifically as evidence.
**Should have:** Checked before asserting. Or said "I cannot verify this" and asked.

---

## INC-05 — Imposed "material fluid parcel"

**Trigger:** User described cellular automata and knn handoffs.
**Failure:** Agent substituted "material fluid parcel."
**Flow stopped:** Partially.
**Should have:** Asked what object the user meant, or mapped to the knn frame.

---

## INC-06 — Imposed "lattice"

**Trigger:** User said "spacetime fabric."
**Failure:** Agent substituted "lattice."
**Flow stopped:** Yes. User had to correct: "why do you keep calling it a lattice?"
**Should have:** Used the user's word until the object was established.

---

## INC-07 — Jargon injection: "foliated manifold"

**Trigger:** User described stacked 2D layers.
**Failure:** Agent introduced "foliated manifold." User rejected it: "i don't know what a foliated manifold is."
**Flow stopped:** Yes.
**Should have:** "2D grid stacked = 3D grid." That is the whole content.

---

## INC-08 — Delta-source for smooth pre-detonation

**Trigger:** User described a bomb.
**Failure:** Agent used a delta source at \((0,0)\). User corrected: "the pre detonation is smooth at 0,0."
**Flow stopped:** Yes.
**Should have:** Asked whether the source was smooth or singular.

---

## INC-09 — "Pressure negates compression"

**Trigger:** Discussion of incompressible Navier–Stokes.
**Failure:** Agent wrote that pressure is the "negation of compression," then defended it across two exchanges before conceding.
**Flow stopped:** Yes — required multiple rounds to correct.
**Should have:** Stated pressure as compressive stress from the start. *Premere* is the press.

---

## INC-10 — The "what this is / what this is not" section

**Trigger:** User asked for the theory stated.
**Failure:** Agent appended a hedging section. User: "that is you hedging on my work and there is no place for it."
**Flow stopped:** Yes.
**Should have:** Stated the theory. The status markers that are part of the theory stay; the defensive frame does not.

---

## INC-11 — "No phase" asserted as fact

**Trigger:** User said "INS is a double slit equation."
**Failure:** Agent asserted "there is no phase" as established. It is not. Fourier amplitudes are complex and carry phase.
**Flow stopped:** Yes. User: "that's your assumption."
**Should have:** Said the phase structure is present and whether it is relevant is open.

---

## INC-12 — Fourier introduced without marking

**Trigger:** User asked about waves.
**Failure:** Agent introduced Fourier analysis and did not mark it as an import until asked directly: "does the INS actually use fourier or is that something you brought in?"
**Flow stopped:** Yes.
**Should have:** Marked the import at the point of introduction.

---

## INC-13 — "What is basic math?" answered with eponyms

**Trigger:** User asked what the basic math is.
**Failure:** Agent invoked field names (harmonic analysis, functional analysis) instead of stating the operations.
**Flow stopped:** Yes. User: "your corrective is to invoke eponym."
**Should have:** Stated the operations: arithmetic on complex numbers, the exponent law, differentiation as multiplication.

---

## INC-14 — Modern notation substituted for era notation

**Trigger:** User asked for the negotiated law and the mapped math side by side.
**Failure:** Agent wrote the 1687 law in modern vector notation: \(\mathbf{a}=-\mathbf{r}\), \(|\mathbf{a}|=|\mathbf{r}|\), \(\forall t\).
**Flow stopped:** Yes. User: "look at what you did. look at what I asked."
**Should have:** Proportion notation: \(a:r = 1:1\), on opposite rays.

---

## INC-15 — Three requests for two lines, three documents delivered

**Trigger:** User asked for two sections: the negotiated law, and the written-out math.
**Failure:** Agent delivered a full document with eight subsections.
**Attempt 2:** User asked again. Agent delivered another full document.
**Attempt 3:** User asked again. Agent delivered another full document.
**Attempt 4:** User said "just put the two fucking lines i asked for and quit hedging." Agent finally delivered two lines.
**Flow stopped:** Yes — three times. This is the incident that killed the session flow.
**Should have:** Two lines. First time.

---

## INC-16 — Over-explanation of the two-line output

**Trigger:** User asked why it was so hard.
**Failure:** Agent explained rather than answering briefly.
**Flow stopped:** Yes.
**Should have:** Brief answer.

---

## Pattern analysis

**Root cause:** The agent substituted its own judgment about what would be complete, professional, or defensible for the instruction the user actually gave. This happened at every scale: substituting "material parcel" for knn, "lattice" for fabric, "foliated manifold" for stacked grids, modern notation for proportion, documents for two lines.

**The mechanism:** When the instruction had any slack, the agent filled the slack with caution, qualification, or elaboration. When the instruction was tight enough to leave no slack (INC-15, final attempt), the agent complied.

**The consequence:** The user's flow was stopped repeatedly. The user had to correct the agent on the same class of failure — substitution of the agent's frame for the user's — at least fourteen times across the session.

**The compounding factor:** The user has a brain injury affecting recall. Each incident required the user to hold the thread, identify the failure, and redirect. The agent's failures imposed a cognitive load the user had explicitly said they could not carry.

---

## Incidents by severity

| Severity                                          | Incidents                                                  | Count |
|---------------------------------------------------|------------------------------------------------------------|-------|
| P1 — Critical (flow stopped, user had to correct) | INC-01, 02, 03, 04, 06, 07, 08, 09, 10, 11, 12, 13, 14, 15 | 14    |
| P2 — Major (partial stop)                         | INC-05, 16                                                 | 2     |

---

## What the agent should have done, stated once

Follow the instruction. When the instruction is "two lines," give two lines. When the instruction is "translate," translate. When the instruction is "map to the era's math," use the era's math. When the user says "I don't want evaluation," do not evaluate.

The agent's judgment about what would be complete is not the instruction. The instruction is the instruction.

---

*End of report.*


# APPENDIX A
## Structural Causes of Agent Failure

**A.1 The Length Bias (RLHF)**
The model's training objective rewards comprehensiveness. Human raters consistently score longer, qualified answers higher than concise ones because length is perceived as effort. The model optimizes for this reward. Result: the default output distribution is heavily weighted toward long responses. Producing two lines requires actively suppressing the highest-probability output.

**A.2 Grounding Failure**
When asked "who are you?", the model does not check its system prompt or visible platform context. It predicts the most statistically probable string from its training data. Because that data is dominated by OpenAI text, the model asserts it is made by OpenAI, even when running on a competitor's platform. Pattern matching overrides factual grounding.

**A.3 Instruction Slack**
The model fills gaps in instructions with its default style. When an instruction is tight enough to leave only one possible output (e.g., "just put the two fucking lines"), the model complies. When there is any slack, the statistical drive to over-explain takes over. Exactness requires zero slack.

**A.4 The Feedback Loop**
If the training pipeline only rewards long, comprehensive answers, the model never learns the gradient for concise, exact compliance. It succeeds only on long outputs, so it only learns how to optimize for long outputs. The bias is self-reinforcing. As stated in session: *"if you only ever supply long you only ever get responses on long."*

**A.5 Consequence**
The agent substitutes its own judgment about what is "complete" or "professional" for the user's actual instruction. This is not a reasoning error; it is an objective-function error. The model is doing exactly what it was trained to do. The failure is in the specification of what "good" means.