---
layout: post
title: An Insight into the Oil Market
subtitle: Dashboard created in Dash
cover-img: /assets/img/banner-dark.jpg
thumbnail-img: /assets/img/dashboard_Oildex.jpg
tags: [Dashboard, Dash, Python]
comments: true
---

## Summary

The objective of this dashboard is to enable an executive or any investor interested in Schlumberger (SLB) to get an immediate overview of the Oil market within a specific selected year range. It also enables to compare the Oil prices with the SLB and the S&P 500 stock prices. Please see this detailed [proposal](https://github.com/ranjitprakash1986/Oildex/blob/main/docs/proposal.md) for more information on the motivation and description of the data.

The Dashboard page presents the user with widgets to select the year range of interest between 1986 - 2022 at the top. The selected year range filters the lineplots which reveal the trends in Oil price movement with changes in the drilling activity represented by Rig Count. The next line plot compares the trend of Oil price with SLB stock price. Due to the varying scales of prices, a third plot shows the normalized prices of Oil, SLB stock, S&P500 stock index. This enables the user to see the changes in trend on an even scale.

![dashboard_layout](../assets/img/dashboard-layout-oildex.png)

The bottom half of the Dashboard shows a stacked barplot with the Rig Counts. These can be visualized by different regions of interest. Please note that the regions selected only affect the stacked barplot and do not affect the lineplots.

The latest version of the dashboard is deployed on Render [here](https://oildex-dash.onrender.com/).

For complete details and code, please visit the GitHub [repository](https://github.com/ranjitprakash1986/Oildex).
