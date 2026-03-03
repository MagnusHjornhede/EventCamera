# Event-Based Object Tracking with Dynamic Vision Sensors

## Project Description

This project implements an object tracking pipeline using event-based data from a Dynamic Vision Sensor (DVS). Unlike conventional frame-based cameras, event cameras asynchronously output brightness-change events with microsecond temporal resolution.

The goal of the project is to:

* Process raw event streams
* Convert asynchronous events into structured representations
* Perform object localization and tracking over time
* Evaluate tracking performance under controlled experimental conditions

The implementation is contained in:

```
ObjectTrackingWithEventCamera.ipynb
```

## Core Concept

Each event consists of:

[
(x, y, t, p)
]

where:

* (x, y) = pixel coordinates
* (t) = timestamp
* (p) = polarity

Events are aggregated into temporal windows and transformed into grid-based representations suitable for tracking algorithms.

## Objective

The system investigates how event representations and temporal aggregation strategies affect tracking accuracy, stability, and latency.

