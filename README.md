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
- **`/tools/security/`**: Rules for rate limiting, OWASP Top 10, Webhooks, Encryption at Rest, and API security.
- **`/tools/compliance/`**: GDPR/CCPA privacy rules, password hashing, and PII masking.
- **`/tools/frontend/`**: Guidelines for mobile-first responsiveness, Core Web Vitals, data sanitization, and internationalization (i18n).
- **`/tools/performance/`**: Directives for modularity, background tasks, pagination, and caching.
- **`/tools/recipes/`**: Standardized, step-by-step instructions for repetitive tasks like creating components or API routes.
- **`/tools/skills.md`**: Defines specialized skills/plugins the AI is allowed to invoke (e.g., SAST tools, API contract testers).

## Getting Started

1. Copy the entire `tools/` folder into the root of your project.
2. Open `tools/project.md` and define your **Tech Stack**.
3. Open `tools/scripts.md` and remove the commands that don't apply to your stack.
4. Point your AI Coding Assistant (e.g., Cline, Antigravity, Cursor, Copilot) to `tools/project.md` and start typing your first task!
