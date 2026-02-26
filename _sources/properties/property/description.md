## SOSA Property Properties

This building block describes the canonical set of properties for a **Property** object according to the SOSA/SSN specification.

A Property is an identifiable quality (property, characteristic) of a FeatureOfInterest that can be observed, acted upon, or sampled. Properties can be associated with different Features of Interest and may be used by one or more Procedures.

Specializations of Property include:
- **ObservableProperty** — a property that can be observed by a Sensor
- **ActuatableProperty** — a property that can be changed by an Actuator
- **SampledProperty** — a property whose value can be assessed by a Sampler

A Property can be expressed as:
- a reference (IRI or CURIE) to an externally defined property, or
- an inline object with an `id`, and optionally `isPropertyOf` (the associated FeatureOfInterest) and `hasProcedure` (Procedures that address this Property).

These properties are independent of the feature model implementation.
