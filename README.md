# A time dependent phase space filter for anisotropic wave equations on unbounded domains

## Overview

This project contains numerical simulations for two different physical models:

1. **Euler equations in a subsonic flow** (euler\_exact.py)
2. **Maxwell equations in an orthotropic medium** (maxwell\_orthotropic\_exact.py)

Both simulations use Fourier transforms (FFT) for efficient computations and store simulation frames for visualization.

## Features

- Implements numerical solutions for Euler and Maxwell equations.
- Uses Fourier transforms (FFT) for efficient computation.
- Supports diagonalization of Hamiltonian matrices.
- Saves wavefield data frames for further analysis.

## Prerequisites

Make sure you have the following dependencies installed:

- Python 3.x
- NumPy
- SciPy
- Matplotlib

You can install them using:

```bash
pip install numpy scipy matplotlib
```

## Project Structure

```
...
├── euler_exact.py  # Euler equation simulation
├── maxwell_orthotropic_exact.py  # Maxwell equation simulation
├── utils.py  # Utility functions 
├── tdpsf.py  # Additional computations 
├── README.md  # Project documentation
```

## How to Run

1. Clone this repository:

```bash
git clone <repo_link>
cd <repo_name>
```

2. Run the desired simulation:

```bash
python euler_exact.py  # For Euler equations
python maxwell_orthotropic_exact.py  # For Maxwell equations
```

3. The simulation data will be stored in the respective folder:
   - `euler_subsonic_exact_<freq>_plots/`
   - `maxwell_orthotropic_exact_<freq>_plots/`

<!-- ## Simulation Details

### Euler Subsonic Flow Simulation

- **Grid Size:** 2048 x 2048
- **Spatial Step (dx):** 0.125
- **Time Step (dt):** 2.0
- **Total Time:** 50
- **Mach Number:** 0.1
- **Wave Frequency:** 10.0

### Maxwell Orthotropic Medium Simulation

- **Grid Size:** 2048 x 2048
- **Spatial Step (dx):** 0.125
- **Time Step (dt):** 2.0
- **Total Time:** 50
- **Anisotropy Parameter (b):** 0.25
- **Wave Frequency:** 10.0 -->

## Output

Each simulation outputs data frames stored in `frameXXXXXX.dat` format in its respective simulation directory. These files contain real-valued wavefield data for analysis and visualization.

## License

This project is open-source and available under the MIT License.

