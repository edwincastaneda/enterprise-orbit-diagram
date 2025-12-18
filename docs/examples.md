# Enterprise Orbit Diagram — Canonical Example

This document presents the **canonical example** of the Enterprise Orbit Diagram (EOD).

The purpose of this example is to provide a **single, clear reference implementation** of the method. It demonstrates how narrative intent, positioning, and grouping work together to communicate enterprise structure to non-technical and strategic audiences.

This example should be understood as **illustrative, not prescriptive**. Organizations may adapt the diagram to their context while respecting the core conventions.

---

## Canonical Example: Enterprise Orbit Diagram

### Context

An organization needs to explain its enterprise software landscape to business stakeholders as an initial discovery artifact. Existing documentation is either missing or overly technical, making it difficult to understand which systems truly matter.

The goal of this diagram is to create a **shared mental model** of the organization’s technology assets, highlighting what is core, what is supporting, and what is merely enabling.

---

### Business Core

At the center of the diagram is the **Business Core**.

This represents the primary domain capability that defines the organization’s value proposition. It is not a system, but the business concept around which all technology exists.

---

### Orbiting Systems

The orbit contains the primary enterprise systems that directly interact with and support the Business Core. These systems are positioned based on **business criticality**, not technical layering.

Examples include:

* Core operational platforms
* Systems of record closely tied to the domain
* Strategic applications that shape how the business operates

Systems positioned closer to the core are harder to replace and more tightly coupled to business outcomes.

---

### Cross-Cutting and External Systems

Some systems enable the organization without defining its business model. These systems are intentionally left **outside any grouping** and placed further from the core.

Typical examples include:

* Identity & Access Management
* Payment Gateways
* Email & Notifications
* External Partners

Their placement communicates enablement rather than differentiation.

---

### Narrative Outcome

Without reading a single technical specification, stakeholders can answer questions such as:

* What capabilities define the business?
* Which systems are critical versus replaceable?
* Where does the organization’s complexity truly live?

The diagram acts as a **conversation starter**, not a technical contract.

---

### Visual Reference

![Enterprise Orbit Diagram — Canonical Example](diagrams/enterprise-orbit-diagram-example.png)

---

This canonical example represents **version 1** of the Enterprise Orbit Diagram in practice. Future versions may introduce additional scenarios while preserving this reference model.
