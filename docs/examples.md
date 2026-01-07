# Enterprise Orbit Diagram — Canonical Example

This document presents a **canonical example** of the Enterprise Orbit Diagram (EOD).

Its purpose is to serve as a **single reference instance** that demonstrates how the conventions of the Enterprise Orbit Diagram are applied in practice: positioning, grouping, distance, and narrative intent.

This example is **illustrative**, not prescriptive.
Organizations may adapt the diagram to their context, as long as the core meaning and conventions are preserved.

---

### Context

The diagram represents an organization at an early discovery stage, where existing documentation is limited or overly technical.

The goal is to create a shared mental model that helps business and technology stakeholders understand:

- what defines the business,
- what directly supports it,
- and what merely enables its operation.

---

### Business Core

At the center of the diagram is the **Business Core**.

It represents the organization’s identity-defining capability — the part of the enterprise that produces business value and without which the organization would no longer recognize what it sells.

Elements shown inside the core (such as domain models, rules, and business outputs) are tightly coupled and evolve together as part of the same business meaning.

---

### Orbiting Systems

Surrounding the Business Core are the **Orbiting Systems**.

They support or operationalize the core capability and are positioned according to **business criticality and coupling**, not technical architecture.

Examples include:

- Core operational platforms
- Analytics & Integration

Systems positioned closer to the core are harder to replace and more tightly coupled to business outcomes.

---

### Cross-Cutting, Legacy, and External Systems

Some systems enable the enterprise without defining or extending the business core. These systems are intentionally positioned **outside the core groupings**.

Typical examples include:

- Identity & Access Management (CC)
- Web Store Catalog (CC)
- API Management (CC)
- Payment Gateway (E)
- Email Notifications (E)
- Legacy POS (L)

* CC=Cross-Cutting | L=Legacy/Transitional | E=External Partner
  
Their placement communicates **enablement, dependency, or transition**, rather than differentiation.

---

### Intended Outcome

This diagram is designed to be understood **without technical documentation**.

It enables stakeholders to reason about:

- What truly defines the business?
- What belongs to the core versus what supports it?
- Which systems are critical, which systems matter most, and which are replaceable?
- Where does the organization’s true complexity reside?

The diagram acts as a **conversation starter**, not a technical contract.

---

### Visual Reference

![Enterprise Orbit Diagram — Canonical Example](diagrams/enterprise-orbit-diagram-example.png)

---

This canonical example represents **version 1** of the Enterprise Orbit Diagram in practice. Future examples may explore additional scenarios while preserving this reference model.
