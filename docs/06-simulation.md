# 06 — Simulation

## Simulation Objective

The project used a Python/Pygame simulation to explore warehouse AGV navigation behaviour in a visual 2D environment.

## Environment Model

The documented scenario includes:

- Static shelves / warehouse structures
- AGV navigation space
- Dynamic forklifts / moving obstacles
- Destination/task locations

## Behavioural Scenarios

### Scenario A — Clear Route
The AGV receives a destination and follows a valid navigation route through the warehouse.

### Scenario B — Static Obstacle
A shelf or fixed warehouse object constrains the available path and must be treated as non-traversable space.

### Scenario C — Dynamic Obstacle
A forklift enters or crosses the planned route. The navigation workflow must detect the changing condition and support avoidance/re-planning.

### Scenario D — Destination / Task
The AGV reaches its target location and supports the corresponding warehouse action such as pickup or drop-off.

## Technology Context

- Python
- Pygame
- VS Code

> The original simulation source files are not currently available to attach to this repository. This document therefore records the verified simulation scope rather than fabricating source code.
