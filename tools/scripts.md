# Approved Commands & Scripts

**To the AI Agent:**
Do not guess terminal commands. Use the specific package manager or build tool defined for this project's stack. Below are the approved scripts based on common ecosystems. Only use the ones relevant to the current project stack defined in `project.md`.

## Node.js / TypeScript (npm / pnpm / yarn)
- **Run Dev:** `npm run dev`
- **Run Linter:** `npm run lint`
- **Run Tests:** `npm run test`
- **Build:** `npm run build`

## Python (Poetry / pip)
- **Run Dev:** `fastapi dev main.py` (or `python manage.py runserver`)
- **Run Tests:** `pytest`
- **Run Linter/Formatter:** `black . && isort .`
- **Migrations:** `alembic upgrade head`

## Rust (Cargo)
- **Run Dev:** `cargo run`
- **Run Tests:** `cargo test`
- **Run Linter:** `cargo clippy`
- **Format:** `cargo fmt`

## Go
- **Run Dev:** `go run main.go`
- **Run Tests:** `go test ./...`
- **Format:** `go fmt ./...`

*(User: Delete the language sections that do not apply to your current project to give the agent clear boundaries.)*
