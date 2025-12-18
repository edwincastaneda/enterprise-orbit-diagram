# Enterprise Orbit Diagram — Examples

This document provides **illustrative examples** of how to apply the Enterprise Orbit Diagram (EOD) conventions in real-world contexts.

The purpose of these examples is not to prescribe a single correct diagram, but to demonstrate **how narrative intent is translated into visual structure**.

---

## Example 1: Core Business Platform

### Context

An organization whose primary value lies in managing and operating a core business platform.

### Business Core

* **Core Business Platform**

This represents the main domain capability that differentiates the company.

### Orbiting Systems

* CRM
* ERP
* Data & Analytics Platform
* Document Management System

These systems are positioned closer to the core because they directly support and shape the primary business capability.

### Cross-Cutting Systems (Not Grouped)

* Identity & Access Management
* Email & Notifications
* Payment Gateway
* External Partners

These systems enable operations but do not define the business model. They remain ungrouped and positioned further from the core.

### Narrative Outcome

The diagram quickly communicates which systems are **strategic**, which are **supporting**, and which are **enabling but replaceable**.

---

## Example 2: Workflow-Oriented Grouping

### Context

An enterprise with a clearly defined end-to-end business workflow.

### Business Core

* **Primary Business Domain**

### Grouped Systems (Workflow Narrative)

A dashed or dotted grouping highlights systems that participate in a shared workflow, for example:

* Intake System
* Validation Engine
* Case Management System
* Decision Support Module

The grouping communicates a business process **without modeling it explicitly**.

### Ungrouped Systems

* Identity & Access Management
* Notifications
* External Integrations

These remain outside the grouping to avoid overloading the diagram with technical or transversal concerns.

### Narrative Outcome

Stakeholders understand *where value flows* without requiring BPMN or sequence diagrams.

---

## Example 3: Modernization Scenario

### Context

An organization assessing modernization or transformation opportunities.

### Visual Cues

* Legacy systems placed further from the core
* Modern or strategic systems positioned closer
* External or SaaS solutions clearly identified

### Narrative Outcome

The diagram supports conversations such as:

* What systems are candidates for replacement?
* Which capabilities must be protected?
* Where does modernization deliver the most value?

---

## Key Takeaway

> The Enterprise Orbit Diagram is most effective when used as a **conversation artifact**, not as a definitive architectural blueprint.

Multiple diagrams may coexist for the same organization, each telling a different strategic story.
