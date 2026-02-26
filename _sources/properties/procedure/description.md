## SOSA Procedure Properties

This building block describes the canonical set of properties for a **Procedure** object according to the SOSA/SSN specification.

A Procedure is a workflow, protocol, plan, algorithm, or computational method specifying how to make an Observation, create a Sample, or make a change to the state of the world via an Actuator. A Procedure is reusable and may be implemented by multiple Systems.

A Procedure can be expressed as:
- a reference (IRI or CURIE) to an externally defined procedure, or
- an inline object with an `id` and optionally:
  - `implementedBy` — the Systems that implement this Procedure
  - `hasInput` / `hasOutput` — the inputs and outputs of the Procedure
  - `isProcedureFor` — the Properties this Procedure can be used to observe or act upon

These properties are independent of the feature model implementation.
