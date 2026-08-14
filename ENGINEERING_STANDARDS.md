# OAE™ Engineering Standards

## Purpose

This repository follows the Open Autonomous Engineer (OAE™) engineering standard for controlled, auditable improvement.

## Required Practices

### Security
- Never commit credentials, tokens, private keys, or production secrets.
- Validate untrusted inputs at system boundaries.
- Keep deployment configuration explicit and reviewable.

### Architecture
- Prefer small, cohesive modules.
- Avoid duplicated domain logic.
- Preserve clear boundaries between application logic, integrations, automation, and deployment.

### Testing
- Every substantive capability must have automated tests.
- Include normal, edge, and failure cases where applicable.
- Tests must not depend on hidden network state unless explicitly classified as integration tests.

### Verification
A change is not complete merely because it compiles or appears to work. Acceptance requires appropriate automated verification and inspection of the resulting change.

### Change Control
- Make one coherent change at a time.
- Keep changes reviewable.
- Preserve existing behaviour unless the change intentionally modifies the contract.
- Record consequential architectural decisions.

### Production Readiness
Production readiness must be demonstrated, not assumed. The repository must have a verified application runtime, configuration contract, tests, deployment path, and operational documentation before it is described as production-ready.

## OAE™ Improvement Loop

```text
Observe → Understand → Plan → Approve → Implement → Test → Verify → Measure
```
