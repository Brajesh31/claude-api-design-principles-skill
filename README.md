# claude-api-design-principles-skill

A Claude Code skill for designing intuitive, consistent, secure, and maintainable REST and GraphQL APIs.

## Overview

This skill helps define API contracts that are easy for consumers to understand and stable as systems evolve. It covers resource modeling, request and response design, errors, pagination, versioning, GraphQL schemas, and practical implementation considerations.

## Main Capabilities

- Design REST resources and endpoints.
- Define HTTP methods and status codes.
- Structure request and response payloads.
- Design consistent error responses.
- Plan pagination, filtering, and sorting.
- Model GraphQL schemas and operations.
- Improve API discoverability and documentation.
- Consider versioning and backward compatibility.
- Review API usability for mobile and third-party clients.
- Validate API contracts before implementation.

## Design Principles

### Consistency

Use predictable naming, response structures, status codes, and error formats across the API.

### Resource-Oriented Design

Model resources around domain concepts. Avoid exposing internal database structures without considering consumer needs.

### Compatibility

Plan how clients will handle new fields, deprecated operations, and breaking changes.

### Security

Enforce authentication, authorization, validation, and rate limits at the appropriate boundaries.

### Developer Experience

Provide understandable contracts, examples, and error messages.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-api-design-principles-skill.git ~/.claude/skills/api-design-principles
```

## Usage

Invoke the skill when designing or reviewing an API contract:

```text
/api-design-principles
```

Provide the domain model, target clients, data requirements, authentication model, and compatibility constraints.

## Recommended Workflow

1. Identify API consumers and their workflows.
2. Define the domain resources and relationships.
3. Choose REST or GraphQL based on access patterns.
4. Design endpoints or schema operations.
5. Define validation and error behavior.
6. Plan pagination and filtering.
7. Review security and authorization boundaries.
8. Document examples and expected responses.
9. Test compatibility and edge cases.
10. Review the design with API consumers.

## Repository Resources

- `assets/api-design-checklist.md`: API design review checklist.
- `assets/rest-api-template.py`: REST API template utility.
- `references/graphql-schema-design.md`: GraphQL schema design guidance.
- `references/rest-best-practices.md`: REST implementation practices.
- `resources/implementation-playbook.md`: Implementation and review playbook.

## API Review Checklist

- Resource names are clear and consistent.
- HTTP methods reflect operation semantics.
- Status codes match actual outcomes.
- Errors have stable structures.
- Pagination is predictable.
- Authorization is enforced per resource and action.
- Inputs are validated.
- Breaking changes are managed.
- Examples match the contract.
- Tests cover success and failure cases.

## Repository Contents

- `SKILL.md`: Main API design instructions.
- `assets/`: Checklist and template utility.
- `references/`: REST and GraphQL design guidance.
- `resources/`: Implementation playbook.
- `README.md`: Overview and workflow.

## Practical Principle

Design for the client workflow, not for the shape of the database. A technically consistent API can still be difficult to use if it does not match how consumers need to work.
