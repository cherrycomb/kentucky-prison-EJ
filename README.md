# Prisons and Environmental Hazards in Kentucky
### RL Martens

This map was created to help visualize and identify potential environmental hazards affecting incarcerated people in the commonwealth of Kentucky. The black dots on the map represent environmental hazards taken from EPA EnviroAtlas and EarthJustice datasets. Zoom in on the points and you'll be able to see exactly what type of hazard each dot represents. The map was created using MapBox Studio and QGIS-LTR.

#### Mapping Process

This map began with a basemap style created in Mapbox Studio. Point datasets representing environmental hazards downloaded from the EPA EnviroAtlas and EarthJustice websites were uploaded directly into Mapbox as datasets and then exported as tilesets. Landfill point data from the DHS was also uploaded directly into Mapbox.  State-run Kentucky adult prison point data was uploded directly into Mapbox. I extracted Federal prison and juvenile prison data from the websites listed below and created my own .csv datasets by locating the coordinates of these facilites on OpenStreetMap. Data from the EPA on cancer risk per million due to cumulative air toxics represented via choropleth on the map was first loaded into QGIS-LTR. Null data was subtracted from the dataset. It was then joined with County level data from NaturalEarthData by GEOID. The temporary join was then exported as a shapefile and uploaded to Mapbox Studio.

#### Data Sources:

##### Environmental Hazards:

+ United States Environmental Protection Agency. EnviroAtlas. Cancer risk per million due to cumulative air toxics, Brownfield Grantee(ACRES), Superfund, Hazardous Waste Sites (RCRA), Toxic Release Inventory (TRI), Cancer Risk per million due to cumulative air toxics. Retrieved: 6 /7/2022, from epa.gov/enviroatlas. 

+ EarthJustice, Coal Combustion Residuals, from https://earthjustice.org/features/coal-ash-contaminated-sites-map. 

+ Department of Homeland Security, Homeland Infrastructure Foundation-Level Data, Solid Waste Landfill Facilities https://hifld-geoplatform.opendata.arcgis.com/datasets/155761d340764921ab7fb2e88257bd97_0/about

##### Prisons:

+ Kentucky Department of Juvenile Justice, Juvenile Detention Facility Locations. https://djj.ky.gov/Facilities/Pages/Detention-Centers.aspx

+ Kentucky Division of Geographic Information, Adult Prison Locations. https://ky.app.box.com/v/kymartian-prisons

+ Federal Bureau of Prisons, Federal Prisons in Kentucky. https://www.bop.gov/locations/list.jsp  

##### Misc. 

+ Natural Earth Data, Admin 2- Counties. https://www.naturalearthdata.com/downloads/10m-cultural-vectors/ 
