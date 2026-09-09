# AGENTS.md

## Project purpose

This is a learning-oriented portfolio project for building an internal IT support ticket system using modern Java and cloud-native technologies.

The project combines:

- Lightweight Specification-Driven Development (SDD)
- Test-Driven Development (TDD)
- Human-written learning-critical code
- AI-assisted implementation

## Engineering principles

Use Robert C. Martin and Martin Fowler as engineering references, without applying their ideas dogmatically.

- Prefer simple designs that satisfy the current requirements.
- Follow SOLID principles where they provide clear value.
- Keep business rules independent from frameworks and infrastructure.
- Dependencies should point toward the domain.
- Separate business logic from delivery mechanisms such as REST and MCP.
- Prefer small, reviewable changes.
- Avoid speculative abstractions and premature generalization.
- Refactor continuously while preserving behavior.
- Optimize for readability and maintainability.
- Follow DRY (Don't Repeat Yourself): avoid duplicating business rules,
    knowledge and implementation logic across the codebase.
- Do not remove duplication prematurely when doing so would introduce
  unnecessary abstractions.
- Prefer a small amount of obvious duplication over the wrong abstraction.

## Specification-Driven Development

- Implement only behavior required by the current approved specification.
- Do not implement future features in advance.
- Work on one small specification at a time.
- Each specification must describe behavior and acceptance criteria before implementation.
- Keep `docs/current.md` updated with the current project state.

## Testing and TDD

- Important behavior must have automated tests.
- Prefer defining important behavior with a test before implementing it.
- Do not modify a valid test merely to make production code pass.
- Tests should verify behavior, not implementation details.
- Refactor only while the relevant test suite is green.
- Prefer fast unit tests for business logic.
- Add integration tests where interaction with frameworks or infrastructure must be verified.

## Learning rules

This is a learning project.

- New technologies and concepts are learning-critical.
- Explain new concepts before introducing them.
- The first implementation of a new concept should be written or explicitly reviewed by the human.
- Do not hide learning-critical behavior behind generated boilerplate.
- Once a concept or pattern is understood, repetitive implementation may be delegated to the coding agent.

## Technology policy

- Target Java 25.
- Prefer the latest stable releases of frameworks, libraries and tools.
- Prefer modern stable Java features when they provide a concrete benefit.
- Preview features require an explicit reason before use.
- Do not introduce a technology or language feature merely to demonstrate it.
- Explain why a modern Java feature is preferable before introducing it.
- Document relevant modern Java features and important technology choices in `README.md`.

## AI-assisted implementation

- The coding agent may generate repetitive or mechanical implementation after the underlying concept is understood.
- The agent must not silently introduce new frameworks, libraries or architectural patterns.
- New dependencies require an explicit reason.
- Prefer modifying the smallest possible surface area.
- Do not perform unrelated refactoring while implementing a feature.

## Verification

Before considering a task complete:

- Run the relevant automated tests.
- Verify that the implementation satisfies the current specification.
- Check that no unnecessary functionality was added.
- Keep the code readable and simple.