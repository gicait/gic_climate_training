## Weather Research and Forecasting Model (WRF)
### What is WRF?
- The Weather Research and Forecasting (WRF) Model is a next-generation mesoscale numerical weather prediction system designed for both atmospheric research and operational forecasting applications.
- The model serves a wide range of meteorological applications across scales from tens of meters to thousands of kilometers.
- The effort to develop WRF began in the latter 1990's and was a collaborative partnership of the National Center for Atmospheric Research (NCAR), the National Oceanic and Atmospheric Administration (represented by the National Centers for Environmental Prediction (NCEP) and the Earth System Research Laboratory), the U.S. Air Force, the Naval Research Laboratory, the University of Oklahoma, and the Federal Aviation Administration (FAA).

#### Inside WRF
- WRF has 2 dynamical cores:
  -  **The Advanced Research WRF (ARW)**
  -  **Non-hydrostatic Mesoscale Model (NMMM)**
- Dynamical core includes mostly advection, pressure gradients, Coriolis force, buoyancy force, filters, diffusion, and time-stepping.
- ARW development, maintenance and support are centered at NCAR/Mesoscale& Microscale Meteorology(MMM)
- NMM development was centered at NCEP/Environmental Modelling Center(EMC) and support is provided by NCAR/Development Tested Center (DTC)
  


---
### What can WRF be used for?
- WRF offers operational forecasting a flexible and computationally-efficient platform, while reflecting recent advances in physics, numerics, and data assimilation contributed by developers from the expansive research community.

- For researchers, WRF can produce simulations based on actual atmospheric conditions (i.e.from observations and analyses) or idealized conditions. 
  - Develop and test physical parameterization 
  - Case-study research for specific weather events
  - Regional climate studies
  - Coupled-chemistry, fire, and hydrological applications
  - Data assimilation research
  - Teaching modelling and numerical weather prediction 
- A tool for numerical weather prediction
  - Hind-casting
  - Real-time (operational) forecasting for wind, solar, and air quality (online and offline)


---
## WRF Preprocessing System (WPS)
### What is WPS?
- A collection
of Fortran and C programs that provides data used as input to the *real.exe* program. There are **three main programs** and a number of auxiliary programs that are part of WPS.

- Main programs: **geogrid.exe**, **ungrib.exe**, **metgrid.exe**

Input to the main programs is through the namelist file "**namelist.wps**".  Each main program has an exclusive namelist record (named "geogrid", "ungrib",or "metgrid", respectively), and the three programs have a group record (named "share") that each program
reads.

**geogrid**
1) Defines the model horizontal domain
2) Horizontally interpolates static data to the model
domain
3) Output conforms to the WRF I/O API

**ungrib**
1) Decodes Grib Edition 1 and 2 data
2) Uses tables to decide which variables to extract
3) Supports isobaric and generalized vertical coordinates
4) Output is in a non-WRF-I/O-API form, referred to as an
   intermediate format

**metgrid**
1) Ingest static data and raw meteorological fields
2) Horizontally interpolate meteorological fields to the 
   model domain
3) Output conforms to WRF I/O API 

<div align=center>
<img width=\textwidth src="https://anamika255.github.io/assets/images/Wrf-workflow.png"/>
<figcaption>WPS and WRF Program flow</figcaption>
</div>

---
**Additional information**
> WRF User Guide: https://www2.mmm.ucar.edu/wrf/users/docs/user_guide_v4/v4.4/contents.html