# 05 — Navigation Workflow

## End-to-End Flow

```text
Task Assigned
     ↓
Destination Identified
     ↓
Read LiDAR / Sensor Data
     ↓
Perception
     ├── Obstacle Detection
     ├── Moving-Obstacle Tracking
     └── Map Update
     ↓
Global Path Planning
     ↓
Local Path Planning
     ↓
Path Optimization
     ↓
Collision-Risk Check
     ↓
┌──────────────────────────┐
│ Safe to Continue?        │
└──────────┬───────────────┘
     Yes ↓       ↓ No
   Execute       Re-plan / Avoid
      ↓              ↓
      └──────→ Continue Navigation
                    ↓
              Reach Destination
                    ↓
             Pick / Drop Task
```

## Dynamic Obstacle Scenario

A forklift can change the free space after a path has already been generated. The navigation design therefore includes moving-obstacle tracking and dynamic re-planning rather than relying only on a fixed route.

## Safety Behaviour

Collision avoidance and emergency-stop behaviour form a dedicated control/safety responsibility between navigation planning and robot execution.
