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

## Methodology: Vector AutoRegression (VAR)

We will use VAR to leverage three complementary tools.

### 1. Granger Causality

**Research question:** Can deep terrestrial water storage in month *t* improve our forecast of precipitation in future month *t+3*, better than the precipitation record alone? If so, storage is said to Granger-cause precipitation.

This provides meaningful evidence of directional predictive influence flowing from one part of the system to another.

### 2. Impulse Response Functions (IRFs)

A single anomalous pulse is introduced to one variable, and we trace how the disturbance propagates through the system over subsequent months.

**Research question:** Can layers beneath the top 5 cm — including those deeper than 1 m — have predictive power for rainfall and wet season onset?

If the IRF shows an acceleration of rainfall following a change in deep subsurface water, this supports the theory that ET from land triggers the wet season. IRFs will also clarify the **timing and persistence** of the precipitation response at each subsurface layer.

### 3. Forecast Error Variance Decomposition (FEVD)

FEVD will **quantify the relative contribution** of each subsurface layer to precipitation variability.
