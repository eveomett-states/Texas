# Texas Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Ananya Agarwal.

# **Sources**

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/texas-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2021-texas-congressional-districts-adopted-plan/): 2021 Texas Congressional Districts plan enacted on 11/11/21

[State House District data](https://redistrictingdatahub.org/dataset/2021-texas-state-house-adopted-plan/): 2021 State House Approved Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2021-texas-state-senate-adopted-plan/): 2021 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-texas-precinct-boundaries-and-election-results/)**:**  VEST 2020 Texas precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-texas-precinct-boundaries-and-election-results/)**:**  VEST 2018 Texas precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-texas-precinct-and-election-results/)**:**  VEST 2016 Texas precinct and election results

# **Processing**

Demographic data were aggregated from the census block level and precincts were assigned to districts using [MGGG's proration software](https://github.com/mggg/maup). Election data were also prorated onto VTDs from the original precinct shapefile using the `maup` package.

## Metadata
* `CNTYVTD`: VTD unique identifier
* `VTD`: VTD name
* `WHITE`: 2010 White population
* `OTHER`: 2010 Other race population
* `HISPANIC`: 2010 Hispanic population
* `TOTPOP`: 2010 Total population
* `VAP`: 2010 Total voting age population
* `BLACK`: 2010 Black population
* `BLKHISP`: 2010 Black hispanic population
* `WVAP`: 2010 White voting age population
* `HISPVAP`: 2010 Hispanic voting age population
* `BHVAP`: 2010 Black hispanic voting age population
* `BVAP`: 2010 Black voting age population
* `OTHVAP`: 2010 Other race voting age population
* `COUNTY`: County name
* `FIPS`: County FIPS code
* `PRES12R`: Number of votes for 2012 Republican presidential candidate
* `PRES12D`: Number of votes for 2012 Democratic presidential candidate
* `SEN12R`: Number of votes for 2012 Republican senate candidate
* `SEN12D`: Number of votes for 2012 Democratic senate candidate
* `TOTVR12`: Number of registered voters in 2012 general election
* `TOTTO12`: Number of ballots cast in 2012 general election
* `SEN14R`: Number of votes for 2014 Republican senate candidate
* `SEN14D`: Number of votes for 2014 Democratic senate candidate
* `GOV14R`: Number of votes for 2014 Republican gubernatorial candidate
* `GOV14D`: Number of votes for 2014 Democratic gubernatorial candidate
* `TOTVR14`: Number of registered voters in 2014 general election
* `TOTTO14`: Number of ballots cast in 2014 general election
* `PRES16D`: Number of votes for 2016 Democratic presidential candidate 
* `PRES16R`: Number of votes for 2016 Republican presidential candidate
* `TOTVR16`: Number of registered voters in 2016 general election
* `TOTTO16`: Number of ballots cast in 2016 general election
* `USCD`: U.S. Congressional District ID
* `SEND`: Texas State Senate District ID
* `HD`: Texas State House District ID
* `AREA`: Area of vtd in square kilometers
* `PERIM`: Perimeter of vtd in kilometers

## Projection
This shapefile uses a NAD83/Texas State Mapping System projection (EPSG: 3081).