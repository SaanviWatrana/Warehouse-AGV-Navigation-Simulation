# 03 — Functional Architecture

The functional architecture separates warehouse navigation into six responsibilities.

## 1. Environment Layer
Represents the warehouse operating context: warehouse space, shelves, robots, goal areas and forklifts.

## 2. Sensing Layer
Collects environmental and robot-state information through LiDAR, IMU, wheel encoders and safety sensors.

## 3. Perception Layer
Transforms sensor information into a representation usable by navigation logic.

Components shown in the design:
- LiDAR Data Reader
- Point Cloud Processing
- Obstacle Detection
- Tracking / Moving-Obstacle Handling
- Map Update / SLAM

## 4. Planning Layer
Determines how the robot should reach its destination.

Components shown in the design:
- Global Path Planner
- Local Path Planner
- Path Optimization
- Dynamic Re-planning

## 5. Control & Safety Layer
Converts navigation decisions into controlled motion and provides safety responses.

Components shown in the design:
- Velocity / Motor Controller
- Collision Avoidance
- Emergency Stop

## 6. Robot Layer
Represents physical execution:
- Drive Base / Motors
- Steering System
- Actuators
- Task Execution

## Architectural Principle

Each layer has a distinct responsibility, allowing the product requirements to be mapped to system behaviour without collapsing sensing, planning and physical execution into one component.
