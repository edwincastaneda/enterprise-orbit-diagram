# Enterprise Orbit Diagram

![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey)
![Canonical](https://img.shields.io/badge/model-canonical%20v1-blue)
![Status](https://img.shields.io/badge/status-RC-yellow)


![EOD](https://github.com/user-attachments/assets/4ca74126-b95a-49b2-a1db-1c312473bbc7)


The Enterprise Orbit Diagram is a strategic visualization model designed to help organizations understand, communicate, and reason about their software assets around a central business core.

The diagram is explicitly concerned with **business identity**, not system design.

Its primary question is not how systems are built or connected, but **which systems define who the organization is**, and which merely enable its operation.

It is especially useful in early discovery phases, low-documentation environments, and modernization initiatives where existing system landscapes are complex, fragmented, or poorly understood.


## What problem does it solve?

Many organizations struggle to explain their technology landscape in a way that is understandable to both business and technical stakeholders.

Existing documentation is often:
- Too technical for non-technical audiences
- Outdated or incomplete
- Scattered across multiple tools and formats

The Enterprise Orbit Diagram provides a single, business-centric view of enterprise software assets, enabling clearer conversations and better strategic decisions.

By grounding the conversation in business meaning rather than technology, the Enterprise Orbit Diagram enables clearer strategic discussions, challenges false assumptions of criticality, and supports better decision-making at executive level.


## What is the Enterprise Orbit Diagram?

The diagram represents enterprise systems as elements orbiting a central business core.

- The core represents the most critical business domain or capability. The Business Core is always singular and represents the irreducible capability without which the organization would no longer recognize what it sells.
- Orbiting elements represent supporting, adjacent, or external software systems.
- Visual distance and grouping help communicate relevance, dependency, and strategic importance. Distance is never aesthetic: it conveys coupling strength, replacement cost, and long-term strategic weight.

## Guide & Documentation

- 📐 [Diagram conventions](docs/conventions.md)

## When to use it

- Enterprise discovery and assessment
- Modernization and legacy transformation discussions
- Executive and stakeholder presentations
- Alignment between business and technology teams
- Early documentation in low-maturity environments


## What it is NOT

The Enterprise Orbit Diagram is not:
- A detailed system design or architecture specification
- A replacement for technical diagrams (e.g. sequence, component, or deployment diagrams)
- A workflow or BPMN model

Its purpose is strategic clarity, not technical precision.

If a representation can be interpreted as a technical architecture diagram, it has crossed the boundary of the Enterprise Orbit Diagram and no longer fulfills its purpose.

--

> The Enterprise Orbit Diagram is a strategic narrative tool.  
> Clarity of meaning always takes precedence over technical completeness.


## Example

Here is a basic example of an Enterprise Orbit Diagram, including its standard nomenclature and canvas layout.

- 🧭 [Canonical example](docs/examples.md)
- 🧩 **More Examples (Coming Soon)**

Additional canonical and exploratory examples will be published over time.

_If you have a proposal for a new Enterprise Orbit Diagram example, you can either open a Pull Request or reach out at **winedcasta@hotmail.com**._

## Resources

- [Excalidraw File](resources/enterprise-orbit-diagram-canvas.excalidraw) _Restore the previous version via file import._
- [Excalidraw URL](https://excalidraw.com/#json=C-BxLuszQGlaYd_wDymgN,aA4d9FqIyXrmkjobVhAnLg) _Warning: Previous work in Excalidraw may be overwritten._
- [Miro Template](https://miro.com/miroverse/enterprise-orbit-diagram-template/?social=copy-link)

## Status

This project documents a visualization pattern that has been applied in real-world enterprise initiatives.

The repository is intentionally lightweight and focused on:
- Explaining the model
- Defining clear diagramming conventions
- Sharing examples and guidance

Community feedback and contributions are welcome.

## Author

Created and maintained by [Edwin Castañeda](https://gt.linkedin.com/in/edwincasta).

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

You are free to use, adapt, and share this model, provided appropriate credit is given to the original author.
