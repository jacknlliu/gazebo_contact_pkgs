# gazebo_contact_pkgs

Improved gazebo contact task simulation packages

Aimed to be a mujoco-like physics engine for Gazebo to improve its contact simulation.

There are many contact task in robotic simulation, for example, peg-in-hole, insert CPU and 3C products, and many robotic assembly tasks. 

> Accurate and fast simulation of contact dynamics is crucial for model based control of robots since the robots interact with environments by the contact force.
> Solving contact dynamics is NP-hard problem[1] due to its non-convexity and discontinuity. To make the problem tractable, physics engines approximate the contact problem as a relaxed problem that enables using efficient solving methods. Each method has different characteristics, but some of them significantly sacrifice the accuracy of the contact solution that leads to the poor reality of the simulation. —— From [SimBenchmark wiki](https://leggedrobotics.github.io/SimBenchmark/)

Four ways to improve this thing:
- fix gazebo source code for support fine contact simulation, for example using DART and Simbody. DART support non-penetration, and Simbody support many contact models which can be used to compute the contact force rather than using impulse (Ft=mv).
- create new gazebo plugins for specific things
- improve the ODE engine and other existing physics engine
- create new physics engine


## Reference
- [1] D. Kaufman et al., “Staggered projections for frictional contact in multibody systems,” 2008.
- [Contact Models and Multibody Dynamics](https://leggedrobotics.github.io/SimBenchmark/about/models.html)
- [SimBenchmark wiki](https://leggedrobotics.github.io/SimBenchmark/)
- [SimBenchmark](https://github.com/leggedrobotics/SimBenchmark)
- [quantifying-the-reality-gap-in-robotic-manipulation-tasks](https://github.com/erwincoumans/quantifying-the-reality-gap-in-robotic-manipulation-tasks)
- [simbody/simbody - High-performance C++ multibody dynamics/physics library for simulating articulated biomechanical and mechanical systems](https://github.com/simbody/simbody)
- [DART (Dynamic Animation and Robotics Toolkit)](https://dartsim.github.io/)
- [siconos/siconos - Simulation framework for nonsmooth dynamical systems](https://github.com/siconos/siconos)
- [siconos/gazebo-siconos](https://github.com/siconos/gazebo-siconos)
