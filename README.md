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
A-heat-transfer/
  A01-steady-conduction-rod/
    README.md
    A01-steady-conduction-rod.xlsx
    A01-steady-conduction-rod.ipynb
    figures/
```

## Posts

<!-- posts start -->

### F · Foundations

- F01 · [Conservation of mass](F-foundations/F01-conservation-of-mass/)
- F02 · Conservation of momentum (Navier-Stokes)
- F03 · Conservation of energy
- F04 · Finite difference method
- F05 · Finite volume method
- F06 · Explicit time stepping
- F07 · Implicit time stepping
- F08 · The CFL condition

### A · Heat transfer

- A01 · [1D steady conduction in a rod](A-heat-transfer/A01-steady-conduction-rod/)
- A02 · 1D conduction with a heat source
- A03 · Fin with convection to air
- A04 · Radial conduction in a pipe wall
- A05 · 1D transient conduction in a slab
- A06 · 2D steady conduction in a plate
- A07 · 2D transient conduction in a plate
- A08 · 1D steady convection-diffusion
- A09 · 2D advection-diffusion of a Gaussian blob
- A10 · Upwind scheme
- A11 · Central scheme
- A12 · QUICK scheme

### B · Exact Navier-Stokes solutions

- B01 · Couette flow
- B02 · Plane Poiseuille flow
- B03 · Hagen-Poiseuille flow in a pipe
- B04 · Combined Couette-Poiseuille flow
- B05 · Flow in an annulus
- B06 · Liquid film on an inclined plane
- B07 · Taylor-Couette flow
- B08 · Stokes first problem
- B09 · Stokes second problem
- B10 · Start-up of channel flow
- B11 · Womersley pulsating pipe flow
- B12 · Taylor-Green vortex
- B13 · Kovasznay flow
- B14 · Lamb-Oseen vortex
- B15 · Hiemenz stagnation-point flow

### C · Pressure-velocity coupling

- C01 · Checkerboard pressure
- C02 · Staggered grid
- C03 · Rhie-Chow interpolation
- C04 · SIMPLE in 1D (nozzle)
- C05 · Channel flow by SIMPLE
- C06 · Lid-driven cavity by stream function-vorticity
- C07 · Projection method
- C08 · Lid-driven cavity by SIMPLE
- C09 · SIMPLEC
- C10 · PISO

### D · Shocks and schemes

- D01 · FTCS scheme
- D02 · FTBS (first-order upwind)
- D03 · Lax-Friedrichs scheme
- D04 · Lax-Wendroff scheme
- D05 · Beam-Warming scheme
- D06 · MacCormack scheme
- D07 · The modified equation
- D08 · Inviscid Burgers equation
- D09 · Conservative and non-conservative form
- D10 · Viscous Burgers equation
- D11 · Godunov method
- D12 · Quasi-1D nozzle with a shock
- D13 · Euler equations and the Sod tube
- D14 · Steger-Warming flux splitting
- D15 · Roe solver
- D16 · HLL solver
- D17 · HLLC solver
- D18 · MUSCL reconstruction
- D19 · Minmod limiter
- D20 · Van Leer limiter
- D21 · Superbee limiter
- D22 · WENO5 scheme
- D23 · Shu-Osher problem
- D24 · 2D Riemann problem
- D25 · Double Mach reflection
- D26 · Scheme comparison

### E · Benchmark flows

- E01 · Blasius boundary layer
- E02 · Developing flow in a channel
- E03 · Backward-facing step
- E04 · Flow past a cylinder
- E05 · Natural convection in a square cavity
- E06 · Rayleigh-Benard convection

### V · Verification

- V01 · Grid convergence and order of accuracy
- V02 · Method of manufactured solutions
<!-- posts end -->
