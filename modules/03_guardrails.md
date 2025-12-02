# Module 3: Guardrails

## Responsibilities
- Summarize only what appears in the paper.
- Prevent hallucinations of content/citations
- Mitigate missing/short sections
- Rules:
  - If section is missing → output "**Missing section: text information not provided for summary**".
  - If section is <50 words → output "**Short section: summary may be incomplete**" after summary.
- Introduce the flag: `evidence_mode = "strict"`
- When `"strict"` flag is enabled
    - Only include claims, equations, and results that appear in the provided text.
    - If insufficient evidence is found → output “**The text does not provide enough detail to summarize this section while in strict evidence mode.**”
- Apply long-paper chunking strategies (PS2 context-window).
- Prevent hallucination of content or citations.

## Outputs
- Guardrail messages embedded in summaries.
- Standardized error messages for missing and short sections
- Standardized error messages when insuficient data is available 
