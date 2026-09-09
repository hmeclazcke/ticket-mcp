# Ticket MCP - Vision

## Purpose

Build an internal IT support system for an organization.

Employees can report technical problems as tickets, and IT technicians can search, review and close those tickets.

Examples of support requests include:

- A notebook does not turn on.
- A user cannot log in.
- A printer is not working.
- An employee needs access to a system or shared resource.

## Core capabilities

The initial business capabilities are:

- Create a ticket.
- Find a ticket by ID.
- List open tickets.
- Close a ticket.

## Learning goals

The project is intended to learn and practice:

- Quarkus
- Modern Java 25
- PostgreSQL
- REST APIs
- OpenAPI
- Model Context Protocol (MCP)
- OAuth2 with Keycloak
- Kubernetes

## Technical direction

- Java 25
- Quarkus
- Maven
- PostgreSQL
- REST
- OpenAPI
- MCP Server
- Keycloak
- Kubernetes

## Architecture direction

Business rules should remain independent from frameworks and infrastructure.

REST and MCP will be treated as different entry points to the same application use cases.

Infrastructure concerns such as PostgreSQL, authentication and deployment should remain outside the core business logic.

## Development approach

The project combines:

- Lightweight Specification-Driven Development
- TDD
- Human-written learning-critical implementation
- AI-assisted repetitive implementation

New concepts should be understood before implementation is delegated to an AI coding agent.