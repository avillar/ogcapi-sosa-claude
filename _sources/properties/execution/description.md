## SOSA Execution Properties

This building block describes the canonical set of properties for an **Execution** object according to the SOSA/SSN specification.

An Execution is an act of carrying out a Procedure by a System on or about a FeatureOfInterest, with the objective of producing a Result. Execution is the common abstract class for:
- **Observation** — estimating a value of a property of a FeatureOfInterest
- **Actuation** — changing the state of the world
- **Sampling** — creating a Sample of a FeatureOfInterest

All executions share the following properties:
- `hasFeatureOfInterest` / `hasUltimateFeatureOfInterest` — the target feature
- `usedProcedure` — the procedure applied
- `madeBySystem` — the system that performed the execution
- `hasResult` / `hasSimpleResult` — the result produced
- `resultTime` — when the result was produced
- `phenomenonTime` — the time the phenomenon being estimated occurred
- `startTime` / `endTime` — the temporal extent of the execution

These properties are independent of the feature model implementation. For observations specifically, use the [SOSA Observation Properties](../observation-owa/) building block, which adds `observedProperty` and `madeBySensor`.
