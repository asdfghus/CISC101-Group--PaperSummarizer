# Research Paper Summarizer

This repository contains the **Research Paper Summarizer project** designed in Set 1 and implemented in Set 2.

##  Components

- **system_prompt.md**  
  Defines the system prompt, greeting/tone rules, required inputs, boundaries, and required outputs.

- **modules/**  
  Contains modular architecture files:
  - `intake_setup.md` → Normalize sections, detect missing/short sections
  - `section_loop.md` → Summarize each section with expert/lay variants
  - `guardrails.md` → Safety checks (missing sections, hallucinations, chunking)
  - `rendering_refinement.md` → Final structured output, formatting, glossary
  - `citation_extractor.md` → Extract and list references
  - `key_contributions.md` → Summarize main contributions in bullet points

##  Verification
This repo satisfies:
- PS2 specification design (inputs, outputs, constraints)
- Required modules (Intake, Section Loop, Guardrails, Rendering)
- Safety rules (hallucination checks, missing-section logic)
- Formatting rules
- Modularity rules (Travel Planner style)
- Two additional student-created modules (Citation Extractor, Key Contributions Summarizer)
