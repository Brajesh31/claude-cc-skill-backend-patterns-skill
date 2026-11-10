# Claude Code Backend Patterns Skill

A Claude Code skill covering practical backend architecture and server-side engineering patterns for Node.js, Express, and Next.js API routes.

It helps structure backend systems around clear API contracts, maintainable application boundaries, reliable data access, and operational safeguards.

## Topics Covered

### API Design and Application Architecture

- Resource-oriented REST API design.
- HTTP methods, status codes, filtering, sorting, and pagination.
- Service-layer and repository patterns.
- Middleware and separation of transport code from business logic.

### Database Design and Performance

- Query optimization and selective data retrieval.
- Preventing N+1 query patterns.
- Transaction boundaries and atomic operations.
- Cache-aside and Redis caching strategies.

### Reliability and Security

- Centralized error handling.
- Bounded retries with exponential backoff.
- JWT authentication and role-based access control.
- Rate limiting and input validation.
- Structured logging and monitoring.

### Background Processing

- Queue patterns for asynchronous work.
- Separating long-running operations from request handling.
- Failure handling and operational visibility.

## Installation

Clone the repository into your Claude skills directory:

```bash
git clone https://github.com/Brajesh31/claude-cc-skill-backend-patterns-skill.git ~/.claude/skills/cc-skill-backend-patterns
```

To update an existing installation:

```bash
cd ~/.claude/skills/cc-skill-backend-patterns
git pull
```

## Usage

Invoke the skill when planning, reviewing, or implementing backend functionality:

```text
/cc-skill-backend-patterns
```

Give Claude the relevant context, including:

- Runtime and framework.
- Database and data-access layer.
- API consumers and authentication requirements.
- Expected workload and performance constraints.
- Reliability, observability, and deployment requirements.

Example request:

```text
Use the backend patterns skill to review my Express API.
Focus on route structure, validation, database queries, error handling,
authentication, and test coverage.
```

## Recommended Workflow

1. Inspect the existing routes, services, data models, and persistence layer.
2. Define the API contract and authorization rules.
3. Separate transport handling from business logic.
4. Choose architecture patterns that match the system's actual complexity.
5. Validate untrusted input at system boundaries.
6. Make database operations efficient and transaction-safe.
7. Handle errors consistently and use bounded retries where appropriate.
8. Add tests for success, failure, and edge cases.
9. Add structured logs without exposing secrets or personal data.
10. Measure performance before introducing caching or additional infrastructure.

## Repository Contents

- `SKILL.md`: Main instructions and backend engineering patterns.
- `README.md`: Installation, usage, coverage, and workflow guidance.
- `LICENSE`: MIT License.

## Engineering Principles

- Prefer simple architecture over unnecessary abstraction.
- Make API behavior explicit and predictable.
- Enforce authorization at the server boundary.
- Measure database performance before optimizing.
- Keep retries bounded and safe for the operation being retried.
- Treat logs and error messages as potential data-leak surfaces.
- Test behavior, not just implementation details.

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE).
