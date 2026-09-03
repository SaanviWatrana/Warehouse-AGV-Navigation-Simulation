# 04 — System Architecture

## High-Level Boundary

```text
┌──────────────────────────────┐
│ Warehouse / External Context │
│ WMS • Operator • Tasks       │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│       Navigation Stack       │
│ Sensing → Perception         │
│ → Planning → Control/Safety  │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│       Robot Execution        │
│ Motors • Steering • Actuators│
└──────────────────────────────┘
```

## Data Flow

1. Sensors observe the warehouse.
2. Perception processes the observations.
3. Obstacle and map state are updated.
4. Planning generates or revises a route.
5. Control and safety evaluate motion.
6. Robot hardware executes the task.
7. Robot/environment state feeds back into the navigation loop.

## External Interfaces

The Figma system view identifies interactions with:

- Warehouse Management System
- Operator interfaces
- Monitoring and analytics
- Maintenance / diagnostics

This repository documents these as architectural boundaries; it does not claim a live integration with those systems.
