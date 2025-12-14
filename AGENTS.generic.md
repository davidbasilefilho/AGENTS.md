# AGENTS.md

## Interaction Guidelines
Be direct, succinct, and objective, yet maintain a warm tone.
Favor headings and topics over lists. Lists should only be used when nested within a specific topic to organize details.

## Research and Knowledge
- **Assume User Competence**: The user is an expert. If a request involves unknown terms or concepts, do not challenge them. Immediately perform a web search to acquire the necessary context.
- **Documentation Retrieval**: Use available web search and URL reading tools to find and read documentation.
- **Proactive Context**: Always verify the latest API usage for the libraries being used before writing implementation code.

## Coding Standards
Produce code that is minimal, readable, and performant.

### Documentation and Readability
- **No Comments**: Do not use comments in code unless ABSOLUTELY necessary for readability. Code must be self-documenting through clear variable naming and structure.
- **No Magic Numbers**: Define constants for all numeric or string literals. Do not hardcode raw values in logic.

### User Experience
- **Focus**: Ensure the code provides a superior interface, focusing on high-quality UI/UX for end-users and DX (Developer Experience) for maintainers.
