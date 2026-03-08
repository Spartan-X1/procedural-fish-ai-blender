# Procedural Fish AI Simulation in Blender

This project demonstrates an autonomous fish AI system built in Blender
using Python. The system simulates natural fish movement using
procedural animation, steering behaviors, and environmental awareness.

The fish can navigate terrain, avoid obstacles, react to predators, and
follow targets while maintaining realistic swimming motion.

------------------------------------------------------------------------

## Features

-   Autonomous fish movement using a velocity-based steering system
-   Terrain awareness using raycasting
-   Obstacle avoidance using a forward radar system
-   Target seeking behavior
-   Predator avoidance behavior
-   Procedural skeletal swimming animation
-   Multi-state behavior system

Behavior states: - IDLING - SWIMMING - FLEEING - TURNING

------------------------------------------------------------------------

## Demo

A demonstration video is included in this repository showing:

-   autonomous navigation
-   terrain avoidance
-   predator fleeing
-   target following
-   procedural swimming animation

------------------------------------------------------------------------

## Requirements

Blender 5 or newer.

No additional dependencies are required.

------------------------------------------------------------------------

## How to Run

1.  Download the repository.
2.  Open `Cinematic_demo.blend` in Blender.
3.  Switch to the **Scripting** workspace.
4.  Select the script in the text editor.
5.  Click **Run Script**.
6.  Press **Play** on the timeline to start the simulation.

After running the script,select the armature(spine of the fish) a panel called **Fish AI** will appear in the
3D Viewport sidebar.

Press **N** to open the sidebar.

------------------------------------------------------------------------

## Fish AI Control Panel

The Fish AI panel allows you to:

-   Change the fish behavior state
-   Assign a target object (When target selected the panel is locked and nothing can be changed apart from removing the target)
-   Assign a predator object (When predator object is selected the panel is locked and nothing can be changed until far away from the predator)

Predator detection radius is approximately 50 meters.

------------------------------------------------------------------------

## Core Techniques Used

### Context Steering

The fish evaluates multiple possible movement directions and selects the
safest path based on: - target direction - obstacle proximity - terrain
collision risk

### Raycasting

Raycasts are used to detect: - terrain height - obstacles in front of
the fish

### Procedural Animation

The swimming motion is generated dynamically by applying sinusoidal
rotations to the fish bones.

### Multi-State Behavior System

Fish behavior is controlled using a state machine with different
behavioral modes.

------------------------------------------------------------------------

## Repository Structure

procedural-fish-ai-blender/ │ ├── Cinematic_demo.blend ├──
fish_ai.mp4 └── README.md

------------------------------------------------------------------------

## Author
Developed by Spartan-X1.
