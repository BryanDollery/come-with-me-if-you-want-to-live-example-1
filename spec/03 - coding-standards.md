---
spec_order: 3 of 4
required: true
preceded_by:
 - @spec/02 - architecture.md
followed_by:
 - @spec/04 - processes.md
---

# Project Coding Standards

---
applyTo: "**"
---
## General
- Write secure code at all times being aware of common vulnerabilities (e.g. OWASP Top 10)
- Consistent 2-space indentation, no tabs
- Self-documenting code, no comments
- Lowercase preferred (except syntax requirements)
- Short methods, meaningful names
- Colored output, standard logging
- Never commit secrets, use .env
- Always use lower-case file names except where it's illegal. e.g. readme.md, not README.md

---
applyTo: "*.js, *.ts, *.jsx, *.tsx"
---
## JavaScript/TypeScript
- ES2024+: fat arrows, const/let, async/await, destructuring
- No braces for single-line conditionals
- Inline single-use variables
- Import order: external → internal → relative
- Interfaces over types for objects
- All source code in `src/`, tests in `tests/`

---
applyTo: "*.jsx, *.tsx"
---
## React
- Functional components + hooks only
- Tailwind, ShadCN/UI, Tanstack Router/DB
- Bun for dev server and tests

---
applyTo: "*.sh"
---
## Bash
- Modern bash, non-POSIX OK
- Full paths for tools (may be aliased): `/usr/bin/cat`

---
applyTo: "dockerfile"
---
## Dockerfile
- lowercase instructions, multi-stage builds

---
applyTo: "makefile"
---
## Makefile
- Use for build/automation
- Complex logic → bash scripts

---
applyTo: "*.puml"
---
## PlantUML
- Read the models before making changes
- Update diagrams before implementing *changes*
