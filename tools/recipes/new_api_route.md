# Recipe: Creating a New API Route

**To the AI Agent:**
When scaffolding a new backend route, follow these steps:
1. Define the route using the versioning strategy (e.g., `/api/v1/resource`).
2. Validate incoming requests using the standard validation library for our stack (e.g., Zod for TypeScript, Pydantic for Python, validator for Go/Rust).
3. Implement the controller logic.
4. Adhere to security guidelines (e.g., rate limiting, as per `tools/security/security.md`).
5. Update the OpenAPI/Swagger documentation to reflect the new route.
