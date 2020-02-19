# Introduction
MachUpX is an implementation of Phillips' numerical lifting-line algorithm with some small modifications to increase its accuracy and versatility. For reference on numerical lifting-line, see Phillips and Snyder "Modern Adaptation of Classic Lifting-Line Theory". The purpose of numerical lifting-line is to quickly and accurately model the aerodynamics of fixed-wing aircraft. Within the limitations of potential flow theory, this algorithm produces very accurate results without the computational overhead of higher-order methods, such as vortex lattice method or CFD.

MachUpX Has been built with both simple aerodynamic analysis and full-state flight simulation in mind. For the user simply wanting to analyze aerodynamics, the state of the aircraft can be specified in terms of alpha, beta, and velocity and forces, moments, aerodynamic derivatives, and span-wise distributions can be determined. For user's wanting to simulate flight, the state of the aircraft using a full 6-DOF state vector and forces and moments can be determined. In the case of flight simulation, the user will need to wrap a method for integrating Newton's 6-DOF dynamics equations around MachUpX, as this is not already provided.

Those users already familiar with previous versions of MachUp (Pro/4/5/Py) will find the interface with MachUpX to be similar. However, attempts have not been made to ensure compatibility between previous versions of MachUp and MachUpX. If the user wishes to use analysis scripts/input files from previous versions of MachUp with MachUpX, modifications will have to be made. For this reason, significant effort has been made to provide clear and thorough documentation for MachUpX.

Examples for using the MachUpX API/command line interface can be found in the examples/ directory of the source code.

Help on using MachUpX can be found at the MachUp discussion forum on [Google Groups](https://groups.google.com/forum/#!categories/machup_forum).