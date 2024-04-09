---
name: Homework Assignment 8
tools: [Python, HTML, Altair/Vega-Lite]
image: assets/pngs/visualization.png
description: Homework 8 which uses altair/vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Vega Lite Example Project

This page demonstrates the output of the interactive visualizations I created for Homework 8 of IS 445 Class. I used the building inventory dataset. The visualizations were created with Python, Altair and Vega-Lite showcasing different intuitive aspects that can be derived from this dataset.

## Visualization 1: Histogram Plot - Building Ages based on Year Constructed 
<vegachart schema-url="{{ site.baseurl }}/assets/json/histogram.json" style="width: 100%"></vegachart>

This interactive histogram dynamically visualizes the ages of buildings, with age calculated as the current year minus the construction year. "Building Age" is on the x-axis, and the count of buildings is on the y-axis, collectively plotting buildings into discrete age bins and highlighting the distribution across various age categories. The encodings used include a quantitative representation of age (x-axis), aggregated counts of buildings (y-axis), color to emphasize distribution, and tooltips for detailed insights. A single color (slateblue) is applied to all bars in the histogram to focus on the distribution shape rather than differentiating between categories. The histogram's interactivity and analytical depth are significantly enhanced by preprocessing steps for data accuracy, including handling missing values and calculating building ages, alongside an interactive age slider that allows viewers to adjust the displayed age range. These design choices craft a comprehensive tool for exploring the age distribution of the building inventory. Hence, this visualization is a great way to make the age data of buildings accessible and engaging.


## Visualization 2: Scatter Plot - Building Year Acquired vs Square Footage

<vegachart schema-url="{{ site.baseurl }}/assets/json/scatterplot.json" style="width: 100%"></vegachart>

This interactive scatter plot explores the relationship between the acquisition year and square footage of buildings, categorized by their usage description. Each point represents a building, plotted to illustrate how its size and the period it was acquired vary by usage type. The visualization has encodings for the  Year Acquired (x-axis), Square Footage (y-axis), color ("Usage Description"), and tooltips, which were optimized by setting the x-axis domain to the actual range of "Year Acquired" in the dataset, ensuring efficient use of space and avoiding data cramping. The logarithmic scale on the y-axis allows for better comparison across buildings of different sizes. The color encoding differentiates buildings based on their usage, adding a layer of categorization that enriches the analysis. This allows viewers to see patterns in how different types of buildings are distributed in terms of size and acquisition year. Interactivity includes a dropdown menu for filtering by usage, adding an enhancive layer for targeted analysis. In particular, the year range on the x-axis had to be adjusted to start from the minimum year in the data instead of zero, to reflect the true temporal spread of the data, improving the plot's clarity and interpretability. These adjustments make the scatter plot more intuitive and informative, facilitating the users' exploration of how building characteristics have evolved over time with respect to their usage purposes.


## Data & Methods

For further information about the data and a detailed analysis, please refer to the links below:

<div class="left">
{% include elements/button.html link="https://github.com/Nitya01/Jekyll-pages/tree/main/_data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Nitya01/Jekyll-pages/tree/main/python_notebooks/IS-445-HW8.ipynb" text="The Analysis" %}
</div>
