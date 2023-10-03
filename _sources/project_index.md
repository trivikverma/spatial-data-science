# Project Details


## 1. Relationship between mobility, built environment and environmental sustainability indicators of a city

Urban mobility significantly contributes to global environmental impact. With growth in urban areas worldwide, cities are implementing policies to focus on sustainable urban and mobility development. Urban areas exhibit high variability in structure, economic output, mobility behavior, among others. Pinpointing to the exact causes of emissions is impossible. However, understanding the relationship of mobility with infrastructure resources and other urban indicators may help governments predict long-term mobility behaviour and intervene with future pathways into sustainable mobility options.

Project goals: You are tasked to identify how mobility is related with infrastructural form of a city and across multiple cities. Use your findings toward helping governments transform mobility within cities for reducing environmental impacts of mobility use.

### Data

1. Local city-wide indicators of urban mobility: [Multi-city Traffic Dataset](https://utd19.ethz.ch/) provided publicly by The Institute for Transport Planning and Systems at ETH Zurich.

2. Global city-wide indicators of urban mobility and environmental impacts: [Urban Typologies Project](http://web.mit.edu/afs/athena.mit.edu/org/i/its-lab/www/dashboard/new%20dashboard/index.html)
[[Reference](https://iopscience.iop.org/article/10.1088/1748-9326/ab22c7)]

3. Get indicators for infrastructure resources from OSMNX (street networks) and PYROSM (amenities and points of interest) python packages.

#### High-level project goals

1. Explore, Investigate, and Visualize various factors of the mobility data across cities of interest.
2. Describe and incorporate additional data sources that you will use to help you understand relationships between mobility and the built environment.
3. Identify correlations between mobility and the built environment.
4. Perform clustering or LISA analysis on city streets where congestion may be related strongly with presence of certain amenities. Think how that may vary with distance to amenities.
4. Or, train and evaluate models using the mobility data (either as predictors or as the primary
response in some fashion) and your own data sources.
6. Use and interpret your models to discuss the causes and correlations of or effects due to differences in congestion across cities or within a city of your choice.
7. Aggregate city-wide findings to correlate with environmental indicators used in data set (2) - urban typology - to comment on policy intiatives of the governments. (Think how you may aggregate city-wide findings to a single score for the whole city to cpmare with indicators used in data set (2))

Note: Not all data may be available for all cities. Hence, conduct this analysis for at least _5_ cities overlapping between sets _1_ and _2_ in the data. You are welcome to do on many more cities.

## 2. Comparison of the distribution of health and emergency services infrastructure across The Netherlands with ?

COVID-19 pandemic has revealed very clearly how our health infrastructure is not resilient. For gloabl health policy, the challenges for decision-makers are not only to understand which communities are vulnerable and where they are located but also assess how resilient the city is to various shocks (natural disasters, evacuations, health emergencies, etc). People who are exposed the most to certain events like extreme heat, are also the most vulnerable to it becauuse they are mostly low-income single households with kids and elderly with mobility issues [[Ref](https://www.nytimes.com/interactive/2020/08/24/climate/racism-redlining-cities-global-warming.html)]. The lack of greenery in their residential areas may even amplify such shocks. It is not an easy task to build infrastructure in a city that is going to be optimally located for all citizenry. Knowledge of spatial and temporal variability of infrastructure use can provide policy-makers with insight about potential interventions.

Project goals: You are tasked to identify trends in ambulance calls across a city and/or in time and measure its relationship with indicators of socio-economic status of households, neighbourhoods or regions.

### DATA

1. We will provide you with an emergency **calls** dataset (ambulance, firefighter, police, and coastguards) of The Netherlands collected from January 2017 to September 2020. That also includes calls made to these services during the period of lockdown and release cycles in the pandemic.
**Since the data is not open-source yet, please send an email to me requesting access to it. Kindly do not share it with anybody outside of your project group.**

2. A few selected OpenData resources
[Den Haag Cijfers](https://denhaag.incijfers.nl/jive)
Statistics Bureau of The Netherlands [CBS](https://www.cbs.nl/nl-nl/reeksen/kerncijfers-wijken-en-buurten-2004-2020)

The calls dataset has the following indicators and was obtained from [112-Nederland](https://www.112-nederland.nl/),

`pmeId` - Related to the id on the website
`pmeTimeStamp` - Time of call registered
`pmeProtocol1` - P2000 protocol related info
`pmeProtocol2` - P2000 protocol related info
`pmeTarget` - P2000 protocol related info
`pmeMessage` - Original message​
`pmePrio` - Priority of the message
`pmePrioLevel` - Conversion of priority to a normalized level
`pmeDienst` - A=Ambulance, B=Brandweer, P=Politie
`pmeStrippedMessage` - Cleaned Message of the call
`pmeStraat` - Street
`pmeHouseNumber` - Mid-point of the street closest to location of call (for data privacy)
`pmeHouseNumberAdd` - Addition to house number
`pmeANRoad` = A=highway, N=Provincial Way
`pmeHectometerpaal` = Location on A or N way
`pmeZip` - Zip code of the area
`pmeRegionName` - Name of region
`pmeLatitude` = wgs84
`pmeLongitude` = wgs84
`pmeHash` - Ignore internal indexing (for collection purposes only)
`pmeGeoAccuracy` = H=Housenumber, S=Street
`pme_strId` = Street Id
`pme_wplId` = Woonplaats Id
`pme_gemId` = Gemeente Id
`pme_proId` = Province Id
`pme_vrgId` = Veiligheidsregio Id
`pmeCapCodes` = Capcodes
`pmeLifeLiner` - True/False (Extraction by air)
`wplName` = Woonplaats
`gemName` = Gemeente / Municipality

#### High-level project goals

1. Explore, Investigate, and Visualize various factors of the emergency services call data: geographic differences and time trends. Example: compare time trends, city trends, or both. You may also choose one city and focus on that.
2. Describe and incorporate additional data sources that you will use to help you understand or use the calls data. Example: demographic data from municipalities in The Netherlands or CBS data as used during assignments.
3. Train and evaluate models using the calls data (either as predictors or as the primary
response in some fashion) and your own data sources.
4. Or, Cluster calls based on some socio-economic indicators of urban regions around The Netherlands.
6. Use and interpret your models to discuss the causes and correlations of or effects due to differences in calls across cities or within a city of your choice. (You may use the Pyrosm package to find locations of health infrastructure and other amenities in a city, and use the Osmnx package to find road-distance to nearest locations from a certain region in a city).

## 3. Modelling COVID-19 in India

COVID-19 has proven to be one of the deadliest pandemics in history. Our policymakers have diminished the consequences and impacts of varied measures to mere models and numbers. Schools have shut down for months, crime and abuse has risen and millions of people have lost their jobs. In India, multiple comunnities of migrant labourers, minorities and children have disproportionately been affected by the pandemic. It is imperative to project where our policy measures our needed most, and how to implement them, to reduce the disproprtionate impact on life and work of countless families across the world.

Project goals: The primary goals of this project are to (1) identify the socio-economic composition of communities affected by COVID-19 across India. (2) compare the characteristics of these communities based on their geography and socio-economic indicators.

### DATA

1. [DDL Covid India](http://www.devdatalab.org/covid): Open-source COVID-19 data that tracks the spread of the disease in India curated by the Development Data Lab.

#### High-level project goals

1. Obtain publicly available county-level data from the source above (demographics,
health indicators, etc.) and combine with COVID-19 case counts at the county-level.
Use state-wide policy data if you can find. You can also use the socio-economic data of India from the same lab found [here](http://www.devdatalab.org/shrug).
2. Explore, Investigate, and Visualize various factors of the demographics of India.
3. Build clustering models for identifying the composition of communities that are affected by COVID-19. Example: Who they are? How are they impacted? What is their socio-economic condition?
3. Compare the impact of governmental policies on controlling the disease based on your
clustering models. Example: how could have policy measures impacted communities differently?
