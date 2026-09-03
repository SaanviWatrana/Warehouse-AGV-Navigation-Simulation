# 02 — PRD & Requirements Framework

> The original PRD file is not currently available in the workspace. This document records the requirements structure supported by the project use cases and architecture screenshots, without inventing unavailable implementation details.

## Product Problem

Warehouse robots must navigate constrained environments, reach assigned destinations and respond safely when static or moving obstacles affect the planned route.

## Product Goal

Define and validate a navigation workflow in which an AGV/AMR can sense its environment, perceive obstacles, plan a path, avoid collisions and execute warehouse tasks.

## Functional Requirements

1. The system shall acquire LiDAR/environment data.
2. The system shall detect relevant obstacles.
3. The system shall update its environmental representation.
4. The system shall track moving obstacles.
5. The system shall generate a navigation path.
6. The system shall support collision-avoidance behaviour.
7. The robot shall navigate toward an assigned destination.
8. The system shall support pick and drop task actions.
9. The system shall support task assignment.
10. The navigation workflow shall account for changing warehouse conditions.

## Non-Functional Considerations

- Safety should take precedence over nominal path efficiency.
- Navigation decisions should be decomposed into understandable system layers.
- Dynamic conditions should be observable and handled through re-planning.
- Product requirements should remain traceable to system components.

## Traceability

```text
Use Case
   ↓
Functional Requirement
   ↓
Functional Layer
   ↓
System Component
   ↓
Simulation Scenario
```
