##  https://github.com/bbarker505/1990_daily_30yr

## Description 
This folder contains daily downscaled temperature (tmin and tmax) data for 1961-1990 normals.
The original data are monthly PRISM temperature data available at http://www.prism.oregonstate.edu.

## Purpose
The data were needed to produce climate suitability models in the Degree-Days, Risk, and Phenological 
event mapping (DDRP) platform, which requires daily temperature (tmax and tmin) data. PRISM has only
monthly data for most years over the 1961-1990 time frame. Climate suitability models produced using
these in DDRP were calibrated in accordance with models produced using the CLIMEX v. 4 software program 
(available at:https://www.hearne.software/Software/CLIMEX-DYMEX/Editions).
 
## Methods
Daily downscaling was conducted by running a Perl and Octave script available at https://github.com/bbarker505/dailynorms.
For each month of a given year, the script uses a bilinear interpolation method to assign each day an avg. temperature 
value that is iteratively smoothed and then adjusted so that the monthly averages were correct. README files in the folder
that contains these scripts provide more details on this analysis.

