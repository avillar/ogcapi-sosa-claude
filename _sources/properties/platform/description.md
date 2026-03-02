## SOSA Platform Properties

This building block describes the canonical set of properties for a **Platform** object according to the SOSA/SSN specification.

A Platform is an entity that hosts other Assets, in particular Systems such as Sensors. A Platform may host multiple Sensors or other Systems, and may itself be hosted by another Platform (e.g. a satellite hosting an instrument, which in turn is mounted on a spacecraft).

The key property of a Platform is:
- `hosts` — an array of hosted Systems (Sensors, Actuators, etc.) or nested Platforms

A Platform can be expressed as:
- a reference (IRI or CURIE) to an externally defined platform, or
- an inline object with an `id` and a list of hosted entities.

These properties are independent of the feature model implementation — they may be included directly in a root JSON object or within the `properties` component of a GeoJSON feature.
