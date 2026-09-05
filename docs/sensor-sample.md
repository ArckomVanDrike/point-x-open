# Sensor Sample

Point X uses a portable sensor contract so different clients can provide different levels of information.

Conceptual model:

~~~js
{
  latitude,
  longitude,
  horizontalAccuracy,
  altitude,
  verticalAccuracy,
  heading,
  speed,
  timestamp
}
~~~

A web client may provide only a subset of these values.

A native application may provide richer positioning and motion information.

The core should not depend on the origin of the sensor data.
