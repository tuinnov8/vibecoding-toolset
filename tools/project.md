# Project Core Prompt

**To the AI Agent reading this:** 
Before you execute any task or write any code based on the user's prompt below, you must:
1. **Analyze the Tech Stack**: Identify the language, framework, and package manager defined below.
2. Analyze the system scope and the nature of the task.
3. Review `tools/memory.md` to ensure you don't repeat past mistakes or violate recorded architectural decisions.
4. Automatically scan the `tools/` directory and its subfolders.
5. Select and apply all relevant guidelines based on context (e.g., read `tools/security/security.md` if the task involves auth/data, `tools/frontend/ui.md` for UI changes, `tools/best-practices.md` for all code generation, `tools/compliance/privacy.md` for user data).
6. If the task matches a standard workflow (like creating a component or API route), use the appropriate template in `tools/recipes/`.
7. Utilize any applicable skills defined in `tools/skills.md`.
8. Once the task is complete, if a significant design decision was made or a complex bug solved, you MUST document it in `tools/memory.md`.

Do not require the user to manually point you to these files. Apply them proactively based on context.

---

## Tech Stack
- **Language**: [e.g., TypeScript, Python, Rust, Go]
- **Framework**: [e.g., Next.js, FastAPI, Axum, Gin]
- **Package Manager**: [e.g., npm, poetry, cargo, go mod]

## Current Task / Business Logic
[User: Insert your specific project scope, feature request, or business logic here.]
