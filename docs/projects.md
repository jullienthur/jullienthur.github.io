# Projects
---
## Single-Axis Linear Actuator & Control System
**Timeline:** Aug 2025 - Dec 2025 | **Team Size:** 3 Members | Links: **[GitHub Repository](https://github.com/jullienthur/1ALA-TCS)**

**Core Technologies:** MATLAB Image Processing, Arduino C, Inverse Kinematics, Serial Communication, State Machines

### Project Overview

Developed a high-speed control system integrating MATLAB and C++ to operate an automated, solenoid-actuated cannon mounted on a single-axis linear rail. The system was designed to autonomously track, target, fire at six pre-specified locations, and reload between each shot.

Through rigorous software optimization and hardware coordination, our team reduced the total execution time from a baseline goal of 100 seconds down to just 45 seconds—**a 55% improvement**.


### System Architecture & Data Pipeline

The system relies on a seamless bi-directional serial communication loop between high-level processing and low-level hardware control:

+ **Vision & Processing:** MATLAB handles the image processing to identify and extract the spatial coordinates of visual targets. This is done through a simplified map of the cannon's surroundings and a color-filter array to identify targets.

+ **Hardware Execution:** This data is fed to the Arduino-based kinematics engine, which translates the coordinates into linear movements and ballistic trajectories.


### Key Optimizations

The final weeks of the project were focused solely upon optimization; the process scaffolding had been finalized. During these weeks, we focused on two things:


+ **Pathfinding Algorithm:** Engineered the software to dynamically sort the engagement sequence of targets based on their spatial proximity to the fixed reloading station, minimizing unnecessary travel distance.

+ **Concurrent Execution:** Wrote custom, non-block state machines in C++. This allowed the system to operate the reloading mechanism and the linear positioning motor simultaneously, effectively eliminating standard process delays and idle time.

### Reflection & Future Scope

While efficient, the current iteration relies on a "stop-and-shoot" mechanism, where the cannon halts at the optimal point on the rail before firing.

If I were to develop a second version, I would implement a dynamic firing system. By utilizing advanced kinematics, the system could calculate the exact firing vector required to shoot *while* in motion. Utilizing the actuator's lateral momentum to curve the ball's trajectory would allow for continuous movement, further slashing the overall cycle time.

## Submersible Water Pump


I'm currently working on updating this project. Please check back a little later to see the finished result!


## My Portfolio Site!

So far, all you've seen has been part of this project! Check back for a small run-down of how I built it and plan to maintain!