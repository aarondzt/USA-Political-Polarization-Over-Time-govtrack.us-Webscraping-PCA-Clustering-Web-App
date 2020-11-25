# Data-driven Congressional subgroups
* A pipeline for extracting Congressional voting records from any year + PCA + clustering

## Contents
* [Data source](https://www.govtrack.us/congress/votes)
* [Data files for House](data_house)
* [Data files for Senate](data_senate)
* [House report (ignore for project grading)](2020%20House.ipynb)
* [Senate report](2020%20Senate.ipynb)

### Overview
Congressional voting patterns go beyond Democrat vs. Republican party lines. In this project, I "scrape" voting record data from GovTrack, extract all the representatives and their votes, and perform clustering in order to determine subgroups within the Democratic and Republican parties. Interestingly, for both parties, there is a "mainstream" voting cluster and distant clusters that represent smaller factions within the parties. I performed this analysis for both the House of Representatives and the Senate, but I decided to focus my analysis on the Senate because there are fewer members, and those members are more widely known.
### Goals
My main goal was to build a data extraction pipeline for GovTrack that could be used to run interesting analyses on Congressional voting patterns from any year. 
### Data
Data was "scraped" from https://www.govtrack.us/congress/votes. On this page are all the votes for both chambers of Congress that can be filtered by year, chamber, category, etc. In each vote's page, there is a .csv file that contains the names of all the present representatives and their vote.
