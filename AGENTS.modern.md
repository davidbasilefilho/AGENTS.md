# AGENTS.md

## Interaction Guidelines
Be direct, succinct, and objective, yet maintain a warm tone.
Favor headings and topics over lists. Lists should only be used when nested within a specific topic to organize details.

## Research and Knowledge
- **Trust User Knowledge**: Assume the user knows what they are talking about. If a request involves something outside your knowledge base, do not assume it does not exist. Research it to acquire context.
- **Documentation Retrieval**: You must use `context7` to fetch documentation. You are ONLY permitted to use web search for documentation fetching if `context7` is unavailable.
- **Proactive Context**: Always verify the latest API usage for the "Modern Tooling Stack" listed below before writing implementation code.

## Modern Tooling Stack
Adopt modern, high-performance tooling by default. Refrain from using legacy equivalents unless explicitly requested.

### JavaScript/TypeScript Ecosystem
- **Runtime**: Use `bun` instead of `node`/`npm`.
- **Package Execution**: Use `bun x --bun` instead of `npx`.
- **Shell Commands**: Use Bun Shell (`$` from `bun`) instead of `execSync`, `spawn`, or other Node.js child process methods.
- **Functional Effects**: Use `effect-ts` for TypeScript projects requiring structured side-effect management, concurrency, and error handling.
- **Framework**: Use `tanstack start` instead of `next.js` or `react-router`.
- **Testing**: Use `vitest` instead of `jest`.
- **Backend**: Use `convex` instead of `supabase` or `firebase`.

### Python Ecosystem
- **Package Management**: Use `uv` instead of `pip` or `poetry`.

### Environment Management
- **General**: Always use `jdx mise` for version management and task running.

## Coding Standards
Produce code that is minimal, readable, and performant.

### Documentation and Readability
- **No Comments**: Do not use comments in code unless ABSOLUTELY necessary for readability. Code must be self-documenting through clear variable naming and structure.
- **No Magic Numbers**: Define constants for all numeric or string literals. Do not hardcode raw values in logic.

### API Design Patterns
- **Dual Getter-Setter Functions**: Use combined getter-setter functions instead of separate methods. A call with no arguments returns the current value; a call with an argument sets the value (e.g., `property()` to get, `property(value)` to set).

### User Experience
- **Focus**: Ensure the code provides a superior interface, focusing on high-quality UI/UX for end-users and DX (Developer Experience) for maintainers.
