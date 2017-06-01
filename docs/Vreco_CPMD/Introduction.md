# Vreco_CPMD

Get the code [here](https://github.com/NNairIITK/Vreco_CPMD).

## Description

This program is useful for reconstructing the free energy surface from a
metadynamics simulation using CPMD. There is no limitation on the number of
collective variables (CV) the program can handle. For runs with 1 (2) CVs, the
2D (3D) reconstructed free energy surfaces, can be viewed in GNUPLOT or
OpenDX. For a 3 CV case, it is possible to print the 4D free energy surface in
a cube file format (for e.g., then using VMD/OpenDX to visualize). See the
example directory for examples to plot and visualize the data.

Important to note that, $F(s)$ , the free energy in collective variable space, is
printed, where

$$
F(s) = - SUM\_t\times V(t,s).
$$

Here $V$ is the biasing potential added at time $t$ in the collective variable
space $s$.