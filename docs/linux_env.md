## Setting up environment for WRF
> Tutorial: https://www2.mmm.ucar.edu/wrf/OnLineTutorial/compilation_tutorial.php

**IMPORTAN**: In order to use personal machines, all the required programs and compiler have to be built and verified through testing.

### System Environment Tests
- It is very important to have a gfortran compiler, as well as gcc and cpp. To test whether these exist on the system, type the following:
    >which gfortran \
    which cpp \
    which gcc 

    If you have these installed, you should be given a path for the location of each.

- We recommend using a Fortran compiler that supports Fortran2003 standard (version 4.6 or later). To determine the version of gfortran you have, type:
    >gcc --version

---
### Libraries for WRF/WPS Builds
- NetCDF (needed by WRF and WPS)
  - netCDF Version 3 or 4
  - If using netCDF4 capabilities
  http://www2.mmm.ucar.edu/wrf/users/building_netcdf4.html
- Optional libraries for GRIB2 meteorological data support
  - JasPer (JPEG 2000 “lossy” compression library) PNG (“lossless” compression library)
  - Zlib (compression library used by PNG)
- Optional MPI library (for building in parallel):
  - E.g., MPICH2 or OpenMPI
  - In principle any implementation of the MPI standard should work, but we have the
  most experience with MPICH.

  ---
### Setting up system environment
- We have made things easier for you by preparing a shell script ('***li1.sh***') to install and set up the system environment.
- You can directly copy and paste the following commands
    >   mkdir LIBRARIES \
        cd LIBRARIES \
        scp root@167.172.132.202://root/libraries/* ./ \
        sh li1.sh

---
## Compiling WRF and WPS with CORDEX
> The **CO**ordinated **R**egional climate **D**ownscaling **EX**periment (**CORDEX**) is a framework aimed at improving coordination of international efforts in regional climate downscaling research. CORDEX was initiated as a result of the task Force on Regional Climate Downscaling, formed by the World Climate Research Program (WCRP).

**Downloading WRF-CORDEX v1.3**
1. First, we will make a new folder and download WRF source codes from its repository.
    >mkdir self_compile \
    cd self_compile \
    git clone --branch v4.0 https://github.com/wrf-model/WRF

   
2. Download CORDEX source codes into the WRF folder and unpack
    >sudo wget https://zenodo.org/record/1469651/files/WRFV4.0_CORDEX_v1.3.tar.gz -P WRF/

    > cd WRF/

    > tar xvfz WRFV4.0_CORDEX_v1.3.tar.gz

3. Edit the Registry.EM file

    > cd Registry

    > v