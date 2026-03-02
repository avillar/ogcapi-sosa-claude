## SOSA Sensor Properties

This building block describes the canonical set of properties for a **Sensor** object according to the SOSA/SSN specification.

A Sensor is a device, agent (including humans), or software (simulation) that can generate Observations pertaining to an ObservableProperty by implementing an ObservingProcedure. Sensors respond to a stimulus — e.g., a change in the environment or input data — and generate a Result.

Sensor is a specialization of [SOSA System](../system/): it inherits all System properties (including `implements`, `hasSubSystem`, `isHostedBy`) and additionally provides:
- `observes` — the ObservableProperties this Sensor can observe

A Sensor can be expressed as:
- a reference (IRI or CURIE) to an externally defined sensor, or
- an inline object with an `id`, optional `name`, and optionally a list of subsystems or observed properties.

These properties are independent of the feature model implementation — they may be included directly in a root JSON object or within the `properties` component of a GeoJSON feature.
