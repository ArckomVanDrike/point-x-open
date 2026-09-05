# Architecture

Point X separates spatial logic from the client that renders it.

~~~text
Sensors
  |
  v
Point X Core
  |
  +-- Target state
  +-- Trace state
  +-- Beacon state
  |
  +-- Web / PWA
  +-- Native App
  +-- Widgets
  +-- Watches
  +-- Wearables
  +-- Smart Glasses / HUD
~~~

The core is intended to remain independent from browser, phone, watch or wearable UI.

Clients provide the sensor data available on their platform and consume standardized navigation state.

## Design goals

- Mapless navigation as the default interaction
- Portable core logic
- Graceful handling of missing sensors
- Explicit positioning confidence
- No false arrival confirmation
- Support for low-attention interfaces
- Compatibility with richer native sensor stacks
