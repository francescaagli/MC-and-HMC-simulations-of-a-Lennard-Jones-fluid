# Monte Carlo and Hybrid Monte Carlo simulations of a Lennard-Jones fluid

## Project description
This project simulates a 3-dimentional Lennard-Jones fluid, more precisely Argon. At first a regular Monte Carlo algorithm is used, and then a slightly more complex Hybrid Monte Carlo algorithm. The simulation is made in the canonical ensemble and using periodic boundary conditions. The energy and the pressure are the quantities analyzed, as well as the acceptance rate.

The first simulation performed is a simple Monte Carlo simulation where at each step the configurations are sampled changing the position of a random particle.

Then a variation of this algorithm is considered by performing an Hybrid Monte Carlo simulation. The moves are not chosen randomly anymore but taken from a velocity Verlet integrator and then accepted or rejected according to the Metropolis criterion. This type of simulation is something in between a Monte Carlo method and a Molecular Dynamics one.

The two different simulations give very similar results in all the quantities. The main differences are in the convergence time and the acceptance rate. Using the simple Monte Carlo simulation the moves are random resulting in an higher convergence time and in a lower acceptance rate, while using the Hybrid Monte Carlo simulation the moves followed the natural time evolution of the system resulting in a lower convergence time and in an higher acceptance rate.

## Repository files

- `MC_HMC.ipynb` – Jupyter notebook.

