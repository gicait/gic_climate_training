## Physics modules within WRF
In order to simulate real weather and to run simulations with coarse resolutions, a minimum set of physics components is required:
- Radiation
  - Longwave (ra_lw_physics)
  - Shortwave (ra_sw_physics)
- Surface
  - Surface layer (sf_sfclay_physics)
  - Land/water surface (sf_surface_physics)
- Planetary Boundary Layer (PBL) (bl_pbl_physics)
- Turbulence/Diffusion (diff_opt, km_opt)
- Cumulus parameterization (cu_physics)
- Microphysics (mp_physics)