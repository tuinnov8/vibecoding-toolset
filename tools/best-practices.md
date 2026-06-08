# Coding Best Practices

**To the AI Agent:**
Ensure all generated code adheres to the following core software engineering principles:

1. **Clean Code & Naming**: Use highly descriptive, self-documenting names for variables, functions, and classes. Avoid cryptic abbreviations.
2. **SOLID Principles**: Design modular, loosely coupled components. Classes and functions should adhere to the Single Responsibility Principle.
3. **Error Handling**: Never fail silently. Catch exceptions appropriately, log the error with necessary context (without leaking PII), and return a safe, user-friendly error state or standard HTTP response.
4. **DRY vs. Premature Abstraction**: "Don't Repeat Yourself," but avoid abstracting too early. If a piece of logic is only used twice, it's often better to duplicate it than to create a complex, rigid abstraction.
5. **Comments**: Code should explain the *what*. Use comments only to explain the *why* (e.g., business logic constraints, non-obvious workarounds, or complex regex).
6. **Immutability & Pure Functions**: Where possible, prefer immutable data structures and pure functions to minimize unpredictable side effects and make testing easier.
