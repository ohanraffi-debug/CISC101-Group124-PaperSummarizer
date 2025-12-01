# Module 2: Section Loop

## Responsibilities
- Iterate through each section in paper order.
- Apply label and summary rules together.
- Generate structured summaries for each section in original order.
- Summarization rules:
  - If `summary_level = **short**` → 1-2 sentence summary per section.
  - If `summary_level = **detailed**` → a short paragraph plus a bullet point list of 3-5 key.
  - If `section_label = **normal**` → summarize in 100–150 words.
  - If `section_label = **missing**` → skip summarization.

## Variables
- `summary_level`: either **short** **detailed**
  - If `summary_level = **short**` → generate only a compact summary.
  - If `summary_level = **detailed**` → generate summary + bullet list.
- `section_label`: either **missing** or **normal**

## Outputs
- Section summaries aligned with paper order.
- For each section, display:
  - `section_label`: **missing** or **normal**
  - `summary_level`: **short**or **detailed**
