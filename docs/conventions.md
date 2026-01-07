# Enterprise Orbit Diagram — Conventions

This document defines the **canonical conventions** of the Enterprise Orbit Diagram (EOD).

The goal of these conventions is not visual aesthetics, but **clarity of business meaning**.  
Every position, color, grouping and connection exists to answer a single question:

> *What truly defines the business, and what merely enables it?*

---

## 1. Core Principle

The Enterprise Orbit Diagram is a **business-first representation** of an enterprise software landscape.

It deliberately avoids:
- Technical layers
- Infrastructure detail
- Deployment topology
- Vendor-specific architectures

Instead, it focuses on **semantic and strategic importance**.

### Decision Helper

To decide whether something belongs to the core or to the orbit, use this question:

> **If this system disappears, does the business still know what it is selling?**

- **No** → Core (or core component)
- **Yes** → Orbit

This question must always override technical convenience or organizational politics.

---

## 2. Business Core

The **Business Core** represents the **irreducible business capability** of the organization.

Key characteristics:
- It is a **business concept**, not a system
- It defines *what* the company is and *what it sells*
- It is stable over time, even if implementations change

The Business Core is always:
- Singular
- Placed at the center
- Visually dominant

---

## 3. Core Components (Extended Core)

Some domains are so tightly coupled to the Business Core that separating them would distort reality.

These are considered **Core Components**, forming an **Extended Core**.

They are:
- Drawn immediately adjacent to the Business Core
- Never optional
- Not interchangeable without redefining the business

---

## 4. Orbiting Systems

Orbiting systems are enterprise systems that **operate around the core**, supporting it but not defining it.

Characteristics:
- Replaceable over time
- Important, but not identity-defining
- Positioned by **business criticality**, not architecture

Distance from the core visually communicates:
- Coupling strength
- Replacement cost
- Strategic weight

---

## 5. Groupings (Narrative Boundaries)

Groupings represent **narrative or conceptual boundaries**, not ownership or deployment units.

Rules:
- Groupings may overlap visually
- They must never imply data ownership
- They exist to help storytelling, not enforcement

---

## 6. Cross-Cutting and External Systems

Some systems enable the enterprise without belonging to any narrative group.

Rules:
- They are placed outside core and orbit groupings
- They must never appear closer to the core than orbiting systems
- Their role is **enablement, not differentiation**

---

## 7. Connections and Flows

Connections represent **meaningful business interactions**, not integrations.

Guidelines:
- Arrows indicate **direction of influence or dependency**
- Avoid bi-directional arrows unless unavoidable
- Prefer fewer, clearer flows over exhaustive accuracy

Connections should answer:
- Who initiates value?
- Who consumes outcomes?
- Where does information *matter*, not travel?

### Arrow Semantics

The diagram uses a **limited set of arrow types**, each with a specific narrative meaning:

- **Solid Arrow**  
  Represents a **primary business dependency**.  
  Indicates that the target component is a direct outcome or responsibility of the source.

- **Dashed Arrow**  
  Represents a **supporting or enabling dependency**.  
  Used when a component influences or constrains another without owning the outcome.

- **Thin / Subtle Arrow**  
  Represents **observational or consumptive relationships**.  
  Used for analytics, reporting, or passive usage of business results.

Only these arrow types are allowed in canonical diagrams.

---

## 8. Color Usage

Color is used to **reinforce meaning**, not to encode technical classifications.

Fixed semantic colors are preferred for consistency:

- **Light Blue**  
  Business Core

- **Lime Green**  
  Extended Core Components

- **Yellow**  
  Orbiting Systems over Narrative Groupings (dashed boundaries)

- **Gray**  
  Cross-cutting Systems

- **Soft Red**  
  External Systems

- **Soft Orange**  
  Transitional or legacy elements (when explicitly needed)

- **White**  
  Neutral space / canvas


Rules:
- Color must never be overloaded with multiple meanings
- Shape and position take precedence over color
- Legends must be minimal and readable by non-technical audiences

---

## 9. What the Diagram Explicitly Avoids

The Enterprise Orbit Diagram must **not** include:

- Microservices
- APIs or protocols
- Databases
- Infrastructure (cloud, on-prem, regions)
- Ownership by teams
- Technology stacks

If any of these appear, the diagram has crossed into architecture and lost its purpose.

---

## 10. Canonical Description

The Enterprise Orbit Diagram is a **strategic narrative tool**.

Its primary use cases are:
- Executive alignment
- Discovery workshops
- Product and platform framing
- Explaining complexity without technical depth

It is not:
- An architecture diagram
- A replacement for technical documentation
- A governance artifact

---

## 11. Evolution Over Time

The diagram may evolve, but only in **controlled ways**.

Allowed evolution:
- Refining groupings
- Repositioning orbiting systems
- Extracting or absorbing core components

Disallowed evolution:
- Multiple business cores
- Technical layering creeping in
- Color semantics changing per diagram

Evolution should be shown via:
- Versioned diagrams
- Side-by-side comparisons
- Small schematic mini-diagrams, not full redraws

The mental model must remain stable even as the organization changes.

---


