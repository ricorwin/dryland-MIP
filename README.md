This dataset was collected as part of a mycorrhizal inoculum potential bioassay conducted with soils sampled from six dryland sites in the Southwestern USA. Within each site, soils were taken from paired areas: a "disturbed" area with low desirable native vegetation cover and known grazing/cropping disturbance, and a "reference" area with no or low disturbance and high desirable native vegetation cover. The soils were collected along two transects and transported back to the Northern Arizona University Research Greenhouse, then used to fill pots for two bioassays (utilizing Bouteloua gracilis and Zea mays, respectively). Arbuscular mycorrhizal colonization of the plant host roots was assessed using staining and microscopy after 5-6 weeks of growth. 

Description of field data columns, where not apparent:

transect: D/R = Disturbed or Reference

rep: Pot number within each site and transect (1-10 = B. gracilis; 11-20 = Z. mays)

m_mark: Meter mark (along the transect tape)

nearby_spp: Nearby plant species at each sampling hole, using USDA plant codes

collection_point_desc: Description of the area around the sampling hole

Vegetation functional group percent cover columns: "nat" indicates native plant species, "nonnat" indicates non-native plant species. Recorded numbers are percent out of 100, with bare cover calculated as the remaining area after plant cover and biocrust were accounted for. 

Description of arbuscular mycorrhizal colonization columns: Fine root segments from the bioassay hosts were cleared and stained for visualization of fungal structures under a microscope. These structures were quantified using the gridline-intersect method for 100 root intersections. Blank cells in the root-scoring and biocrust columns indicate the structure or cover was not observed and are treated as 0.

no_fungus: Number of root intersections where no fungal structures were crossed

am_hyphae: Number of root intersections where arbuscular mycorrhizal hyphae were crossed

DSE: Number of root intersections where dark septate endophyte structures were crossed

LSE: Number of root intersections where light septate endophyte structures were crossed

arb: Number of root intersections where arbuscules were crossed

coil: Number of root intersections where arbuscular mycorrhizal coil structures were crossed

ves: Number of root intersections where arbuscular mycorrhizal vesicles were crossed

spore: Number of root intersections where arbuscular mycorrhizal spores were crossed

olpid: Number of root intersections where olpidium fungal structures were crossed

plasmod: Number of root intersections where plasmodiophorid structures were crossed

mold: Number of root intersections where mold structures were crossed

unk_fungi: Number of root intersections where unknown fungal structures were crossed

xtra: Number of root intersections where more than one structure overlapped/were crossed together

total_sub_xtra: Total number of intersections with extra structures subtracted (100 targeted)

am_RLC: arbuscular mycorrhizal root length colonized, calculated as the sum arbuscular mycorrhizal structures divided by the total intersections crossed, then multiplied by 100. 

For analysis, the primary variables examined were am_RLC as the response, and site, transect, and vegetation cover categories as predictors, using R 4.4.2 with glmmTMB 1.1.10, DHARMa 0.4.7, performance 0.16.0, emmeans 1.10.5, and vegan 2.6-10. Analyses can be reproduced by opening Dryland_MIP_analysis.Rmd in R and knitting it; the spreadsheet must be in a folder named data/ next to the Rmd. Figures and the Table S2 contrasts are written to an automatically created figures/ folder. 

An additional note on the soil physicochemical data (Dryland_Pooled_Soil_Physicochem.xlsx): This sheet contains soil properties measured on two pooled composites per transect (soil from the first five and last five sampling points). Table 1 in the manuscript reports the mean of the two composites for each transect. Sand and clay were determined by hydrometer, and silt was calculated by difference (100% - sand - clay). Sand, silt, and clay are stored as proportions (displayed as percentages in Excel). Methods for all properties are described in the manuscript. These data were not used in the statistical analyses. For additional questions on any of the above, contact the author of this page. 
