# U.S. Elections 2024

This repository contains data scraped from the [New York City Board of Elections website](https://enr.boenyc.gov/). 

Resulting analysis will be used for a reporting assignment that looks into voting results in the Bronx, for the [Mott Haven Herald](https://motthavenherald.com/) and [Hunts Point Express](https://huntspointexpress.com/). 

## Data sources

* [New York City Board of Elections website](https://enr.boenyc.gov/)
* Election districs, from [NY Open Data](https://data.cityofnewyork.us/City-Government/Election-Districts/h2n3-98hq) — `nyed_20241121.csv`

## Content

* `bx-assembly_districs.csv` holds all links of Bronx assembly district votes breakdown
* `electoral_district_votes.csv` holds scraped unofficial election night results in each of the electoral districts in Bronx assembly districts
* `electoral_district_for_viz.csv` holds "prepared" data for viz