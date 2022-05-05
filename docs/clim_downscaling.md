## What is Climate Downscaling?

- Most climate change projections are developed using global-scale models that generate average temperature changes that can be expected to occur over decades and far into the future.
- These global models are unable to represent granular atmospheric features such as cloud cover, airborne particles, and local pollution sources. Yet these smaller details can have a big impact on local climate, which is one reason the effects of climate change are expected to vary depending on geographic location.
- **“Downscaling”** climate models are an attempt to bridge the gap between global and local effects by layering local-level data over larger-scale climate models.
- Downscaled modeling examines relatively small areas in detail—in some cases down to 25 square kilometers,3 a far higher resolution than that offered by global climate model simulations.
- **Goal**: to generate more locally relevant projections of long-term weather patterns for regions, states, and cities.

- A process of generating higher-resolution data (or climate change information) from the relatively coarse-resolution GCMs.
- Generally, there are two main strategies for downscaling:  
  - **Dynamical Downscaling**: Dynamical extrapolation of the effects of large-scale climate processes to regional or local scales.
  - **Statistical Downscaling**: Establishing a statistical relationship between local observational data and large-scale (global) variables.


---

**Dynamical Downscaling** 

- Dynamical downscaling is carried out by nesting a fine-scale climate model in a coarse-scale global model.
- A higher resolution climate model is used for dynamical downscaling, and these models are often called regional climate models (RCM).
-  RCM use lower resolution climate models (in most cases GCMs) as boundary conditions and physical principles to reproduce local climate. 
-  RCM are computationally intensive, so for some regions only limited RCM output data is available. 
-  RCM for CORDEX with a grid size of 0.44 degrees are often used (grid sizes of ~45 $\times$ 45 $km^2$
).

<div align=center>
<img width=\textwidth src="./_media/dyn_down.jpg"/>
</div>


---

**Statistical Downscaling**
- If RCM data is not available for your region or is still too coarse, you can use Statistical downscaling.
- Statistical downscaling involves relating the large-scale climate state to the local-scale target variables (e.g. precipitation, temperature, and humidity) using a ***transfer function***, such as regression or weather generators. 
- A statistical relationship is developed between the historic observed climate data and the output of the climate model for the same historical period. The relationship is used to develop the future climate data.
- Essential for statistical downscaling is the availability of local weather data. The results of
the statistical downscaling become better with higher quality and longer duration of historic observed weather data. 


<div align=center>
<img width=\textwidth src="https://bookdown.org/floriandierickx/bookdown-demo/figures/statistical-downscaling-theory.png"/>
</div>


---
**Strengths and weaknesses of Statistical versus Dynamical downscaling methods**

|  | **Statistical Downscaling** | **Dynamical Downscaling** |
|---|---|---|
| **Advantages** | <ul> <li>Comparatively cheap and computational efficient.</li> <li>Can provide point-scale climate variables from GCM-scale output.</li> <li>Able to directly incorporate observations into method.</li> </ul> | <ul> <li>Produces responses based on physically consistent processes.</li> <li>Can resolve atmospheric processes on a smaller scale (e.g. orographic and rain-shadow effects in mountainous areas).</li> </ul> |
| **Disadvantages** | <ul> <li>Dependent upon choice of predictors.</li> <li>Does not account for non-stationarity in the predictor-predictand relationship.</li> <li>Regional climate system feedbacks not included.</li> <li>Affected by bias in underlying GCM.</li> </ul> | <ul> <li>Computationally intensive.</li> <li>Limited number of scenario ensembles available.</li> <li>Dependent on GCM boundary forcing; affected by biased in underlying GCM.</li> <li>Dependent on RCM parameterizations.</li> <li>Different RCMs will give different results.</li> </ul>
 |

