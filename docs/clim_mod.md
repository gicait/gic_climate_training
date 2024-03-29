## What is a model?
- A model is a simplified representation of a real system.
> A schematic description of a system, theory, or phenomenon that accounts
for its known or inferred properties and may be used for further studies of
its characteristics.

#### Physical models
- A physical copy of an object scaled to smaller or larger
  - Scaled-down model: a model of an airplane
  - Scaled-up model: a model of an atom

#### Numerical models
- Use mathematical formulas or statistical methods
    - Climate models are based on mathematical formula

## General Circulation Models (GCM)

- A general circulation model (GCM) is a type of climate model.
- A climate model is a mathematical representation of the climate system based on physical biological and chemical principles. 
  
<div align=center>
<img width=\textwidth src="./_media/gcm_parts.PNG"/>
</div>

### Insights into GCMs
- GCMs are computer programs often hundreds of thousands of lines of code mostly written in Fortran and strung together by Unix scripts
- It divides the atmosphere, oceans, and land into a 3 dimensional grid system 
- The physical equations and parameterization are then calculated for each grid cell in a loop.
- Parameterizations are formulas based on empirical evidence
- The fundamental physical quantities calculated by a GCM are:
  - Temperature ($T$)
  - Pressure ($P$)
  - Winds speed (East-West: $U$, North-South: $V$)
  - Specific Humidity ($Q$)

<div align=center>
<img width=\textwidth src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/AtmosphericModelSchematic.png/350px-AtmosphericModelSchematic.png"/>
</div>

#### Typical workflow of GCM
1. Compile all the mathematical equations needed to represent the physical characteristics and processes, and enter them into each grid box.
2. The equations are converted into computational codes and set the climate variables.
3. The computational codes are run on a cluster or a supercomputer to solve all the equations and calculate the next set of initial conditions.
4. Models are tested and refined by simulating past climate
5. The results are then checked against the observation data.
6. The models that successfully approximate past climate are considered valid, and can be used to model future climate scenarios.
<div align=center>
<img width=\textwidth src="https://ccafs.cgiar.org/sites/default/files/research/pictures/fig_1_gcm_limitations_and_bc.jpg"/>
</div>
