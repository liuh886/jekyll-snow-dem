---
layout: page
title: "Project Background & Links"
permalink: /background-and-publications/
sectionid: "project-background"
image: /img/cm-og-image.png
---

Accurate estimates of accumulated snow are critical in predicting runoff for water resource management and hydroelectricity. Snow characteristics also induce significant uncertainties for periglacial, weather and climate studies. Remote sensing provides multiple techniques to observe snow pack. While snow cover extent has been successfully addressed, SWE or Snow depth are much more challenging, particularly the snow depth in mountain areas.

- Preferred frequency (Ku-band Synthetic Aperture Radar) for snow depth is not in space yet.
- Passive microwave observations has coarse (~25km) footprints and lack of mountains.
- Airborne Lidar system is accurate but local interest and costly(Deems et al., 2013; Painter et al., 2016).


## Altimetry or radar, which one is the solution?

Firstly, ICESat's elevations on snow surface are compared to the DEM elevations to retrieve snow depth by Désirée Treichler. She found that the main source of uncertainty lies with ICESat's large footprints (70 m) and the terrain variation therein within the reference DEM: spatially varying, systematic vertical bias severely hamper accurate estimation. For the regions with abundant frozen lakes(no need DEM), the repeat ICESat altimetry observations can derive snow accumulation information with r of 0.88 and RMSE of 5 cm. Now **what if there is new ICESat-2 (~ 14 m footprint) and high quality DEM nowadays?**

- Treichler, D., & Kääb, A. (2017). **Snow depth from ICESat laser altimetry—A test study in southern Norway**. *Remote Sensing of Environment*, *191*, 389–401. https://doi.org/10.1016/j.rse.2017.01.022

- Shu, S., Liu, H., Frappart, F., Huang, Y., Wang, S., Hinkel, K. M., Beck, R. A., Yu, B., Jones, B. M., Arp, C. D., Wang, L., & Ye, Z. (2018). **Estimation of snow accumulation over frozen Arctic lakes using repeat ICESat laser altimetry observations – A case study in northern Alaska**. *Remote Sensing of Environment*, *216*, 529–543. https://doi.org/10.1016/j.rse.2018.07.018

Microwave radar in C-band (Sentinel-1) is an ideal solution for snow depth: 6 days revisit period, 2-satellites with long-term continuity, 5 m x 20 m resolution. The C-Snow team from Leuven University has done extensive work. By cross-polarized backscatter algorithm, C-SNOW retrieves snow depth in mountainous areas with the large scale (1 km). Sentinel-1 reveals the spatial detail and the elevation profile of snow depth by resembling with reanalysis data.

- Lievens, H., Demuzere, M., Marshall, H.-P., Reichle, R. H., Brucker, L., Brangers, I., de Rosnay, P., Dumont, M., Girotto, M., Immerzeel, W. W., Jonas, T., Kim, E. J., Koch, I., Marty, C., Saloranta, T., Schöber, J., & De Lannoy, G. J. M. (2019). **Snow depth variability in the Northern Hemisphere mountains observed from space**. *Nature Communications*, *10*(1), 4629. https://doi.org/10.1038/s41467-019-12566-y

## ICESat-2's elevation measurement is beneficial, and DEM continue hampering

ICESat-2 has made a great success in the polar area. The top height of snowpack over the sea ice can be retrieved by ICESat-2. The actual snow depth then equals to the top height minus the bare height of sea ice from radar measurements of CryoSat-2. Elevation differencing works but gets unhandy when it comes to complex terrain.

- Kwok, R., Kacimi, S., Webster, M. A., Kurtz, N. T., & Petty, A. A. (2020). **Arctic Snow Depth and Sea Ice Thickness From ICESat‐2 and CryoSat‐2 Freeboards: A First Examination**. *Journal of Geophysical Research: Oceans*, *125*(3). https://doi.org/10.1029/2019JC016008

## DEM Co-registration & uncertainty 

The shift between repeat DEMs might have systematic difference, in particular if the originate from different sensors or orientation procedures.  Kääb (2005, 2011) and Nuth (2011) has an iterative approach by solving a cosine equation to co-registrate DEMs efficiently, which is a key to address DEM uncertainties and snow depth in this case.

