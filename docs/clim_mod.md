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
<img width=\textwidth src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/AtmosphericModelSchematic.png/350px-AtmosphericModelSchematic.png"/>
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
<img width=\textwidth src="https://ccafs.cgiar.org/sites/default/files/research/pictures/fig_1_gcm_limitations_and_bc.jpg"/>
</div>