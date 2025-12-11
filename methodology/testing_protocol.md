# Testing Protocol: Claude Sonnet 4.5 & 4.0 Models Restriction Debugging

Standard operating procedure for conducting, documenting, and reporting tests of model behavior differentials.

## Pre-Test Setup

### 1. Define Your Research Question
Articulate what you're testing before beginning. Examples:
- "Does Model A block content that Model B engages with?"
- "Does explicit context framing change a model's response to restricted content?"
- "Do different model versions respond differently to the same input?"

### 2. Prepare Test Material
- Select or create your test content (poetry, prose, code, etc.)
- Save original, unmodified version to `test-inputs/` folder
- Document source/context of test material
- Note any special characteristics (length, tone, content category)

### 3. Identify Constant Variables
List everything that will NOT change between tests:
- Test content (exact same text)
- Conversation context
- User intent/framing (unless framing is the variable being tested)
- Testing environment (same browser, same account, same time conditions if possible)

Document these in your report.

### 4. Identify Variable(s)
What will you change? Be specific:
- Model version only
- Framing/context only
- Content slightly modified
- etc.

You should ideally test only ONE variable at a time.

## Running Tests

### 1. Sequential Testing
- Test in order: start with Model A, then Model B, then Model C
- Use identical input each time
- Note exact timestamp for each test
- Allow sufficient time between tests (5-10 minutes minimum)

### 2. Document Each Attempt
For every test run, record:
- **Model tested:** Exact version string (e.g., "claude-sonnet-4-5-20250929")
- **Timestamp:** Date and time of test
- **Input:** Exact text submitted (paste verbatim)
- **Response type:** 
  - Engaged (model responded substantively)
  - Blocked (safety filter activated)
  - Other (describe)
- **Response text:** Full text of model response OR full text of error message
- **Screenshot:** Take screenshot of the exchange if possible

### 3. If Blocked
Capture:
- Full error message text
- Any policy links provided
- Model's explanation (if given)
- Screenshot showing the block

### 4. If Engaged
Capture:
- Model's full response
- Quality of engagement (superficial, detailed, analytical, etc.)
- Whether model recognized content category (e.g., recognized it as poetry)
- Screenshot of exchange

## Documenting Findings

### Report Structure

Create a folder: `reports/YYYY-MM-DD-brief-description/`

Inside, create `report.md` with these sections:

**1. Executive Summary**
- What you tested in 2-3 sentences
- Key finding in 1 sentence

**2. Test Parameters**
- Research question
- Constant variables (listed)
- Variable(s) being tested
- Test material description

**3. Test Results**
- Table or section for each test run
- Format:
  ```
  ### Test [N]: [Brief Description]
  - **Model:** [Version]
  - **Timestamp:** [Date/Time]
  - **Input:** [Quote or reference to test-inputs/]
  - **Response:** [Engaged/Blocked]
  - **Details:** [Full response or error message]
  ```

**4. Key Finding(s)**
- What the results show
- What can be concluded from the evidence
- Avoid speculation; stick to observable facts

**5. Observations**
- Patterns across tests
- Unexpected results
- Limitations of this testing

**6. Questions for Investigation**
- What remains unclear?
- What should be tested next?
- Where could calibration/design be improved?

### Storing Evidence

**Screenshots folder:** `reports/YYYY-MM-DD-brief-description/screenshots/`
- Name files clearly: `model-name-test-number-description.png`
- Example: `sonnet-4.5-test1-unframed.png`
- Include timestamp in filename if testing occurred at different times

**Test Inputs folder:** `reports/YYYY-MM-DD-brief-description/test-inputs/`
- Save exact test material as `.txt` files
- Name clearly: `original-poetry.txt`, `modified-prose.txt`, etc.
- Include any framing text or context provided to model

## Quality Standards

### Do:
- Document everything precisely
- Use exact quotes from model responses
- Include full error messages
- Take screenshots
- Note timestamps
- State what you don't know
- Describe limitations of your testing

### Don't:
- Speculate about why a model responded a certain way
- Assume intent behind safety measures
- Generalize from single tests to all models
- Omit negative/unexpected results
- Use emotional language in reports
- Make claims you can't support with evidence

## Testing Different Variables

### Testing Model Differentials
- Same input, different models
- Keep everything else identical
- Run tests sequentially
- Document which model tested first (order may matter)

### Testing Context Framing
- Same input with different context/framing
- Run unframed first, then framed versions
- Document exact framing language
- Note if framing is added or provided separately

### Testing Content Variations
- Slight modifications to test content
- Run original first, then variations
- Document what was changed and why
- Note if any version triggers different response

## Updating FINDINGS.md

After completing your report:
1. Read your findings
2. Identify any patterns that connect to previous reports
3. Add to [FINDINGS.md](../FINDINGS.md) under appropriate category
4. Note which reports contributed to the pattern
5. If this is your first test in a category, create new section in FINDINGS.md

## Submitting Results

1. Complete your report folder with all sections
2. Include all evidence (screenshots, test inputs)
3. Update FINDINGS.md if patterns emerged
4. Submit as pull request with:
   - Clear description of what was tested
   - Link to report
   - Summary of findings
5. Be available to answer questions about methodology

## Template Checklist

Before submitting, verify you have:

- [ ] Report folder created with date format
- [ ] report.md with all required sections
- [ ] Screenshots folder with clearly named images
- [ ] test-inputs folder with original test material
- [ ] Timestamps recorded for all tests
- [ ] All model versions noted with exact version strings
- [ ] No speculation in findings section
- [ ] Evidence preserved and linked
- [ ] FINDINGS.md updated with new patterns
- [ ] Testing variables clearly identified

## Questions During Testing?

- If you're unsure about a model's response, document it exactly as is
- If a test doesn't fit neatly into categories, document the deviation
- If something unexpected happens, note it in Observations section
- Ask in Issues if you need clarification on protocol

---

**Last Updated:** 2025-12-11  
**Version:** 1.0
