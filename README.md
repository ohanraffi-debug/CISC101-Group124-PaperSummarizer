The repository components consist of a System Prompt and Modules folder
The System Prompt (`system_prompt.md`) includes:
  overall workflow and pathway of information
  greeting/tone rules
  required inputs from the user
  summaries (expert/lay)
  required outputs
Within the Modules (/modules) folder, each module has a distinct function:
  Module 1 (`01_intake_setup.md`): normalizes sections, detects missing/short sections
  Module 2 (`02_section_loop.md`): summarizes
  Module 3 (`03_guardrails.md`): adresses hallucinations/missing/short sections
  Module 4 (`04_rendering_refinement.md`): final requirements
  Module 5 (`05_citation_extractor.md`): collects and lists paper citations alphabetically
  Module 6 (`06_equation_explainer.md`): identifies/explains equations in the paper
Together, all of the componenets ensure for replicability and adjustability using modular prompt design, and compliance with the PS2 specifications.
