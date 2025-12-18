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

### Convention

* No arrows by default
* If arrows are used:

    * Keep them minimal
    * Use them narratively
    * Avoid exhaustive representations

The diagram favors **understanding over completeness**.

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
