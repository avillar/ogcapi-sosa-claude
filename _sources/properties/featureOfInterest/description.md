## SOSA FeatureOfInterest Properties

This building block describes the canonical set of properties for a **FeatureOfInterest** object according to the SOSA/SSN specification.

A FeatureOfInterest is the thing whose property is being observed, acted upon, or sampled. It is an abstraction of a real-world phenomenon (e.g. a river, a building, an animal) to which a property of interest belongs.

A FeatureOfInterest can be expressed as:
- a reference (IRI or CURIE) to an externally defined feature, or
- an inline object with an `id` and optionally a set of associated properties (`hasProperty`).

These properties are independent of the feature model implementation — they may be included directly in a root JSON object or within the `properties` component of a GeoJSON feature.
