---
layout: post
title: Wildfires in British Columbia
subtitle: Tableau Dashboard
gh-repo: ranjitprakash1986/wildfire_analysis
gh-badge: [star, fork, follow]
cover-img: /assets/img/banner-dark.jpg
thumbnail-img: /assets/img/wildfires_dashboard.jpg
share-img: /assets/img/path.jpg
tags: [Tableau, Dashboard, Data Analysis, Data Insights]
---
### Summary

There is an increasing focus on mitigation of extreme weather events across the world. The fallacy of mankind is perhaps the tendency to value short-term benefits in the face of long-term detriments. While manifesting in different forms ; floods, heatwaves, droughts, wildfires - the ongoing weather patterns have forced governments to make pre-emptive efforts to avoid further escalation. British Columbia, had its worst wildfire season, surpassing the previous record set in 2018. Thus it is essential to understand if there is a direct correlation between the climate factors such as temperature, precipitation and surface winds and the severity of wildfires. These "apparent" correlations that need to be statistically verified which could be a further extension of this project which mainly portrays the visualization of the existing data after data cleaning. Here is a brief overview, and links to my [Dashboard](https://public.tableau.com/app/profile/ranjit.sundaramurthi/viz/BCWildfires_16962267361080/Dashboard1) and [Github](https://github.com/ranjitprakash1986/wildfire_analysis)

### Data Wrangling and Visualization: 

I gathered open-source data from [canada.ca](www.canada.ca) and [nrcan.gc.ca](www.cwfis.cfs.nrcan.gc.ca). I wrangled vector data from shape-files for the wildfires data. These files provide the location (longitude and latitude) and the burnt area geometry in Canada. I aggregated this data at the yearly granularity level and performed spatial join to trim it down to records specific to British Columbia. You can check out the Python scripts for this data wrangling on my GitHub repository. The Tableau visualization brings the datasets for wildfires, temperature, precipitation and wind speed, together in one place to let use investigate "apparent" correlations.

### Key Takeaway: 

From 2017 onward, the area burnt by wildfires in British Columbia spiked dramatically. Even though the number of unique fire events remained relatively steady, it indicates that these fires were harder to suppress, thereby burning larger areas. The average summer temperature increased by 8% from 1986 to 2022, while summer precipitation showed a declining trend after 2008. This could indicate that the drier and hotter summers create conditions appropriate for raging wildfires. Oddly, surface wind speeds decreased over time. As mentioned again, these are conjectures that need to be statistically verified before making any claims.


### Limitations 

This analysis is an over simplified overview of wildfires and its possible drivers. It is highly likely that several factors, not included in this assessment play a major part in driving wildfires. These include the extent of vegetation, the type of vegetation, localized weather metrics rather that provincial averages and several others. I do not claim to be an expert in this domain, however found it interesting to explore myself.

Note: The precipitation data is until 2017, wind speed data is until 2014, while the ongoing 2023 wildfire season is not fully updated.