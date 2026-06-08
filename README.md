# Vibecoding Toolset (Agentic AI Workflow)

> **Created and maintained by: Antony Ngemu (tech@tuinnov8.com)**

Natural Language is the future of coding and programming, ushering in the new role of the *Prompt Engineer*. However, the fundamental principles of programming will never be skipped. Therefore, this workflow does the heavy lifting of enforcing required coding standards, ensuring those core principles are never ignored by your AI coding agents.

While the Software Development Life Cycle (SDLC) phases remain unchanged, this workflow will help you deliver a production-grade solution faster—saving you from unforeseen problems, wasted time, and burned AI credits. The time is now to elevate yourself and become a Prompt Engineer, not just a "VibeCoder".

When using this toolkit, focus your time on refining the **business logic**, the **system architecture**, and the **UI design**. Let the framework handle the rest.

## Features
- Language-Agnostic Architecture (Node.js, Python, Rust, Go)
- Security & Compliance (OWASP, Rate Limiting, Encryption at Rest, GDPR)
- Performance & Optimization
- Coding Best Practices (SOLID, DRY)
- UI/UX Design Guidelines (Responsiveness, A11y, i18n)
- Scalable Architecture & Database Schemas

## Workflow Structure & Where to Modify

The magic of this workflow relies on the central hub (`project.md`), which acts as an automatic router for your AI agent. When you issue a prompt via `project.md`, the AI analyzes the scope of your task, scans the entire `tools/` directory, and autonomously applies the relevant guardrails (e.g., pulling in `security.md` for backend tasks or `ui.md` for frontend tasks).

Most of the framework consists of **strict guardrails** that shouldn't be altered unless your organization's standards change. However, there are a few specific places where you **must** interact with and edit the workflow:

### 📝 Files You Need to Edit:
1. **`tools/project.md` (The Brain):**
   - **Where you work every day.** Define your **Tech Stack** at the top (Language, Framework, Package Manager).
   - Write your daily prompts and business logic under the **Current Task** section.
2. **`tools/scripts.md` (The Commands):**
   - **Edit once per project.** This file contains standard terminal commands for various languages. Delete the languages that do not apply to your project so the AI only uses the correct scripts.
3. **`tools/memory.md` (The Log):**
   - **Review occasionally.** The AI will automatically log architectural decisions and bugs here. You can also manually edit this to add "gotchas" you want the AI to remember in future sessions.

### 🛡️ Guardrail Files (Do Not Edit, Let the AI Read):
The following files and directories enforce the principles of programming. The AI will read them automatically based on the context of your task.

```text
.
└── tools
    ├── accessibility
    │   └── a11y.md
    ├── api
    │   └── api.md
    ├── best-practices.md
    ├── ci-cd
    │   └── deployment.md
    ├── compliance
    │   └── privacy.md
    ├── database
    │   └── schema.md
    ├── frontend
    │   ├── i18n.md
    │   └── ui.md
    ├── images
    │   ├── architecture
    │   └── ui
    ├── memory.md
    ├── performance
    │   └── performance.md
    ├── project.md
    ├── recipes
    │   ├── new_api_route.md
    │   └── new_component.md
    ├── scripts.md
    ├── security
    │   └── security.md
    ├── skills.md
    └── testing
        └── testing.md
```

#### Detailed Breakdown of Files:

- **`accessibility/a11y.md`**: Enforces WCAG compliance, semantic HTML usage, ARIA roles, and keyboard navigation support.
- **`api/api.md`**: Sets standards for API versioning (e.g., `/api/v1/`), semantic HTTP status codes, and maintaining OpenAPI/Swagger documentation.
- **`best-practices.md`**: Mandates core programming principles such as SOLID, DRY, robust error handling (no silent failures), and descriptive naming conventions.
- **`ci-cd/deployment.md`**: Defines CI/CD pipeline stages (lint -> test -> build -> deploy) and instructions for generating efficient Dockerfiles.
- **`compliance/privacy.md`**: Ensures GDPR/CCPA compliance by instructing the agent to mask PII in logs and securely hash passwords.
- **`database/schema.md`**: Requires the use of ORMs/query builders, enforces strict naming conventions, and mandates that all schema changes use migrations.
- **`frontend/i18n.md`**: Instructs the agent to never hardcode strings in the UI, enforcing the use of localization files and translation hooks.
- **`frontend/ui.md`**: Sets guidelines for mobile-first responsiveness, Core Web Vitals optimization, professional icons, brand colors, and data sanitization to prevent XSS.
- **`images/architecture/ & ui/`**: Dedicated folders to store visual context, such as system design diagrams, database schemas, and UI mockups, for vision-capable agents.
- **`memory.md`**: Acts as the AI's continuous learning log to store architectural decisions and solved bugs, preventing the repetition of past mistakes.
- **`performance/performance.md`**: Contains rules for application scaling, including background task processing, code modularity, database pagination, and caching strategies.
- **`project.md`**: The central brain and routing mechanism. It contains your tech stack definitions and the daily task prompt.
- **`recipes/new_api_route.md`**: A templated step-by-step guide for scaffolding new backend endpoints securely.
- **`recipes/new_component.md`**: A templated guide ensuring every new UI component follows standard practices, including test creation.
- **`scripts.md`**: A list of approved, language-specific terminal commands (like running dev servers, tests, and linters) so the AI doesn't have to guess.
- **`security/security.md`**: The non-negotiable security guardrails covering rate limiting, OWASP Top 10 mitigation, webhook security, `.env` secret management, and encryption at rest.
- **`skills.md`**: Lists specialized plugins or capabilities the AI is authorized to invoke (e.g., SAST scanners, accessibility checkers).
- **`testing/testing.md`**: Establishes testing requirements, including unit testing business logic, E2E testing for critical paths, and maintaining minimum code coverage.

## Getting Started

1. Copy the entire `tools/` folder into the root of your project.
2. Open `tools/project.md` and define your **Tech Stack**.
3. Open `tools/scripts.md` and remove the commands that don't apply to your stack.
4. Point your AI Coding Assistant (e.g., Cline, Antigravity, Cursor, Copilot) to `tools/project.md` and start typing your first task!
