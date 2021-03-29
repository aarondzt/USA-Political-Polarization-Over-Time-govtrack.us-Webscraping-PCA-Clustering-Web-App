%%%%%%%%%%%%%%%%%%%%

# DATA-690 WEB APPS INSTRUCTIONS
Run voila on Senate Data Analysis.ipynb

%%%%%%%%%%%%%%%%%%%%

# Data-driven Congressional subgroups
A pipeline for extracting Congressional voting records from any year + PCA + clustering

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
### Limitations
One major limitation is that, as much as I tried, I could not find a meaningful interpretation of what PC1 and PC2 represent for both the Democratic and Republican parties. While it does appear to provide separation and aid in picking out the more fringe senators (e.g. progressives, Tea Partiers, etc.), it is very difficult to arrive at a sound conclusion as to what it actually represents. This is in comparison to PC1 for the Senate as a whole, which very obviously represents Democrats vs. Republicans.
### Future directions
In this project, I focus on the current year 2020, but in the future, it would be interesting to run analyses on multiple years and do a comparative analysis with regards to the degree of polarization, the most polarizing issues, the cluster structure, etc.
### Conclusion
I saw [this Tweet](https://twitter.com/seanjtaylor/status/1331426161356808192) today, and found it to encapsulate my motivation for pursuing this project: "Perhaps my most controversial opinion: In machine learning education, the focus on supervised learning and particularly on classification problems gives people a totally misguided idea about how to use data to solve real problems." I wanted to avoid the mostly banal Kaggle/UCI datasets and build a pipeline to gather my own data. Congressional data does not lend itself to sophisticated machine learning classification/regression models, but I believe that by applying PCA + clustering to it, I learned a lot about the structure of our political system - data-driven knowledge that could not be attained just by reading the news. This pipeline could be used to gather data on any Congress, all the way back to the first Congress of 1789, and could provide the basis for very interesting quantitative comparisons of how American politics has evolved over time.

## Project Info
<pre>
Contributors : <a href=https://github.com/aarondzt>Aaron Tan</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Anaconda
Libraries    : numpy, pandas, matplotlib, seaborn, sklearn, urllib.request, re, yellowbrick.cluster
</pre>

<pre>
Date published     : 11.25.2020
</pre>
