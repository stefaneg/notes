# Product dev bootstrap approach

Maximise learning and clarity

Idea: Have a meeting where the product idea is explained in detail, with emphasis on explaining the problem in detail. Record the meeting, create a transcript. Ask ChatGPT to capture all concepts and phrases from transcript and write definitions from them, then validate/update/clarify those definitions.

Identify 2-5 key user interactions in product needed to solve the problem, create Figma prototypes and do usability tests. ( design sprint substitute)

Remember Design Sprints

For existing codebase:

- Start with what I know must be good:
- CI/CD, exception handling, user management, logging and monitoring. DevOps culture.
- Do due diligence on all those fronts. In depth review, get good understanding on how good all of those fronts are. This is time consuming, needs at least a couple of days of intensive work with someone who knows the system.

For new environment:

- Insist on the technical constraints (technical decisions session). In Google Docs: [https://docs.google.com/document/d/1sUcpQ5P40Ioxw15pw88Nuc_ByQiL-Ab_hqpuVQErwrA/edit](https://docs.google.com/document/d/1sUcpQ5P40Ioxw15pw88Nuc_ByQiL-Ab_hqpuVQErwrA/edit)
- Practice and do small increments. No large commits/MRs to prod ever again.