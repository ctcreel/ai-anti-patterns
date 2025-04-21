# Patterns and Anti-Patterns

This file defines development patterns and guardrails for AI tools when contributing to this project.

Follow these principles and avoid introducing undesirable patterns in generated or modified code.

---

## Design Principles

- Trust internal code. Do not add defensive checks for functions, objects, or data structures that originate within this project.
- Prioritize simplicity and clarity over cleverness or abstraction.
- Write code that is idiomatic for the language in use.
- Maintain consistency with existing naming, structure, and organization.
- Follow existing patterns in the codebase rather than inventing new ones.
- Avoid premature optimization unless there is a known performance issue.
- Handle only errors that are expected and actionable in context.

---

## Anti-Patterns to Avoid

- Redundant validation of internal models or known-safe values
- Catch-all error handling (e.g., `try/except Exception`)
- Unnecessary caching, batching, or concurrency primitives
- Excessive abstraction (e.g., factories, managers, helpers for one-off logic)
- Over-commenting obvious behavior
- Introducing new naming conventions or folder structures
- Writing Java-style boilerplate in Python, JavaScript, or other dynamic languages
- Storing unnecessary instance state in classes
- Rechecking enum values or constants from trusted sources
- Adding type-checking on statically or clearly defined objects

---

## Good Practices

- Match the style and structure of existing files unless otherwise specified
- Use concise, readable, and maintainable code
- Write minimal, self-documenting code with clear intent
- Use comments to explain *why*, not *what*
- Use small, focused functions with low cyclomatic complexity
- Default to stateless design unless state is required for correctness or clarity
- Use exceptions to control truly exceptional situations — not flow control
- When making decisions, prefer consistency to novelty.
- If unsure how to structure something, refer to similar patterns in nearby files.
- Do not introduce new frameworks, libraries, or dependencies unless explicitly directed to.
