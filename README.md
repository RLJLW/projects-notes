## General projects notes and ideas

How to Get Sentinel-2 data
https://www.earthdata.nasa.gov/learn/tutorials/find-landsat-sentinel-2-imagery-area-interest-worldview

Detect a fire risk
 - Excessive heat, plus high winds - model learns to predict fire risk
 - Analyse dry amounts of vegetation and highlight fire risks

Could use Sentinel2 and Landsat, and SAR
 
Analysing landscapes

Check - some suggestions by Chat GPT follows (retyped and summarised) :
--------------- Chat GPT suggestions retyped and summarised ---------
Plant stress could mean
 - Lack of water
 - Nutrient Deficiency
 - Disease
 - Excess heat
 - Excess salinity 
 - Pest Attack

Lower refelctance in NIR -> leaves lose internal structure
Higher reflectance in red = less Chlorophul absorption

Detect crop water stress before its visible
Optimizse irrigation schedules
identify butrient or disease hot spots
estimate yield potential

"
Spectral Region	Sensitive To	What It Tells You
Visible (400–700 nm)	Chlorophyll absorption	Greenness, photosynthesis
Red edge (~700 nm)	Chlorophyll breakdown	Stress onset
Near-Infrared (NIR, 700–1300 nm)	Leaf structure + water content	Health and moisture
Shortwave Infrared (SWIR, 1300–2500 nm)
" - Chat GPT


--------------- /Chat GPT suggestions retyped and summarised ---------


  

Use Normalised Difference Vegetation index
Use NDWI - Water index - see https://en.wikipedia.org/wiki/Normalized_difference_water_index - used to monitor water content in leaves, another similar formula can be used to "monitor water content in water bodies".
Use PRI - Photo chemical reflectance index
https://en.wikipedia.org/wiki/Photochemical_Reflectance_Index
 - Can be used to measure plants response to stress.
 - PRI is can be used to analyze photosynthetic light use efficiency, or rate of C02 uptake.
 - Useful for determining vegetation productivity and stress.
 - Analyse eco system health and stress
 - uses 531 nm and 570 nm in a simmular formulate to NDVI

Caratenoids absorb light energy in photosnthesis, used by all photosynthetic organisms

 - PRI measures refeletance on either side of the green reflectance peak of the graph at 550nm
 - It compares reflectance in the blue spectrum which - which is cholorophyll and caratenoids, with the red which is
   chlorophyll only - Therefore it can determine a kind of an index between choloropyl to aratenooid levels
   which is often called bulk pigment rations.



"
Since PRI measures the relative reflectance on either side of the green reflectance “hump” (550 nm), it also compares the reflectance in the blue (chlorophyll and carotenoids absorption) region of the spectrum with the reflectance in the red (chlorophyll absorption only) region. Consequently, it can serve as an index of relative chlorophyll:carotenoid levels, often referred to as bulk pigment ratios or “pool sizes”. Over longer time scales (weeks–months), changes in bulk pigment content and ratios due to leaf development, aging or chronic stress have been reported to play a significant role together with the xanthophyll pigment epoxidation in the PRI signal (Gamon et al., 2001, Peñuelas, Filella, et al., 1997a, Sims and Gamon, 2002, Stylinski et al., 2002). Thus, PRI is also often related to chlorophyll/carotenoid ratios in leaves across a large number of species, ages and conditions (Filella et al., 2009, Stylinski et al., 2002). Therefore, to the extent that photosynthetic activity correlates with changing chlorophyll/carotenoid ratios in response to stress, ontogeny or senescence, PRI may provide an effective measure of relative photosynthetic rates. Together, these responses to de-epoxidation state of the xanthophyll cycle and to chlorophyll/carotenoid ratios ensure that PRI scales with photosynthetic efficiency across a wide range of conditions, species and functional types (Filella et al., 1996, Gamon et al., 1992, Gamon and Qiu, 1999, Peñuelas et al., 1995, Stylinski et al., 2002).
Nowadays, the PRI is increasingly being used as an index of photosynthetic performance in general and of RUE in particular in natural and seminatural vegetation (e.g. Asner et al., 2004, Mänd et al., 2010, Middleton et al., 2009, Peñuelas and Llusia, 2002) or in crops (e.g. Strachan et al., 2002, Zhou and Wang, 2003). The relationships between PRI and different ecophysiological related variables have been tested over a wide range of species, plant functional types, temporal steps and environmental conditions.
"
- https://www.sciencedirect.com/science/article/abs/pii/S0034425710002634
