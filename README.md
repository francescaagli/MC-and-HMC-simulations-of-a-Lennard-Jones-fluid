# Monte Carlo and Hybrid Monte Carlo simulations of a Lennard-Jones fluid

## Project description
Here I simulated a 3-dimentional Lennard-Jones fluid, more precisely Argon. I used at first a regular Monte Carlo algorithm, and then a slightly more complex Hybrid Monte Carlo algorithm. The simulation was made in the canonical ensemble and using periodic boundary conditions. The energy and the pressure were the quantities analyzed, as well as the acceptance rate.

The first simulation performed is a simple Monte Carlo simulation where at each step the configurations were sampled changing the position of a random particle.

Then I considered a variation of this algorithm by performing an Hybrid Monte Carlo simulation. The moves were not chosen randomly anymore but were taken from a velocity Verlet integrator and then accepted or rejected according to the Metropolis criterion. This type of simulation is something in between a Monte Carlo method and a Molecular Dynamics one.

The two different simulations gave very similar results in all the quantities. The main differences were in the convergence time and the acceptance rate. Using the simple Monte Carlo simulation the moves were random resulting in an higher convergence time and in a lower acceptance rate, while using the Hybrid Monte Carlo simulation the moves followed the natural time evolution of the system resulting in a lower convergence time and in an higher acceptance rate.

## Repository files

- `MC_HMC.ipynb` – Jupyter notebook.
- `MC_HMC.html` – HTML version of the notebook.

