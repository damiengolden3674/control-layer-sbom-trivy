# Architecture Boundary — Anti-Reconstruction Contract

## Hierarchy
**Human → The Control Layer → Control AI → Governed Executor → Ecosystem/OS**

A repository can implement a capability, but it cannot become the authority that governs itself.

## What this repository deliberately does not contain
- private root-of-trust material
- production signing keys or secrets
- authoritative runtime identity
- complete production dependency graph
- final release authorization
- production credentials
- recovery credentials
- human approval records

## Reconstruction rule
Cloning every public repository may reproduce source code. It must **not** reproduce an authoritative Control Layer deployment.

A production claim is valid only when the private trust domain binds:
**component identity + exact release + architecture contract + policy/adjudication + runtime attestation + governed executor + recovery evidence**.

If any required binding is absent, stale, revoked, or inconsistent, the correct state is **HOLD** or **ESCALATE**.

## Security model
This is not security through obscurity. Public source remains intentionally inspectable. The protected boundary is authorization, cryptographic identity, signed release state, runtime attestation, private state, and human authority.
