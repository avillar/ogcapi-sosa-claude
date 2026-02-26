## SOSA ObservableProperty Properties

This building block describes the canonical set of properties for an **ObservableProperty** object according to the SOSA/SSN specification.

An ObservableProperty is an observable quality (property, characteristic) of a FeatureOfInterest. It is the characteristic that a Sensor is designed to estimate or calculate a value of, by implementing an ObservingProcedure.

An ObservableProperty can be expressed as:
- a reference (IRI or CURIE) to an externally defined property, or
- an inline object with an `id` and optionally a reference to the feature it belongs to (`isPropertyOf`).

ObservableProperty is a specialization of [SOSA Property](../property/).
