# London real estate market

### Statistical analysis of the real estate prices in London from custom made RDS Database built by myself using AWS (free tier) and scraping public data

#### Database 
 - Property prices for each sale transaction since 1995 (poscode, address, property type)
 - EPC certificate data (property characteristics such as sq ft, number of bedrooms, and current and potential energy efficiency 
 - Crime since 2008 (Crime rates by type of crime and lower layer super output areas (LSOA - the area larger than the postocde but smaller than the district))
 - Schools and their characteristics by LSOA
 - High quality grocery stores by LSOA
 - Venues by LSOA (bars, restaurants offices)
 - Tube stations by LSOA
 - Historical GDP, Interest rates and house price index (HPI) 
 
 
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
