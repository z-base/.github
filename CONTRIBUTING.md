# Contributing to z-base

STATUS: DRAFT

This document describes how collaboration is expected to work.
It is not final. Nothing here is absolute.

z-base is highly modular by design.
Each package and each specification lives in its own repository.
Coordination happens through architecture, not through a monolith.

---

## 1. Independent First

Anyone is welcome to:

- Use the package template
- Create a new module or specification
- Publish it in their own GitHub / Git provider
- Iterate independently

There is no permission gate for experimentation.

The ecosystem grows by parallel exploration.

---

## 2. Community Convergence

The community may decide that:

- A package aligns with z-base architectural direction
- A specification fills a core gap
- A module becomes a foundational primitive

At that point, discussion may begin about deeper collaboration.

---

## 3. Direct Collaboration Model

Direct collaboration on:

- Implementation
- Specification authorship
- Normative evolution

is not assumed.

It must be explicitly agreed upon with the original author.

If a module or spec becomes foundational:

- Ownership MAY be transferred to the `z-base` organization
- Or shared governance MAY be established
- Or it MAY remain external but recognized

Merged contributors are always credited.

No contribution erases authorship.

---

## 4. Modular Structure

The project is intentionally modular:

- One repository per package
- One repository per specification
- Clear boundaries between runtime logic and normative definitions

Large multi-domain repositories are discouraged.

Modularity is not aesthetic.
It is governance and auditability.

---

## 5. Specification Discipline

Specifications are implementation-agnostic.

They must:

- Define semantics, not code structure
- Avoid platform-specific assumptions
- Remain deterministic and portable
- Reference normative sources where possible

RFC 2119 keywords MUST be interpreted according to:
https://www.rfc-editor.org/rfc/rfc2119.html

When writing or modifying specifications, prefer:

- WHATWG Infra
- ECMA-262
- JSON (RFC 8259)
- URI (RFC 3986)
- JSON-LD 1.1
- RDF Concepts / RDF Schema
- WebCrypto Level 2
- JOSE RFCs (7515–7519, 7638, 8037, etc.)
- DID Core
- VC Data Model

Do not invent behavior if a normative reference exists.

---

## 6. Implementation Discipline

Runtime libraries are:

- ESM format specific
- JS runtime-agnostic
- Deterministic
- Explicit

Guidance is defined in AGENTS.md.

Highlights:

- Minimal surface area
- One responsibility per module
- Typed, semantic error classes
- No implicit global state
- No infrastructure reimplementation
- Dependency preference over boilerplate
- Strict separation of `.types/`, `.errors/`, `.helpers/`

Architecture is treated as a constraint system.

---

## 7. Governance Reality

z-base is not a DAO.
It is not consensus-driven for its own sake.

Architecture decisions are based on:

- Semantic clarity
- Portability
- Determinism
- Security
- Long-term coherence

Disagreement is expected.
Forking is allowed.
Experimentation is encouraged.

Centralization of authority inside the system is rejected.
Centralization of editorial direction may still exist.

These are different things.

---

## 8. Credits

All merged contributors are credited.
Authorship history is preserved.
Specifications retain attribution.

Portability of identity applies to contributors too.
