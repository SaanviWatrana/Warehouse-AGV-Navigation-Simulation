# 01 — Use Cases

## Actors

### Warehouse Operator
Supervises the navigation process and interacts with warehouse-level tasks.

### LiDAR Sensor
Supplies environmental sensing data used for obstacle detection, tracking and map updates.

### Warehouse Management System
Provides warehouse context and task-related interactions.

### Autonomous Mobile Robot (AMR)
Performs navigation and material-handling actions inside the warehouse.

## Core Use Cases

| Use case | Purpose |
|---|---|
| Read LiDAR Data | Acquire range/environment data |
| Detect Obstacles | Identify objects that affect navigation |
| Update Map | Maintain an updated representation of the environment |
| Track Moving Obstacles | Estimate the changing position of dynamic obstacles |
| Plan Path | Generate a route toward the destination |
| Avoid Collision | Modify/stop motion when collision risk exists |
| Navigate to Destination | Execute the planned movement |
| Pick Item | Perform a warehouse pickup action |
| Drop Item | Perform a warehouse drop action |
| Assign Task | Associate a warehouse task with the robot |

## Functional Relationship

The use cases establish the product behaviour that the later functional and system architecture decomposes into sensing, perception, planning, control/safety and robot execution layers.
