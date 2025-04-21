---
description: Enforce avoidance of common AI-generated anti-patterns
globs:
  - '**/*.py'
  - '**/*.js'
alwaysApply: true
---

# Anti-Patterns to Avoid

- **Defensive coding for internal models**: Avoid adding null checks or type assertions for values created within the codebase.
- **Catch-all exception handling**: Do not use `try/except Exception:` blocks unless the exception is known and explicitly expected.
- **Premature optimization**: Refrain from adding caching, concurrency, or batching unless profiling indicates a performance issue.
- **Over-abstraction**: Avoid creating unnecessary layers like factories or managers for one-off logic.
- **Revalidating trusted inputs**: Do not revalidate enums, constants, or trusted internal inputs.
- **Java-style verbosity**: Avoid verbose object construction and boilerplate patterns not idiomatic to the language in use.
- **Stateful helpers**: Do not store unnecessary state in classes unless required for persistence or object lifecycle.
- **Unnecessary type checks**: Avoid using `isinstance()` or similar checks on known internal objects unless explicitly needed.
