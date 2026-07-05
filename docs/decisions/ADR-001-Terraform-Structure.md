# ADR-001 - Terraform Structure

## Status
Accepted

## Context

The project requires multiple environments (Development, Test, Production).
The infrastructure should be modular, reusable and maintainable.

## Decision

We will use a modular Terraform structure with reusable modules and separate environment folders.

modules/
    resource-group/
    storage-account/
    azure-openai/
    ai-search/

environments/
    dev/
    test/
    prod/

## Consequences

- Reusable modules
- Easier maintenance
- Environment isolation
- CI/CD friendly
- Enterprise-ready