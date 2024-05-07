---
name: Final Project Part 3
tools: [Python, HTML, Folium]
image: assets/pngs/cover_pic.png
description: Final Project with semi-real time interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

<h2 align="center">Earthquake Data - Interactive Dashboard Webpage</h2>
Welcome to the interactive earthquake observatory, built by Group 1, for the Final Project of Data Visualizations Coursework

<h3 align="center">Visualization 1: Geopandas Plot with Matplotlib Markers</h3>
<iframe src="{{ site.baseurl }}/assets/html/visualization_1.html" width="100%" height="450" frameborder="0" allowfullscreen></iframe>

In this visualization, geopandas was used to create a geographical plot of the earthquake events. You can see the earthquakes on the map, they are color coded by the magnitude and sized by depth. Users can use this visualization to gain insights into earthquake occurrences and their spatial distribution such as identifying high seismic regions. The patterns can be analyzed to see if there is correlation between earthquakes’ magnitude, depth, and geographic locations. Users can assess the impacts of recent earthquakes, which can help with disaster preparedness and responses.



<h3 align="center">Visualization 2: Time Series Plot</h3>

<iframe src="{{ site.baseurl }}/assets/html/visualization_2.html" width="100%" height="600" frameborder="0" allowfullscreen></iframe>

The second plot an interactive time series chart illustrating daily earthquake frequencies over a specific period. Displayed on the x-axis are the dates, while the y-axis quantifies the daily counts of earthquakes. The line graph, marked with red points at each data point, illustrates the trend in earthquake occurrences over this one-month period (early March to early April 2024). An interactive feature allows the users to hover over the points on the line to get the exact date and  enhances user engagement. This feature aids in the detailed examination of trends and anomalies in earthquake activities, making this visualization a practical resource for those tracking seismic patterns.

<h3 align="center"> Visualization 3: Scatter Plot - Earthquake's Depth vs Magnitude </h3>

<iframe src="{{ site.baseurl }}/assets/html/visualization_3.html" width="100%" height="600" frameborder="0" allowfullscreen></iframe>

The scatter plot illustrates the relationship between the depth at which earthquakes occur and their respective magnitudes. As shown, most earthquakes occur at shallower depths, with the majority of magnitudes clustering between 0 and 2 on the Richter scale. Interestingly, the plot highlights that while high-magnitude earthquakes (above 4.0) can occur at various depths, they predominantly appear at depths less than 100 km. The plot also displays a few outliers, where significant earthquakes have occurred at greater depths, showing that high-magnitude earthquakes are not exclusively shallow. This visualization can help in understanding the distribution and frequency of earthquake magnitudes in relation to their depths, providing crucial insights for geoscientific studies and earthquake preparedness initiatives.

<h3 align="center">Visualization 4: Folium Plot - Overall Earthquake locations on semi real-time global map</h3>

<iframe src="{{ site.baseurl }}/assets/html/earthquake_map.html" width="100%" height="600" frameborder="0" allowfullscreen></iframe>

Finally we present an interactive map visualization designed to enable users to explore seismic events. The map features a clustering mechanism that efficiently manages the display of numerous markers. Users can interact with the map by zooming in and out, as well as panning across different geographic regions. Clicking on individual markers reveals detailed information about each earthquake, including its magnitude, depth, type, and exact location. This interactive tool aims to provide valuable insights into the patterns and details of earthquake occurrences worldwide.


<h3 align="center">Earthquake Data</h3>

For further information about the data please refer to the link below:

<div style="text-align: center;">
{% include elements/button.html link="https://github.com/Nitya01/Jekyll-pages/tree/main/_data/all_month.csv" text="The Data" %}
</div>