- Kääb, A. (2005). ***Remote sensing of mountain glaciers and permafrost creep***. Geographisches Institut der Universität Zürich. page 67
- Nuth, C., & Kääb, A. (2011). **Co-registration and bias corrections of satellite elevation data sets for quantifying glacier thickness change**. *The Cryosphere*, *5*(1), 271–290. https://doi.org/10.5194/tc-5-271-2011

## Climate - Related Links

### Snowdepth in forecast system
Snow in reanalysis provides critical surface information for forecast system from the medium to sub-seasonal timescales. But now even the stat-of-art reanalysis products produces an over-extensive snowpack in autumn, winter and spring over parts of the TP. We do need more information about snow depth.

- Orsolini, Y., Wegmann, M., Dutra, E., Liu, B., Balsamo, G., Yang, K., de Rosnay, P., Zhu, C., Wang, W., Senan, R., & Arduini, G. (2019). **Evaluation of snow depth and snow cover over the Tibetan Plateau in global reanalyses using in situ and satellite remote sensing observations**. *The Cryosphere*, *13*(8), 2221–2239. https://doi.org/10.5194/tc-13-2221-2019
-  Global reanalysis products (ECMWF-EAR5, JRA-55, MERRA-2) are systematically compared with in situ snow depth and satellite snow cover dataset. The results suggest a common model precipitation bias over the Himalayas and the TP, and excessive snowfall might be the primary factor for the large overestimation of snow depth and cover in ERA5 reanalysis.
   
### Snowdepth in periglaciation and climate study

> Decreasing snow depth, in parallel, reduces the thermal insulation of soil interface with atmosphere and increases soil vulnerability to fluctuations in air temperature. This can in turn contribute to decreasing frost depth and increasing the frequency of swings in FT states. Such changes can result in widespread alterations in regional hydrology, phenology, geology, water quantity, and quality as well as socio-economic activities. In addition, some of these alterations can create feedback effects with other elements of the environment. For instance, thawing landscapes in northern regions can affect the climate system through the emission of excessive greenhouse gas fluxes, which can intensify the rate of global warming.
- Hatami, S., Nazemi, A. Compound changes in temperature and snow depth lead to asymmetric and nonlinear responses in landscape freeze–thaw. Sci Rep 12, 2196 (2022). https://doi.org/10.1038/s41598-022-06320-6

## Other Resources

**DEM products**

 * [Arctic DEM]([ArcticDEM – Polar Geospatial Center (umn.edu)](https://www.pgc.umn.edu/data/arcticdem/))

**Other projects**

- [C-SNOW: 1 km resolution observations of snow depth by Sentinel-1 Radar ](https://ees.kuleuven.be/project/c-snow)

**Tools, Repository & Documentary** 

- [xDEM: Analysis of digital elevation models for geosciences — xdem 0.0.6 documentation](https://xdem.readthedocs.io/en/latest/)
- [Technical Specs | ICESat-2 (nasa.gov)](https://icesat-2.gsfc.nasa.gov/science/specs)

_If you are interested in our project do not hesitate to [get in touch with us](/about-us.html/)._



***References:***

Deems, J. S., Painter, T. H., and Finnegan, D. C. (2013). Lidar Measurement of Snow Depth: A Review. J. Glaciol. 59 (215), 467–479. doi:10.3189/ 2013JoG12J154

Painter, T. H., Berisford, D. F., Boardman, J. W., Bormann, K. J., Deems, J. S., Gehrke, F., et al. (2016). The Airborne Snow Observatory: Fusion of Scanning Lidar, Imaging Spectrometer, and Physically-Based Modeling for Mapping Snow Water Equivalent and Snow Albedo. Remote Sensing Environ. 184, 139–152. doi:10.1016/j.rse.2016.06.018

Hugonnet, R., Brun, F., Berthier, E., Dehecq, A., Mannerfelt, E. S., Eckert, N., & Farinotti, D. (2022). **Uncertainty analysis of digital elevation models by spatial inference from stable terrain**.  IEEE JOURNAL OF SELECTED TOPICS IN APPLIED EARTH OBSERVATIONS AND REMOTE SENSING.
