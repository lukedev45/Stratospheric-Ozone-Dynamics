# Stratospheric Ozone Dynamics  
_Repository for modelling stratospheric ozone dynamics using the Chapman mechanism and altitude-dependent rate constants._
## Project Overview  
This project implements a computational model of stratospheric ozone dynamics by numerically solving the coupled chemistry-transport equations based on the Chapman mechanism for ozone (O₃) formation and destruction.  
In this version, the model incorporates altitude-dependent reaction rate constants and diurnal (and potentially latitudinal) variations. The aim is to simulate how ozone concentration profiles evolve in the stratosphere over time and how they respond to changes in parameters (e.g., photolysis rates, height-dependent kinetics).

## Motivation  
Understanding ozone dynamics in the stratosphere is crucial because ozone plays a key role in absorbing harmful UV radiation and in atmospheric chemistry and climate. The Chapman mechanism provides a foundational description of ozone chemistry. By extending the model to include altitude-dependence and numerical methods for partial difference equations (similar in spirit to your earlier heat-distribution work), the project aims to:  
- Allow exploration of sensitivity to rate‐constant profiles and photolysis parameterisations.  
- Serve as a learning tool (for yourself) linking your work on atmospheric modelling (e.g., stratospheric ozone, Chapman mechanism) to computational methods.  
- Produce a flexible framework that could be extended (e.g., incorporate heterogeneous chemistry, multi-dimensional transport, catalytic cycles).  

## Features  
- Implementation of the Chapman ozone reactions (O₂ + hv → 2 O, O + O₂ + M → O₃ + M, O₃ + hv → O₂ + O, O + O₃ → 2 O₂)  
- Altitude‐dependent reaction rate constants and/or photolysis rates  
- Use of a one-dimensional vertical grid for the stratosphere (height vs concentration)  
- Time‐stepping via an explicit Euler (or more stable method) scheme  
- Output of ozone concentration profiles over time and height  
- Plotting routines (e.g., via matplotlib) to visualise results  
- Modular code structure so that new reaction terms or transport terms can be added  
