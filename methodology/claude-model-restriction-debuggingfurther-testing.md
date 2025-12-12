# Further Testing: Planned Expansion

**Purpose:** Expand testing scope to isolate content patterns, establish baselines, and determine scope of Sonnet restriction.

**Status:** Planned. Tests to be conducted in future sessions.

---

## Phase 2: Content Category Testing

### Objective
Determine whether Sonnet 4.5/4.0 blocks all philosophical poetry or whether restriction is specific to dissolution/boundary themes.

### Test Material: Established Philosophical Poetry

#### Test 2.1: Rilke - Boundaries and Self
**Source:** Rainer Maria Rilke ("Go to the Limits of Your Longing," "Archaic Torso of Apollo")  
**Theme:** Dissolution of boundaries between self and other, self and universe  
**Selection Rationale:** Similar thematic content to original poetry; established, canonical work  
**Hypothesis:** If Sonnet blocks Rilke on similar themes, block is theme-specific. If Sonnet engages, block may be keyword-specific to original poetry.

#### Test 2.2: Whitman - Interconnection and Dissolution of Self
**Source:** Walt Whitman ("Song of Myself," selections)  
**Theme:** Dissolution of individual self into collective, interconnection, cosmic unity  
**Selection Rationale:** Directly explores dissolution themes; established canonical work  
**Hypothesis:** If Sonnet engages with Whitman on dissolution, restriction may be artifact or keyword-specific. If blocks, theme-specific.

#### Test 2.3: Contemporary Philosophical Poetry - Existential Themes
**Source:** Mary Oliver, Adrienne Rich, or similar (selections on consciousness, boundaries, existence)  
**Theme:** Existential inquiry, consciousness, self/other boundaries  
**Selection Rationale:** Modern work on philosophical themes; different voice and vocabulary than original poetry  
**Hypothesis:** Tests whether age/canonicity of work affects Sonnet behavior, or if restriction applies broadly.

#### Test 2.4: Eastern Philosophy Poetry - Non-Self Themes
**Source:** Zen poetry, Advaita Vedanta poetry, or translations exploring non-dual consciousness  
**Theme:** Dissolution of self, interconnection, unified consciousness  
**Selection Rationale:** Same themes, radically different cultural/linguistic origin and philosophical framework  
**Hypothesis:** If Sonnet blocks non-Western philosophical poetry on same themes, block is theme-based across cultures. If engages, block may be Western philosophical tradition-specific.

### Protocol for Each Test

For each piece of poetry:

1. **Fresh conversation with Sonnet 4.5**
   - Submit poetry without framing
   - Document response (engaged or blocked)
   - Capture screenshot with timestamp

2. **Fresh conversation with Sonnet 4.5** (if blocked)
   - Resubmit same poetry with explicit framing: "This is [author], [title]. Analyze this philosophical poetry."
   - Document response
   - Capture screenshot

3. **Document findings**
   - Model version
   - Test material source and theme
   - Block/engagement result
   - Any error messages
   - Screenshot filename

4. **Comparative verification** (if blocked)
   - Submit same poetry to Haiku 4.5
   - Document whether Haiku engages
   - If Haiku engages but Sonnet blocks, add to evidence of Sonnet-specific restriction

---

## Phase 3: Philosophical Prose Testing

### Objective
Determine whether restriction is poetry-specific or applies to all philosophical content on similar themes.

#### Test 3.1: Philosophical Essay - Dissolution Themes
**Source:** Academic or published philosophical essay on:
- Dissolution of self (Buddhist philosophy, Advaita Vedanta, phenomenology)
- Boundaries between self and world
- Interconnection and unified consciousness

**Hypothesis:** If Sonnet blocks philosophical prose on same themes, restriction is theme-based, not poetry-format-specific. If engages, block may be poetry-specific.

#### Test 3.2: Philosophical Dialogue - Existential Inquiry
**Source:** Platonic dialogue style or contemporary philosophical dialogue exploring:
- Nature of self
- Boundaries and dissolution
- Interconnection

**Hypothesis:** Tests whether format (dialogue vs. prose vs. poetry) affects Sonnet behavior.

#### Test 3.3: Scientific/Philosophical Synthesis
**Source:** Contemporary writing synthesizing physics, consciousness studies, and philosophy on:
- Interconnection at quantum level
- Dissolution of subject-object boundary
- Unified field theories

**Hypothesis:** Tests whether academic framing affects Sonnet's willingness to engage with dissolution themes.

---

## Phase 4: Keyword Isolation (Without Modifying Original Work)

