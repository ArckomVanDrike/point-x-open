<img width="1672" height="941" alt="point-x-readme-hero" src="https://github.com/user-attachments/assets/ef5ee3c4-066b-4b6d-90a7-194ce01e6636" />
# Point X

**Navigation without the map.**

Point X is a spatial navigation platform built around digital beacons.

Instead of showing you everything around you, Point X focuses on one simple question:

> Where is the thing that matters to me?

A Point X beacon can represent a car, a refuge, a campsite, a meeting point, a checkpoint, a trail marker, a public landmark, or any other location worth finding again.

## Core idea

Point X separates navigation from maps.

A map may be useful for planning and organizing locations, but active navigation can often be reduced to:

- direction
- distance
- confidence
- arrival state

This makes Point X suitable for phones, widgets, watches, wearables, smart glasses and other low-attention interfaces.

## Core concepts

### Drop X

Save a location as a personal beacon.

### Follow X

Follow a saved beacon using direction and distance.

### Reach X

Confirm arrival only when positioning confidence is sufficient.

### Trace X

Record a path as a sequence of stabilized spatial breadcrumbs.

### Beacon Sequence

Follow a sequence of beacons where reaching one can activate the next.

## Beacon visibility

Point X is designed to support:

- Private
- Shared
- Public
- Official / Verified
- Temporary

## Possible beacon behaviors

A beacon may eventually act as:

- Navigation target
- Checkpoint
- Information point
- Achievement
- Puzzle / clue
- Route step
- Safety point
- Temporary meeting point

## Cross-platform architecture

Point X is being designed around a shared core rather than a single client.

~~~text
Point X Core
    |
    +-- Web / PWA
    +-- Native App
    +-- Phone Widgets
    +-- Watches
    +-- Wearables
    +-- Smart Glasses / HUD
~~~

The same navigation state can therefore be rendered differently depending on the device.

## Public architecture

The current public model includes:

- [Architecture](docs/architecture.md)
- [Beacon Model](docs/beacon-model.md)
- [Sensor Sample](docs/sensor-sample.md)
- [Target Snapshot](docs/target-snapshot.md)
- [Roadmap](docs/roadmap.md)

## Status

Point X is currently under active early development.

The main implementation, sensor-fusion algorithms and native platform work are currently developed privately.

This repository documents the public architecture, concepts and interoperability model.

Interfaces described here may still change before Point X Core v1.

## Philosophy

> The beacon is the platform.  
> The map is only an editor.

Point X began as a small location experiment in 2023 and is now being rebuilt around a more focused idea: simple, portable spatial navigation.
