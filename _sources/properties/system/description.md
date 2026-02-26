## SOSA System Properties

This building block describes the canonical set of properties for a **System** object according to the SOSA/SSN specification.

A System is a unit of abstraction for pieces of infrastructure that implement Procedures. A System may be a physical device, a network of devices, a software agent, or any other entity capable of implementing a Procedure. Systems may have subsystems, may implement multiple Procedures, and may be hosted by Platforms.

Specializations of System include:
- **Sensor** — a System that observes properties
- **Actuator** — a System that changes the state of the world
- **Sampler** — a System that creates Samples

A System can be expressed as:
- a reference (IRI or CURIE) to an externally defined system, or
- an inline object with an `id` and optionally:
  - `name` — a human-readable name
  - `implements` — the Procedures implemented by this System
  - `hasSubSystem` — component subsystems
  - `isSubSystemOf` — the parent system
  - `isHostedBy` — the Platform hosting this System

These properties are independent of the feature model implementation. For sensor-specific properties, use the [SOSA Sensor](../sensor/) building block.
