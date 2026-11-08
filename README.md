# claude-cc-skill-backend-patterns-skill

A Claude Code skill for backend architecture, API design, database performance, and reliable server-side application patterns.

## Overview

This skill focuses on practical backend engineering across Node.js, Express, and Next.js API routes. It covers API contracts, service boundaries, persistence, validation, error handling, and performance.

## Main Topics

### API Design

- Resource-oriented REST endpoints.
- Consistent HTTP methods and status codes.
- Filtering, sorting, and pagination.
- Stable response and error formats.
- Authentication and authorization boundaries.

### Application Architecture

- Route and controller responsibilities.
- Service-layer business logic.
- Repository and persistence boundaries.
- Dependency management.
- Modular organization.

### Database Design and Performance

- Schema and index design.
- Query efficiency.
- Transaction boundaries.
- Connection management.
- Avoiding N+1 query patterns.
- Migration planning.

### Reliability

- Input validation.
- Structured error handling.
- Timeouts and retries.
- Idempotency.
- Logging and observability.
- Background and asynchronous processing.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-cc-skill-backend-patterns-skill.git ~/.claude/skills/cc-skill-backend-patterns
```

## Usage

Invoke the skill for backend design or implementation tasks:

```text
/cc-skill-backend-patterns
```

Provide the runtime, framework, database, API consumers, expected workload, and reliability requirements.

## Recommended Workflow

1. Inspect existing routes, services, and data access.
2. Define the API contract.
3. Identify business logic and data ownership.
4. Choose a suitable architecture boundary.
5. Validate input at trust boundaries.
6. Implement persistence with explicit transaction behavior.
7. Handle errors consistently.
8. Add tests and observability.
9. Review query performance and security.
10. Verify deployment and migration impact.

## API Example

```text
GET    /api/items
GET    /api/items/:id
POST   /api/items
PATCH  /api/items/:id
DELETE /api/items/:id
```

Use resource naming and method semantics consistently. Define authorization and validation for every operation.

## Quality Checklist

- API contracts are predictable.
- Business logic is separated from transport code.
- Database access is efficient and tested.
- Authentication and authorization are enforced.
- Errors are handled consistently.
- Retries are safe and bounded.
- Logs avoid sensitive data.
- Migrations are reversible where possible.
- Tests cover success and failure paths.

## Repository Contents

- `SKILL.md`: Main backend development patterns.
- `README.md`: API, architecture, and database guidance.

## Practical Principle

Do not optimize the database before understanding the query workload. Measure real access patterns, then design indexes, caching, and service boundaries around evidence.
