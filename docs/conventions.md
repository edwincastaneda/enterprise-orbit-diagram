# Enterprise Orbit Diagram — Conventions

This document defines the **official conventions** of the Enterprise Orbit Diagram (EOD).

The goal of these conventions is **clarity over precision**: the diagram is designed to explain enterprise software ecosystems to business and strategic audiences, not to model technical architectures in detail.

---

## 1. Core Principle

> **Everything revolves around the Business Core.**
> **Position communicates relevance, not technical layering.**

If this principle is respected, the diagram remains valid regardless of company size, industry, or technology stack.

---

## 2. Business Core

### Definition

The **Business Core** represents the primary domain, capability, or value proposition of the organization.

### Conventions

* There is **always one single core**
* It is placed **at the center** of the diagram
* It must be **visually dominant**

### What it represents

* A business domain
* A core capability
* The reason the organization exists

### What it does NOT represent

* A system
* A microservice
* A database
* A technical component


## Extended Business Core

### Definition
In some domains, a single business capability is implemented through multiple tightly coupled systems. In these cases, the diagram uses the concept of an **Extended Business Core**.

An Extended Business Core represents a **single conceptual core** composed of multiple internal components that together deliver the organization’s primary value.

### Conventions
- There is still **only one Business Core**
- The core may contain **internal components or sub-systems**
- Internal components do **not orbit** the core
- Internal components are not connected by arrows

> **A core may be internally composed, but it must be externally perceived as one.**

### What qualifies as a core component
A system qualifies as part of the Extended Business Core if, without it, the organization would no longer be able to define, structure, or deliver its primary offering.

Typical examples include:
- Product or Asset Information Management (PIM)
- Form or Schema Management
- Template or Document Generation

### Visual Guidance
The Extended Business Core may be represented as:
- A single large core with a composite label, or
- A core containing visually grouped internal components

The choice depends on diagram complexity and audience familiarity.

### Decision Helper: Core vs Orbit

When deciding whether a system belongs to the Business Core or the Orbit, use the following question:

> **If this system disappears, does the business still know what it is selling?**

- **No** → Business Core (or Core Component)
- **Yes** → Orbit

This heuristic intentionally focuses on **business identity and value**, not technical dependencies or operational convenience.

---

## 3. Orbit

### Definition

The **Orbit** represents the enterprise software ecosystem that interacts with the Business Core.

### Conventions

* There is **only one orbit**
* The orbit is not segmented
* The orbit does not represent layers or tiers

The orbit is a **narrative space**, not a technical boundary.

---

## 4. Orbiting Systems

### Definition

Each orbiting element represents a **software system or major module**.

### Conventions

* Represented as simple nodes (circles or basic shapes)
* No arrows by default
* Positioned relative to the core

### Positioning Rule

> **Distance from the core indicates business criticality and coupling.**

* Closer systems are more business-critical
* Distant systems are more replaceable or indirect

This positioning is intentionally subjective and designed to spark conversation.

---

## 5. Groupings (Narrative Boundaries)

### Definition

Groupings are **visual delimiters** (usually dotted or dashed shapes) used to highlight a shared business narrative.

### Conventions

* Groupings are optional
* They do not represent technical layers
* They do not imply ownership or deployment boundaries

### Purpose

* Explain workflows
* Highlight responsibility areas
* Tell a business story

> **Only systems that shape a shared narrative should be grouped.**

---

## 6. Cross-Cutting and External Systems

### Definition

Some systems enable the business without defining it.

### Conventions

* They remain **outside any grouping**
* They stay within the orbit
* They are typically placed further from the core

### Common Examples

* Identity & Access Management
* Payment Gateways
* Email & Notifications
* External Partners

These systems communicate enablement, not differentiation.

---

## 7. Connections and Flows

Connections are **optional visual elements** used to express **business-level flows of value or influence** between the Business Core and surrounding systems.

A connection **does not** represent:
- Technical integrations
- APIs or events
- Execution order
- System dependencies

The diagram remains valid **with or without connections**.

---

### Connection Semantics

A connection represents **how business information, decisions, or outcomes move or influence other systems**.

> **Connections describe business meaning, not system mechanics.**

---

### Allowed Connection Types

Only the following connection types are permitted:

- **Business Core → Orbit**  
  Indicates that the core produces information, decisions, or outcomes consumed by orbiting systems.

- **Orbit → Business Core**  
  Indicates that an orbiting system provides inputs that initiate or modify the core business state.

- **Orbit ↔ Orbit (restricted)**  
  Allowed only when the flow is essential to understanding the business narrative.  
  Excessive orbit-to-orbit connections should be avoided.

---

### Prohibited Connections

The following connections must **not** be represented:

- Connections involving **Cross-Cutting or External Systems**
- Connections between **internal components of the Business Core**
- Bidirectional connections used by default
- Dense or network-like connection patterns

If such relationships need to be explained, a **separate technical or integration diagram** should be used.

---

### Visual Guidance

- Connections should be visually simple
- No technical labels should be attached
- Connections should support the narrative, not dominate it

---

## 8. Color Usage

### Recommended Use

* Distinguish Build vs Buy vs External
* Highlight core vs supporting systems

### Avoid

* Excessive color coding
* Complex legends
* Color per system

Color should support the narrative, not dominate it.

---

## 9. What the Diagram Explicitly Avoids

The Enterprise Orbit Diagram is **not** intended to replace:

* BPMN diagrams
* Sequence diagrams
* Infrastructure diagrams
* Microservice maps
* Deployment views

If those details are required, complementary diagrams should be used.

---

## 10. Canonical Description

> *The Enterprise Orbit Diagram is a strategic visualization of enterprise software where proximity and grouping communicate business relevance rather than technical structure.*

---

These conventions define **version 1** of the Enterprise Orbit Diagram.
Future versions may expand visual patterns while preserving the core narrative principles.

## Method Evolution
