# Real-Estate-of-USA---Caltech-Project---Center-for-Technology-Management-Education
Capstone Project - California Technology - Center for Technology &amp; Management Education
1. A banking institution requires actionable insights into mortgage-backed 
securities, geographic business investment, and real estate analysis.

2. The mortgage bank would like to identify potential monthly mortgage 
expenses for each region based on monthly family income and rental 
of the real estate. 

3. A statistical model needs to be created to predict the potential demand 
for amount of loan in dollars for each of the region in the USA. Also, 
there is a need to create a dashboard which would refresh periodically, 
post data retrieval from the agencies.

4. The dashboard must demonstrate relationships and trends for the key 
metrics as follows: number of loans, average rental income, monthly 
mortgage and owner’s cost, family income vs mortgage cost 
comparison across different regions. The metrics described here do 
not limit the dashboard to these few.

The objective is to identify white spaces/potential business in the mortgage loan. The mortgage bank would like to identify potential monthly mortgage expenses for each of region based on factors which are primarily monthly family income in a region and rented value of the real estate. Some of the regions are growing rapidly and Competitor banks are selling mortgage loans to subprime customers at a lower interest rate. The bank is strategizing for better market penetration and targeting new customers. A statistical model needs to be created to predict the potential demand in dollars amount of loan for each of the region in the USA. Also, there is a need to create a dashboard which would refresh periodically post data retrieval from the agencies. This would help to monitor the key metrics and trends.

The dashboard must demonstrate relationships and trends for the key metrics as follows:  number of loans, average rental income, monthly mortgage and owner’s cost, family income vs mortgage cost comparison across different regions. The metrics are described not to limit the dashboard to these few only.

Dashboard Link on Tableau Public: https://public.tableau.com/views/USARealEstate-CapstoneProject/USARealEstate?:language=en-US&:display_count=n&:origin=viz_share_link

## Dataset

| Column Name                     | Details                                                                                                                                                                        |
|---------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| UID                           | The ID of the location of which you are analyzing. ID location compatible across all Golden Oak Research Locations.                                                                                      |
| BLOCKID                            | Block ID of tract. If there is no specified block id the location is then a tract. The maximum number of blocks for any given track is 9.                                                                                                      |
| COUNTYID                           | The County Code reported by the U.S. Census Bureau for the specified geographic location.                                                                          |
| STATEID                    | The state code reported by the U.S. Census Bureau for the specified geographic location.                                                                                                       |
| state                         | The state name reported by the U.S. Census Bureau for the specified geographic location.                                         |
| state_ab                        | The abbreviated state name reported by the U.S. Census Bureau for the specified geographic location.                                                                                                                         |
| city                             | The closest city name reported by the U.S. Education Department by the closest school relative to the Census Location.                                 |
| place                             | The place name reported by the U.S. Census Bureau for the specified geographic location.                                                                                                                      |
| type                      |  The place Type reported by the U.S. Census Bureau for the specified geographic location.                                                                              |                                                                                     |
| primary                      |  TDefines whether the location is a tract location or a block group.                                                                              |                                                                                     |
| zip_code                      |  The closest zip code reported by the U.S. Education Department by the closest school relative to the Census Location.                                                                              |                                                                                     |
| area_code                      |  The area code reported by the U.S. Census Bureau of the closest geographic location with area code information.                                                                              |                                                                                     |
| lat                      |  The latitude of geographic location.                                                                             |                                                                                     |
| lng                      |  The longitude of geographic location.                                                                             |                                                                                     |
| ALand                      |  The Square area of land at the geographic or track location.                                                                             |                                                                                     |
| AWater                      |  The Square area of water at the geographic or track location.                                                                             |                                                                                     |
| pop                      |  Male and Female population of the geographic location.                                                                             |                                                                                     |
| male_pop                      |  Male population of the geographic location.                                                                             |                                                                                     |
| female_pop                      |  Female population of the geographic location.                                                                             |                                                                                     |
| rent_{stats}                      |  The {stats} gross rent of the specified geographic location (stats include mean, median, stdev, sample_weight and samples). While sample_weight is the sum of gross rent weight used in calculations. and samples refer to The number of gross rent records used in the statistical calculations.                                                                             |                                                                                     |
| rent_gt_x                      |  The empirical distribution value that an individual’s rent will be greater than x% of their household income in the past 12 months (x varies in pre-defined set [10, 15, 20, 25, 30, 35, 40, 50]).                                                                             |                                                                                     |
| universe_samples                      |  The size of the renter-occupied housing units sampled universe for the calculations.                                                                             |                                                                                     |
| used_samples                      |  The number of samples used in the household income by gross rent as percentage of income in the past 12 months calculation.                                                                              |                                                                                     |
| hi_{stats}                      |  The {stats} household income of the specified geographic location. {stats} include mean, median, stdev, sample_weight and samples. sample_weight is the number of households used in the statistical calculations.                                                                             |                                                                                     |
| family_{stats}                      |  The {stats} family income of the specified geographic location. {stats} include mean, median, stdev, sample_weight and samples.                                                                             |                                                                                     |
| hc_mortgage_{stats}                      |  The {stats} Monthly Mortgage and Owner Costs of specified geographic location.                                                                              |                                                                                     |
| hc_{stats}                      |  The {stats} Monthly Owner Costs of specified geographic location.                                                                             |                                                                                     |
| home_equity_second_mortgage                     |  percent of houses with a second mortgage and home equity loan.                                                                              |                                                                                     |
| second_mortgage                      |  percent of houses with a second mortgage.                                                                             |                                                                                     |
| home_equity                     |  percent of houses with a home equity loan.                                                                              |                                                                                     |
| debt                      |  percent of houses with some type of debt.                                                                             |                                                                                     |
| {}_cdf                      |  Cumulative distribution value of one minus the percentage of homes with a {second mortgage, home equity, debt(any home related debt)}. The value is used as a performance feature.                                                                              |                                                                                     |
| hs_degree_{}                      |  Percentage of {peole, male, female} with at least high school degree.                                                                               |                                                                                     |
| male_age_{stats}                    |  The {stats} age of males in the geographic location.                                                                               |                                                                                     |
| female_age_{stats}                    |  The {stats} age of females in the geographic location.                                                                               |                                                                                     |
