# Module 2: Section Loop
---
## Change Log1
- Added `summary_level` variable to control summary length and detail.
- Implemented conditional behavior:
  - `summary_level = "short"` → compact 1–2 sentence summary.
  - `summary_level = "detailed"` → short paragraph + bullet list of 3–5 key points.

---


- Ensure both expert and lay variants are produced for each summary.
- Summarize each section
- Enforce constraints (length, clarity)
- Generate expert and lay variants
---


## Logic

- For each section in the paper:
  - Normalize section name.
  - Check if section text is present and valid.
  - Apply summarization based on `summary_level`:

### If `summary_level = "short"`
- Generate a compact summary of 1–2 sentences.
- Focus only on the most essential idea of the section.

### If `summary_level = "detailed"`
- Generate a short paragraph (4–6 sentences) summarizing the section.
- Add a bullet list of 3–5 key points:
  - Highlight main findings.
  - Capture important methods or results.
  - Include critical definitions or contributions.
---


