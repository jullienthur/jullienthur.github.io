# Projects

<hr>

## Single-Axis Linear Actuator & Trajectory Control System
**Timeline:** Aug 2025 - Dec 2025 | **Team Size:** 3 Members | **Links:** **[GitHub Repository](https://github.com/jullienthur/1ALA-TCS)**

**Core Technologies:** MATLAB Image Processing, C++, Inverse Kinematics, Serial Communication, State Machines

<details class="project-accordion">

<summary> View Project Details </summary>

<div class="accordion-content">

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

</div>

</details>

<hr>

## Submersible Water Pump
**Timeline:** Jan 2026 - Apr 2026 | **Team Size:** 3 Members

**Core Technologies:** SolidWorks, 3D Printing (PLA), GD&T

<details class="project-accordion">

<summary> View Project Details </summary>

<div class="accordion-content">

### Project Overview

Designed and fabricated a custom semi-submersible water pump tailored for low-flow applications. Conceived as a practical design exercise in Geometric Dimensioning and Tolerancing (GD&T), the primary objective was to ensure complete electronic isolation from the fluid while maximizing output.'

Through multiple physical iterations, our team successfully increased the flow rate from a baseline objective of 1 GPM up to **2.5 GPM**.

### Design & Engineering

+ **Drive Shaft & Gearbox:** The system is powered by a 3W motor running through a 1:7.72 gearbox, achieving a final average output of 72 RPM under load.

+ **Impeller Design:** Modeled custom centrifugal impellers in SolidWorks to optimize head pressure and flow rate. We utilized an enclosed impeller design, where the shrouds compensate for axial movement and mitigate pressure leakage within the two-part housing. The blades are backward-curved to increase endurance in a static pressure environment and reduce motor wear upon startup.

+ **Volute & Housing:** The volute follows a standard spiral profile, feeding into an outlet pipe capable of pulling water up a 1-meter head. The bottom piece extends around the impeller to accommodate potential shifting during sub-optimal working conditions.

<figure>
    <img src="assets/images/impeller-resource.jpg"
         alt="Types of Impeller">
</figure>
Figure 1: Different Impeller Designs reference
<div class="cad-viewer-container"> <model-viewer src="assets/impeller-preview.glb" loading="eager" alt="Interactive 3D Model of the Pump Assembly" auto-rotate camera-controls shadow-intensity="1" exposure="1.0"></model-viewer> </div>
Figure 2: Our Final Impeller Design
<div class="cad-viewer-container"> <model-viewer src="assets/top-case-preview.glb" loading="eager" alt="Interactive 3D Model of the Pump Assembly" auto-rotate camera-controls shadow-intensity="1" exposure="1.0"></model-viewer> </div>
Figure 3: Top Casing Design
<div class="cad-viewer-container"> <model-viewer src="assets/bottom-case-preview.glb" loading="eager" alt="Interactive 3D Model of the Pump Assembly" auto-rotate camera-controls shadow-intensity="1" exposure="1.0"></model-viewer> </div>
Figure 4: Bottom Casing Design


### Challenges & Optimization

The most significant issue we experienced was driveshaft whip, which caused excessive friction between the housing and the impeller. We solved this by designing and integrating two stabilizing brackets between the gearbox and the submerged pump section to ensure rigid, true rotation.

### Future Scope

While the current impeller design meets all performance criteria, future iterations will focus on the exterior housing. I plan to redesign the housing for a more ergonomic appearance, refine the internal volute geometry, and implement a streamlined adapter between the end volute and the outlet pipe.

</div>

</details>

<hr>

## My Portfolio Site!
**Timeline:** Mar 2026 - Present | **Links:** **[GitHub Repository](https://github.com/jullienthur/jullienthur.github.io)**

**Core Technologies:** HTML/CSS, JavaScript, Git/GitHub

<details class="project-accordion">

<summary> View Project Details </summary>

<div class="accordion-content">

So far, all you've seen has been part of this project! Check back for a run-down of how I built it and plan to maintain!

</div>

</details>

<hr>