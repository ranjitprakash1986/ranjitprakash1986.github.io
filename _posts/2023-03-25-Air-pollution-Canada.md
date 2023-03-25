---
layout: post
title: Trends in Air Pollution in Canada
subtitle: Dashboard created in Shiny R
cover-img: /assets/img/banner-dark.jpg
thumbnail-img: /assets/img/pollution-skyline-canada.jpg
tags: [Dashboard, Dash, R]
comments: true
---

## Summary

Air pollutants are increasingly impacting the health and quality of life of Canadians and their levels are tracked across Canada on an hourly basis by the National Air Pollution Surveillance (NAPS) Program in Canada. This data is however stored in hard to understand data files on a yearly basis and is not very accessible to regular Canadians. To address this challenge, we propose building a data visualization app that allows all Canadians to visually explore the dataset of NAPS to better understand the changing trends of air pollution in Canada. Our app will show how the levels of various air pollutants, such as CO2 and NO2, have changed from 2001-2020 and allow users to explore different aspects of this data by selecting different pollutants and zooming in to the province and city level.

![dashboard-layout](../assets/img/dashboard-layout-air-pollution-canada.png)

The landing page presents the user with options on the left side to select a Province in Canada or/and a specific City in Canada via drop-down menus. The pollutants of interest can be selected via checkboxes. By default, these options are set as entire Canada and all pollutants. This corresponds to the following selections, Select Province: "All" , Select City: Inactive, Select Pollutant: "All". The dashboard provides definitions of the pollutants, model assumptions and a summary to provide an overall insight. The attributions and credits are enlisted for user convenience.

The latest version of the dashboard is deployed on Render [here](https://extra.shinyapps.io/air-pollution/). Please allow a some time for the Dashboard to load.

For complete details and code, please visit the GitHub [repository](https://github.com/ranjitprakash1986/Air_Pollution_Canada).
