# CFD with Excel and Python

Solvers for fluid flow and heat transfer, written twice: once as a Microsoft Excel spreadsheet and once as a Python notebook. Each folder holds one case or one numerical scheme. The `README.md` in each folder explains the physics, the derivation and every solver step.

## How to use the files

Excel files open in Excel 2016 or later. Some 2D cases need iterative calculation, which is turned on under File, Options, Formulas; the settings for each case are written in its `Inputs` tab.

To run the notebooks on your own computer:

```
pip install -r requirements.txt
jupyter notebook
```

The notebooks also open in Google Colab without any installation.

## Folder layout

Each branch has its own folder, and each post folder has the same content:

```
Heat-transfer/
  Steady-conduction-rod/
    README.md
    Steady-conduction-rod.xlsx
    Steady-conduction-rod.ipynb
    figures/
```

## Posts

<!-- posts start -->

### Foundations

- [Conservation of mass](Foundations/Conservation-of-mass/)
- Conservation of momentum (Navier-Stokes)
- Conservation of energy
- Finite difference method
- Finite volume method
- Explicit time stepping
- Implicit time stepping
- The CFL condition

### Heat transfer

- 1D steady conduction in a rod
- 1D conduction with a heat source
- Fin with convection to air
- Radial conduction in a pipe wall
- 1D transient conduction in a slab
- 2D steady conduction in a plate
- 2D transient conduction in a plate
- 1D steady convection-diffusion
- 2D advection-diffusion of a Gaussian blob
- Upwind scheme
- Central scheme
- QUICK scheme

### Exact Navier-Stokes solutions

- Couette flow
- Plane Poiseuille flow
- Hagen-Poiseuille flow in a pipe
- Combined Couette-Poiseuille flow
- Flow in an annulus
- Liquid film on an inclined plane
- Taylor-Couette flow
- Stokes first problem
- Stokes second problem
- Start-up of channel flow
- Womersley pulsating pipe flow
- Taylor-Green vortex
- Kovasznay flow
- Lamb-Oseen vortex
- Hiemenz stagnation-point flow

### Pressure-velocity coupling

- Checkerboard pressure
- Staggered grid
- Rhie-Chow interpolation
- SIMPLE in 1D (nozzle)
- Channel flow by SIMPLE
- Lid-driven cavity by stream function-vorticity
- Projection method
- Lid-driven cavity by SIMPLE
- SIMPLEC
- PISO

### Shocks and schemes

- FTCS scheme
- FTBS (first-order upwind)
- Lax-Friedrichs scheme
- Lax-Wendroff scheme
- Beam-Warming scheme
- MacCormack scheme
- The modified equation
- Inviscid Burgers equation
- Conservative and non-conservative form
- Viscous Burgers equation
- Godunov method
- Quasi-1D nozzle with a shock
- Euler equations and the Sod tube
- Steger-Warming flux splitting
- Roe solver
- HLL solver
- HLLC solver
- MUSCL reconstruction
- Minmod limiter
- Van Leer limiter
- Superbee limiter
- WENO5 scheme
- Shu-Osher problem
- 2D Riemann problem
- Double Mach reflection
- Scheme comparison

### Benchmark flows

- Blasius boundary layer
- Developing flow in a channel
- Backward-facing step
- Flow past a cylinder
- Natural convection in a square cavity
- Rayleigh-Benard convection

### Verification

- Grid convergence and order of accuracy
- Method of manufactured solutions
<!-- posts end -->
