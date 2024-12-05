# U.S. Elections 2024

This repository contains data scraped from the [New York City Board of Elections website](https://enr.boenyc.gov/). 

Resulting analysis will be used for a reporting assignment that looks into voting results in the Bronx, for the [Mott Haven Herald](https://motthavenherald.com/) and [Hunts Point Express](https://huntspointexpress.com/). 

![image](/viz/viz-map-rev.png)

## Data sources

* [New York City Board of Elections website](https://enr.boenyc.gov/)
* Election districs, from [NY Open Data](https://data.cityofnewyork.us/City-Government/Election-Districts/h2n3-98hq) — `nyed_20241121.csv`

## Content and process

### notebooks

* `scraper.ipynb` used `BeautifulSoup` to scrape vote results per election district in the Bronx
* `clean-up.ipnyb` prepared and sanitized dataset for visualization

I created a new column that merges the assembly district and election district numbers, so we have a code consistent with geocode IDs. 

In an earlier version, I added all Trump votes and Harris votes, then calculated the differential vote counts for choropleth mapping. **In this version**, I also calculated for the percentages of Trump and Harris votes, so we can use a fixed barometer (percentage points) to compare with other election years.

I use vote differential to visualize the data — instead of simply counting the number of votes — because *lands don't vote; people do*.

### `csv` files

* `bx-assembly_districs.csv` holds all links of Bronx assembly district votes breakdown
* `electoral_district_votes.csv` holds scraped unofficial election night results in each of the electoral districts in Bronx assembly districts
* `2020_votes_full` holds our main dataset, which includes vote counts and percentage of votes (both per candidate and totals)

### `viz`

This folder holds our Illustrator and exported PNG file. 