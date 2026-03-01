# Subsurface Water Influence on Precipitation

## Motivation

We are interested in understanding how subsurface water influences precipitation, contributing to the body of research evaluating the role of the land surface as a memory and modulator of the hydrological cycle.

**Key literature:**

| Study | Method | Finding |
|---|---|---|
| Tuttle (2016) | Granger causality | Changes in surface soil moisture can help predict subsequent precipitation events |
| Dirmeyer (2011) | Land–atmosphere model experiments | Soil moisture correlates with rainfall on weeks-to-months timescales |

---

## Research Gap

Upper soil layers act as a fast-to-medium memory in the coupled system, but **do deeper layers of soil and groundwater contribute to precipitation variability?**

Modeling studies show groundwater impacts precipitation through medium-to-slow moving feedbacks in the land-atmosphere system:

| Study | Notes |
|---|---|
| Barlage (2017) | — |
| Anyah (2008) | — |
| Martinez (2016) | — |
| Adole (2018) | Vegetation greening precedes the first rain in the Sahel |
| Wright (2017) | Model-based studies of the Congo suggest that early-season soil moisture and vegetation feedbacks: (1) precondition rainfall, (2) accelerate monsoon onset, and (3) influence larger-scale circulation to bring in ocean moisture earlier |

However, limitations in stable isotope analyses highlight a need for **additional observationally constrained approaches** to verify the influence of deep subsurface water.

---

## Research Question

| Hypothesis | Statement | Approach |
|---|---|---|
| 1 | Increases in subsurface water, at a shallow (below 5 cm) and deep (below 1 m) level, influence increases in rainfall. | Compare prediction with subsurface water vs the rainfall's autoregressive timeseries data. Compare F-stat vs p-value. |
| 2 | Deep subsurface water increases rainfall at monthly and inter-annual scales. | IRFs |
| 3 | Deep subsurface water can trigger the onset of the wet season. | IRFs |

**Research question:** Can layers beneath the top 5 cm — including those deeper than 1 m — have predictive power for precipitation variability, wet season onset, and wet season duration across medium and multi-year timescales?

---

## Data

| Source | Scales | Var(s) | Data |
|---|---|---|---|
| SMAP | 300 km grid cell, monthly | surface soil moisture (5 cm and above) | surface soil moisture (5 cm and above) |
| GRACE JPL, SMAP | 300 km grid cell, monthly | tws (total water storage) - surface soil moisture (5 cm and above) | Subsurface water levels (shallow; below 5 cm) |
| GRACE-constrained GLDAS2.2 | 300 km grid cell, monthly | tws (total water storage) | Subsurface water levels (deep; below 1 m) |
| - | - | - | - |

Five locations will be examined at 13.5° N latitude, and 2 location in Congo looking at different water basins.

| Country/Area | Latitude Range | Longitude Range | 
|---|---|---|
| The Sahel | 13.5° N | 17° W to 35° E |
| Burkina Faso | 13.5° N  3° W to 1° E |
| Chad | 13.5° N | 13°40' E to 23° E |
| Guinea | 13.5° N | 12°W to 13.5°W |
| Nigeria | 13.5° N | 8° E to 14° E |
| Mali | 13.5° N | 12°W to 4°E |
| Congo | - | - |
| Congo | - | - |

---

## Methodology: Vector AutoRegression (VAR)

We will use VAR to leverage three complementary tools.

### 1. Granger Causality

**Research question:** Can deep terrestrial water storage in month *t* improve our forecast of precipitation in future month *t+3*, better than the precipitation record alone? If so, storage is said to Granger-cause precipitation.

This provides meaningful evidence of directional predictive influence flowing from one part of the system to another.

### 2. Impulse Response Functions (IRFs)

A single anomalous pulse is introduced to one variable, and we trace how the disturbance propagates through the system over subsequent months.

If the IRF shows an acceleration of rainfall following a change in deep subsurface water, this supports the theory that ET from land triggers the wet season. IRFs will also clarify the **timing and persistence** of the precipitation response at each subsurface layer.

### 3. Forecast Error Variance Decomposition (FEVD)

FEVD will **quantify the relative contribution** of each subsurface layer to precipitation variability.
