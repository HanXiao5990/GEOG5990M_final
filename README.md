# GEOG5990M_final
# The background/context of the project:
This project is doing a public resource assessment, to evaluate is fuel resource distributed equally in Leeds.
This idea is derived from a Environmental Assessment(EA) concept: Environmental Justice Analysis. It is an assessment tool usually used to assess the distribution equity of air quality or other shared resources.
This approach is used here to assess fuel distribution within the city of Leeds, to see if it's related with the deprivation, because many researches showed that nowadays people are facing the problem of fuel poverty, especially in winter.
The purpose of this report is to show Public and Policymaker an exploration of the uneven distribution of fuels. Hope it can inspire and help the improvement of social welfare in the future.
# What data the GitHub repository contains:
there are two data files needed, one contains the households number and proportion of fuel poverty situation and the other contains the boundary of Leeds, the two data are from different data source. Noted below:
(1)Fuel poverty by LSOA.csv;  data sources: Data Mill North https://datamillnorth.org/dataset/2j70l/fuel-poverty-by-lsoa-england
(2)Leeds.geojson;  data sources: Office for national statistics https://geoportal.statistics.gov.uk/maps/761ecd09b4124843b95511a242e2b1a1
(3)File_1_ID_2015_Index_of_Multiple_Deprivation.csv;  data source: gov.uk https://www.gov.uk/government/statistics/english-indices-of-deprivation-2015
# What the code aims to do:
The codes aims to do these things: read in data files; join the fuel and deprivation data to the Leeds geospatial file by LSOA code; check the data type, found a object which should be  int, so change it as it should be;
check if there are any missing values, and drop the rows with missing values; describe the variables needed and create histograms for them; divide the regions into 10 groups shareing similar households number, and calculate their average fuel poverty rate and average deprivation;
create a bar chart for the groups, showing each group's average fuel poverty rate and average deprivation; create choropleth maps for the deprivation and fuel poverty rate to evaluate if there's any distribution injustice.
# Any further information someone might need to be able to run your code and reproduce your analysis:
nothing more need to be informed with the codes, they should be fine. There's only one thing needs to notice: From the variable name in the origin file we can see that the variable name is" Index of Multiple Deprivation (IMD) Decile (where 1 is most deprived 10% of LSOAs)", which means ther lower deprivation decile in this dataset, actually indicates higher deprivation, we multiplied this variable by 10 and the resulting new variable should still maintain this trend. It's still confusing to me but, it actually doesn't matter if the high deprivation index indicates high poverty or high wealth because eventually, the two maps ( average deprivation and proportion of fuel poverty)show complementary states, so either way, there is indeed unequal distribution of fuel energy.
