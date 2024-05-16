# GEOG5990M_final
# The background/context of the project:
This project is doing a public resource assessment, to evaluate is fuel resource distributed equally in Leeds.
This idea is derived from a Environmental Assessment(EA) concept: Environmental Justice Analysis. It is an assessment tool usually used to assess the distribution equity of air quality or other shared resources.
This approach is used here to assess fuel distribution within the city of Leeds, because many researches showed that nowadays people are facing the problem of fuel poverty, especially in winter.
The purpose of this report is to show Public and Policymaker an exploration of the uneven distribution of fuels. Hope it can inspire and help the improvement of social welfare in the future.
# What data the GitHub repository contains:
there are two data files needed, one contains the households number and proportion of fuel poverty situation and the other contains the boundary of Leeds, the two data are from different data source. Noted below:
(1)Fuel poverty by LSOA.csv;  data sources: Data Mill North https://datamillnorth.org/dataset/2j70l/fuel-poverty-by-lsoa-england
(2)Leeds.geojson;  data sources: Office for national statistics https://geoportal.statistics.gov.uk/maps/761ecd09b4124843b95511a242e2b1a1
# What the code aims to do
The codes aims to do these things: read in data files; join the fuel data to the Leeds geospatial file by LSOA code; check the data type, found a object which should be  int, so change it as it should be;
check if there are any missing values, luckily not; describe the variables needed and create histograms for them; divide the regions into 10 groups shareing similar households number, and calculate their average fuel poverty rate;
create a bar chart for the groups' average fuel poverty rate; create choropleth maps for the households number and fuel poverty rate to evaluate if there's any distribution injustice.
