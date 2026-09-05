# Target Snapshot

A Target Snapshot represents the current navigation state for a selected beacon.

Conceptual model:

~~~js
{
  targetId,
  targetName,
  distanceMeters,
  bearingDegrees,
  relativeBearingDegrees,
  status,
  confidence,
  arrivalRadiusMeters,
  updatedAt
}
~~~

This allows the same navigation state to be rendered by:

- a web interface
- a native app
- a phone widget
- a watch
- smart glasses
- another compatible client

The UI is a consumer of navigation state, not the owner of navigation logic.
