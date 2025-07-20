# TC-Center-FRACTL

# TC_center_finding
This repository houses code to estimate TC centers using the horizontal wind. All scripting done in Python.
## Background
Identifying a TC center is not a trivial task. This is especially true when using platforms that contain missing data, such as airborne radar observations, which is the platform that motivated this method. Previous work has identified TC centers using the mass field (e.g., centroids of pressure perturbations on height surfaces; Nguyen et al. 2014). However, when using radar observations, the mass field may not be readily available. The center-finding method introduced here aims to use the motion-relative horizontal wind field to identify the TC center. 

The goal is to objectively identify the grid point that yields the best match with a perfectly cyclonic vortex using a weighted angle-deviation technique. To some extent, this method is similar to identifying the center of circulation, which is done subjectively in an operational setting. Although the present method was originally intended for radar analyses, preliminary analyses show it also works using high-resolution model output.

## Code dependencies
numpy

## How to use
As of now, a single Python file is provided, which includes the functions used to apply the center-finding algorithm. At the end of the .py file, an example is provided of how to apply the recenter_tc function to get the TC center coordinates.

## Reference
This method is discussed in more detail in Fischer et al. (2022, 2024; full reference below):

Fischer, M. S., P. D. Reasor, R. F. Rogers, and J. F. Gamache, 2022: An Analysis of Tropical Cyclone Vortex and Convective Characteristics in Relation to Storm Intensity Using a Novel Airborne Doppler Radar Database. Mon. Wea. Rev., 150, 2255–2278, https://doi.org/10.1175/MWR-D-21-0223.1.

Fischer, M. S., R. F. Rogers, P. D. Reasor, and J. P. Dunion, 2024: An Observational Analysis of the Relationship between Tropical Cyclone Vortex Tilt, Precipitation Structure, and Intensity Change. Mon. Wea. Rev., 152, 203–225, https://doi.org/10.1175/MWR-D-23-0089.1.
