# gazebo_contact_pkgs

Improved gazebo contact task simulation packages

Aimed to be a mujoco-like physics engine for Gazebo to improve its contact simulation.

Four ways to improve this thing:
- fix gazebo source code for support fine contact simulation, for example using DART and Simbody. DART support non-penetration, and Simbody support many contact models which can be used to compute the contact force rather than using impulse (Ft=mv).
- create new gazebo plugins for specific things
- improve the ODE engine and other existing physics engine
- create new physics engine


## Reference
- [simbody/simbody - High-performance C++ multibody dynamics/physics library for simulating articulated biomechanical and mechanical systems](https://github.com/simbody/simbody)
- [DART (Dynamic Animation and Robotics Toolkit)](https://dartsim.github.io/)
- [siconos/siconos - Simulation framework for nonsmooth dynamical systems](https://github.com/siconos/siconos)
- [siconos/gazebo-siconos](https://github.com/siconos/gazebo-siconos)
