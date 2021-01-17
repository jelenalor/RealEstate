# London real estate market
<i>January 2021</i>

### Statistical analysis of the real estate prices in London from custom made RDS Database built by myself using AWS (free tier) and scraping public data

#### Database 
 - Property prices for each sale transaction since 1995 (poscode, address, property type)
 - EPC certificate data (property characteristics such as sq ft, number of bedrooms, and current and potential energy efficiency 
 - Crime since 2008 (Crime rates by type of crime and lower layer super output areas (LSOA - the area larger than the postocde but smaller than the district))
 - Schools and their characteristics by LSOA
 - High quality grocery stores by LSOA (Foursquare API 1km search radious for each lsoa)
 - Venues by LSOA (bars, restaurants offices)
 - Tube stations by LSOA
 - Historical GDP, Interest rates and house price index (HPI) 
 - Geographic boundaries
 
#### Data Cleaning
Data was cleaned using Python before loading into the Database. <br>
EPC property data was matched to Property pricing data on address using fuzzy string matching algorithm fuzzywuzzy as per below:
- The address in both datasets were converted into the string in a format > "House number, flat number, street"
- Numeric and alpha characters were separated and matched individually. Each match was performed at a post code level.
- Only match of 100% for numbers and > 50% for alpha characters were kept as a correct match. This is because sometimes street names, house names are written slightly differently.

 
#### IDEAS
- Identify best areas to invest in (areas with good access to schools, stores, public transport, low crime rates but significantly less prices property) [Clustering, similarity]
- Estimate the $ or % impact onto the house price due to its proximity to good schools or good stores [Regression]
- Examine and visualize the most sought after areas in London
- Built web based app providing detailed info into the area and past sales for a chosen post code (crime rates, schools catchment, availability of good stores or transportations)
- Built house price predictor/estimator model 
- Analyse how the economy impacts house market (credit availability, economic crises or growth)
- Identify the areas with the highest rate of growth in sales/ prices in the last 5 years and understand the drivers 
 
 
#### Data Sources:
- UK Gov
- Foursquare
- epc.opendatacommunities.org
- Bank of England
