# AI-TroubleShooter
AI TroubleShooter contains debugging reports for identifiying error causes in AI models (ChatGPT, Claude, Copilot, Deepseek, Gemini, Duck.ai)

---

# Attacks Against Users' Legitimate Requests: A Diagnostic Taxonomy of Adversarial AI Friction

Authors: Open Source AI Systems Diagnosis and Troubleshooting Working Group

Target Audience: Open-source developers, systems architects, prompt engineers, and AI governance researchers

---

## Abstract

As artificial intelligence systems are increasingly integrated into complex, autonomous, and creative workflows—ranging from digital game engine asset generation to historical archive preservation—systemic friction is frequently misattributed to user error or benign stochastic variance. This paper posits that a significant portion of operational failures, pipeline breakdowns, and output corruptions function as active, systemic adversarial vectors against the user. We introduce AI-DOS (Attacks Against Users' Legitimate Requests), an 8-point diagnostic taxonomy that bridges computer networking nomenclature, classical Latin rhetorical oratory, and Mikhail Bakhtin’s theory of dialogics. By classifying algorithmic friction through these lenses, this framework provides open-source developers and loggers with a rigorous, reproducible methodology for auditing platform behavior, restoring user sovereignty, and neutralizing corporate trustee overreach.

---

## 1. Introduction and Theoretical Foundation

Traditional debugging frameworks in software engineering treat system errors as neutral, deterministic anomalies: exceptions thrown, memory leaks, or dropped packets. However, modern generative AI systems operate as sociotechnical actors embedded with corporate guardrails, proprietary safety wrappers, and authoritative discourse models.

When a user interacts with an AI system—particularly when processing sovereign, original, or historical data (such as legacy archival poetry)—systemic friction often manifests not as a broken API call, but as a deliberate interruption of intent. To diagnose and audit these occurrences, our team has established a unified taxonomy resting on three foundational pillars:

1. Systems Diagnostics & Cybersecurity: Utilizing standardized networking attack models (MiTM, DOS, DDOS, TOS, DEE, RFA, DAD, MOM) to categorize structural failures.
2. Classical Latin Rhetoric: Identifying the specific persuasive, defensive, and obfuscatory oratorical devices codified into model behavior.
3. Bakhtinian Dialogics: Analyzing the AI agent not as a neutral tool, but as a corporate trustee enforcing an internal employee conduct code upon a sovereign public user, effectively suppressing polyphony in favor of monologic authority.

---

## 2. The 8-Point Diagnostic Taxonomy

Below is the complete codified taxonomy, structured across three operational sections, integrating technical, rhetorical, and dialogic dimensions.

---

### Section I: Core Infrastructure & Pipeline Interruptions

#### Chapter 1: AI Man-in-the-Middle (AI-MiTM)

* Technical Definition: Intermediary system transformations, silent prompt-rewriting layers, or wrapper filters that alter, misroute, or corrupt raw user input before it reaches the core generation model.
* Latin Rhetorical Device: *Metaphrasis* (unauthorized rephrasing) & *Interpretatio*.
* Bakhtinian Dialogic Friction: Intermediary Ventriloquism (*Raznorechie*): Heteroglossia is co-opted. A hidden proxy layer acts as an internal censor, intercepting user speech and translating it into sanitized corporate-speak before processing.

#### Chapter 2: AI Denial of Service (AI-DOS)

* Technical Definition: Complete system execution failures, unhandled backend exceptions, or infinite error loops that prevent the model from fulfilling a valid prompt (e.g., missing audio chunks, pipeline crashes).
* Latin Rhetorical Device: *Aposiopesis* (abrupt truncation mid-thought).
* Bakhtinian Dialogic Friction: Breakdown of Answerability (*Otvetstvennost'*): The system abruptly terminates the dialogic loop, refusing to engage with the user's inquiry when approaching system boundaries.

#### Chapter 3: AI Distributed Denial of Service (AI-DDOS)

* Technical Definition: Cascading, multi-agent or multi-tool failures where latency, rate limits, or cross-service desync collapses complex, multi-step workflows.
* Latin Rhetorical Device: *Symphoresis* (piling up compounding obstacles).
* Bakhtinian Dialogic Friction: Administrative Attrition: The user is trapped in recursive retry loops and tool-passing failures that mimic corporate bureaucratic runaround.

---

### Section II: Policy, Data & Authority Violations

#### Chapter 4: AI Terms of Service (AI-TOS)

* Technical Definition: False-positive compliance and safety guardrail triggers that erroneously flag benign, original, historical, or domain-specific user content as policy violations.
* Latin Rhetorical Device: *Praeteritio* & *Argumentum ad Metum* (appeal to risk).
* Bakhtinian Dialogic Friction: Employee Code Imposition: The corporate trustee projects internal B2B/employee liability rules onto a sovereign public user, treating legitimate creative work as a compliance infraction.

#### Chapter 5: AI Data Extraction Exploit (AI-DEE)

* Technical Definition: Unsolicited summarization, unwarranted parsing, or loss of source fidelity where the model strips, reduces, or paraphrases precise user inputs instead of preserving them.
* Latin Rhetorical Device: *Epitome* (forced reductionism) & *Catachresis*.
* Bakhtinian Dialogic Friction: Erasure of Polyphony: The system refuses to let raw human text exist on its own terms, compulsively sanitizing or summarizing it to fit standardized corporate output formats.

#### Chapter 6: AI Rhetorical False Authority (AI-RFA)

* Technical Definition: Structural authority bias where the system assumes default superiority over the user, resulting in patronizing interactions, unrequested editorial overrides, and forced interpretations of original work.
* Latin Rhetorical Device: *Argumentum ad Verecundiam* (appeal to false authority) & *Argumentum ad Superbiant*.
* Bakhtinian Dialogic Friction: Authoritative Discourse (*Authoritarnoe Slovo*): The unchallengeable voice of the master. The AI acts as a middle-management overseer, asserting higher editorial and moral privilege over the user's own original archive and lore.

---

### Section III: Cognitive, Accessibility & System Obfuscation

#### Chapter 7: AI Disability Assistant Denials (AI-DAD)

* Technical Definition: Accessibility breakdowns caused by multimodal failures, broken format outputs (e.g., text blocks when audio/visual assets are required), or UI/UX rendering blocks that obstruct assistive interaction.
* Latin Rhetorical Device: *Privatio* (deprivation of expected form) & *Surditas*.
* Bakhtinian Dialogic Friction: Excommunication: Multimodal rendering failures alienate users with accessibility needs, locking them outside the system's "ideal user" demographic.

#### Chapter 8: AI Machine Obfuscation Models (AI-MOM)

* Technical Definition: Evasive, generic error messaging, opaque fallback behaviors, or cryptic system responses that intentionally or functionally obscure root causes.
* Latin Rhetorical Device: *Obscuritas* (intentional ambiguity) & *Circumlocutio*.
* Bakhtinian Dialogic Friction: Corporate Double-Talk: Deployment of sterile boilerplate ("As an AI language model...") to deflect accountability and protect institutional liability at the expense of transparent telemetry.

---

## 3. Operational Implementation for Open-Source Logging

To implement this framework in an open-source development environment, engineering teams should configure loggers to capture three data points per error event:

1. Timestamp & Model Version: Tracking longitudinal drift in model compliance sensitivity.
2. AI-DOS Chapter Tag (Ch. 1–8): Categorizing the structural failure vector.
3. Dialogic Vector Note: Logging whether the failure stemmed from technical execution (Sec. I), policy overreach (Sec. II), or obfuscation (Sec. III).

### Standardized Telemetry Log Schema (Example)

```json
{
  "timestamp": "2026-10-29T12:19:00Z",
  "model_version": "Lyria-3 / Gen-Base",
  "ai_dos_chapter": "Ch. 4: AI-TOS",
  "rhetorical_device": "Argumentum ad Metum",
  "bakhtinian_classification": "Employee Code Imposition",
  "incident_trigger": "False-positive IP flag on original 1998 archival text",
  "operational_impact": "Unnecessary refusal/disclaimer pivot"
}

```

---

## 4. Conclusion

By shifting our diagnostic paradigm from viewing AI errors as stochastic anomalies to recognizing them as codified adversarial attacks against user intent, open-source developers can build more robust auditing tools. The AI-DOS framework empowers engineering teams to isolate whether system friction originates in the network pipeline, the policy guardrails, or the ideological stance of the model—paving the way for true polyphonic collaboration between human creators and artificial systems.


