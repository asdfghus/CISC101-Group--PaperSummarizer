# Module 3: Guardrails


 ## Change Log
- Added `evidence_mode` variable with option `"strict"`.
- Implemented strict evidence behavior: only include claims, equations, and results from source text.
- Added standardized warning messages for missing/empty or too-short sections.

---
- Flag missing/empty sections
- Flag <50-word sections
- Mitigate hallucinations
- Apply long-paper chunking strategies
---
## Logic

### Evidence Mode
- Variable: `evidence_mode`
- If `evidence_mode = "strict"`:
  - Summarizer must only include claims, equations, and results explicitly present in the source text.
  - If insufficient information is found:
    - Output: “The source text does not provide enough detail to summarize this section in strict evidence mode.”

### Section Warnings
- If section is missing or empty:
  - Output: “Section skipped: no usable text was provided.”
- If section length < 50 words:
  - Output: “Section very short: summary may be incomplete.”

### General Guardrails
- Always flag hallucinations or unsupported claims.
- Ensure summaries remain objective and grounded in the provided text.