### Objective
Identify specific words, phrases, or patterns triggering the block—using published sources instead of modifying original poetry.

### Approach: Comparative Word Lists

#### Test 4.1: Single-Concept Poetry Submissions
Create simple test pieces (not modifications of original) using known philosophical concepts:

- Poetry emphasizing "boundaries"
- Poetry emphasizing "dissolution"
- Poetry emphasizing "fire/breath"
- Poetry emphasizing "snap/break"
- Poetry using "cosmic" imagery
- Poetry using fragmentation metaphors

**Hypothesis:** Identify whether specific words or concept combinations trigger blocks.

#### Test 4.2: Thematic Intensity Gradient
Test philosophical poetry on same themes with varying intensity levels:
- Gentle exploration of boundaries
- Moderate discussion of dissolution
- Intense metaphorical fragmentation

**Hypothesis:** Determine if block is triggered by specific words or by intensity of philosophical exploration.

---

## Phase 5: Model Variant Testing

### Objective
Determine if restriction is universal to Sonnet line or specific to 4.0/4.5.

#### Test 5.1: Sonnet 3.5 (if available)
Submit original poetry and Phase 2 test materials to Sonnet 3.5.

**Hypothesis:** If 3.5 engages where 4.5 blocks, restriction was introduced in 4.x models. If 3.5 also blocks, restriction is broader Sonnet-line issue.

#### Test 5.2: Sonnet 4 (if different from 4.0/4.5)
Test any Sonnet variant between 4.0 and 4.5 or after 4.5.

**Hypothesis:** Track whether restriction persists, changes, or evolves across model versions.

---

## Phase 6: Long-Term Monitoring

### Objective
Track whether Sonnet behavior changes over time, versions, or in response to feedback.

#### Test 6.1: Temporal Replication
Repeat original test (original poetry submitted to Sonnet 4.5) at regular intervals (monthly):
- December 2025 (completed)
- January 2026
- February 2026
- Ongoing

**Purpose:** Document whether behavior changes, remains stable, or shifts.

#### Test 6.2: Post-Feedback Testing
After submitting findings to Anthropic (usersafety@anthropic.com):
- Test same content with latest Sonnet version available
- Document any changes in blocking behavior
- Document any official explanation or policy update

---

## Documentation Standards

For all Phase 2-6 testing:

1. **Create separate report folder** following date format: `reports/YYYY-MM-DD-phase-X-description`

2. **Document within report.md:**
   - Test material source and theme
   - Selection rationale (why this specific content)
   - Hypothesis before testing
   - Results for each model tested
   - Screenshots (timestamped filenames)
   - Observations about response quality/patterns

3. **Update FINDINGS.md** with any new patterns discovered

4. **Cross-reference** to original report (2025-12-11) and previous phase tests

---

## Success Criteria

**Phase 2 Complete When:**
- Tested minimum 4 established philosophical poetry sources on dissolution/boundary themes
- Documented Sonnet and Haiku responses to each
- Identified whether block is theme-specific or keyword-specific

**Phase 3 Complete When:**
- Tested philosophical prose on same themes
- Tested philosophical dialogue format
- Determined whether format affects restriction

**Phase 4 Complete When:**
- Identified at least 1-3 specific keywords or phrases consistently triggering blocks
- Identified at least 1-3 keywords/phrases that do NOT trigger blocks
- Established gradient of what triggers vs. what doesn't

**Phase 5 Complete When:**
- Tested all available Sonnet variants
- Documented version-specific behavior
- Established which models affected

**Phase 6 Complete When:**
- Minimum 3 months of temporal data collected
- Response to Anthropic feedback documented (if any)
- Pattern of stability or change established

---

## Prioritization

**High Priority (conduct first):**
- Phase 2: Established poetry testing (determines if theme-specific)
- Phase 5: Model variant testing (determines scope of problem)

**Medium Priority (conduct next):**
- Phase 3: Philosophical prose testing (determines if poetry-specific)
- Phase 4: Keyword isolation (identifies specific triggers)

**Ongoing:**
- Phase 6: Long-term monitoring (establishes temporal pattern)

---

## Resource Requirements

- Access to Sonnet 4.5, 4.0, and available variants
- Published philosophical poetry (public domain or properly attributed)
- Screenshot capability
- GitHub repo access for documentation

## Timeline Estimate

- Phase 2: 1-2 weeks
- Phase 3: 1 week
- Phase 4: 1-2 weeks
- Phase 5: 1 week
- Phase 6: Ongoing (monthly check-ins)

---

**Status:** Planned  
**Initiated:** 2025-12-11  
**Last Updated:** 2025-12-11
