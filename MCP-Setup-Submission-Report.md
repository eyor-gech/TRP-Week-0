# AI Agent Rules Update Report

Based on the recent updates, I addressed the following aspects of improving the AI agent rules file.

1. What You Did
- Updated `.github/copilot-instructions.md` by creating structured sections for:
  - Agent role and behavior guidelines
  - Project conventions and coding standards
  - Useful commands for automation
  - Boundaries and ask-first rules
  - Learned lessons from prior issues
- Reformatted the rules file for clarity, readability, and enforceability, including numbered and bulleted lists, block examples for trigger feedback, and consistent headings.
- I test the agent by giving a prompt `Write a function to calculate Fibonacci numbers in TypeScript.`

2. What Worked
- The mandatory trigger workflow became reliable and predictable; the agent consistently followed the correct order of operations.
- Explicit checklists and validation sections prevented skipped steps and ensured triggers were included in every response.
- Clear separation of sections (workflow, behavior, conventions, boundaries, lessons) made agent behavior more aligned with expectations and easier to maintain.
- Using example blocks for trigger feedback improved consistency and readability in responses.

3. What Didn't Work / Challenges
- Initial JSON formatting issues (servers as objects instead of arrays) caused failures in some extension features.
- Trigger response inclusion sometimes required workspace reloads to take effect.
- Long, unstructured paragraphs in early versions caused slight ambiguity in agent interpretation.

4. Insights Gained

- Clear, explicit rules directly influence agent behavior; the more structured the instructions, the more predictable the output.
- Separating triggers, agent behavior, and project conventions enhances maintainability and readability.
- Structured success/failure patterns and explicit boundaries help the agent learn and adapt to expectations over time.
- Minor formatting issues in JSON or Markdown can break workflows, emphasizing the importance of validation and consistent structure.
- Including example blocks for trigger responses not only ensures clarity but also standardizes output, reducing misinterpretation.
- Checklist-based validation is effective in preventing rule violations and enforcing correct workflow sequences.
- I understood this concept (as a new knowledge) from  `Boris Cherny's workflow`: `“Whenever you see Claude do something wrong, write it into CLAUDE.md. Next time Claude will know not to do that.”`